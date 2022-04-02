# Trabalho-de-Urna-eletronica

programa
{
	
	funcao inicio()
	{	real turma_t[5], turma1=0.0,turma2=0,turma3=0.0, votos=0.0
		real turma=0.0, contagem=1.0, nulo=0.0, branco=0.0, eleitor=0.0, eleitor_valido=0.0, perc_valido=0.0,perc_nulo=0.0, perc_branco=0.0, perc_ana=0.0,perc_pedro=0.0,perc_rita=0.0,perc_alfredo=0.0,perc_regina=0.0,perc_ricardo=0.0
		real perc_ana1=0.0, perc_ana2=0.0, perc_ana3=0.0,perc_pedro1=0.0,perc_pedro2=0.0, perc_pedro3=0.0, perc_rita1=0.0,perc_rita2=0.0,perc_rita3=0.0, perc_alfredo1=0.0,perc_alfredo2=0.0,perc_alfredo3=0.0,perc_regina1=0.0,perc_regina2=0.0,perc_regina3=0.0, perc_ricardo1=0.0, perc_ricardo2=0.0,perc_ricardo3=0.0
		//turma1 embaixo
		inteiro voto1=77,ana_turma1=0,pedro_turma1=0,rita_turma1=0,alfredo_turma1=0,regina_turma1=0,ricardo_turma1=0
		//turma2 embaixo
		inteiro voto2=77,ana_turma2=0, pedro_turma2=0, rita_turma2=0, alfredo_turma2=0, regina_turma2=0, ricardo_turma2=0
		//turma 3 a baixo
		inteiro voto3=77,ana_turma3=0, pedro_turma3=0, rita_turma3=0, alfredo_turma3=0, regina_turma3=0, ricardo_turma3=0
		
		para (inteiro i=0;i<5;i++)
		{
			escreva("Qual sua turma? ")
			leia(turma)
			turma_t[i]=turma
			enquanto(turma!=1 e turma!=2 e turma!=3)
			{
				escreva("Informe uma turma valida (1, 2, 3) ")
				leia(turma)
			}
			se(turma==1)
			{
				escreva("(Turma 1) Informe seu voto: ")
				leia(voto1)
				
			enquanto(voto1!=1 e voto1!=2 e voto1!=3 e voto1!=4 e voto1!=5 e voto1!=6 e voto1!=10 e voto1!=0)
			{
				escreva("Informe um Voto correto (1,2,3,4,5,6,10,0) " )
				leia(voto1)
			}
			}
			senao
			{
			se(turma==2)
			{
				escreva("(Turma 2) Informe seu voto: ")
				leia(voto2)
					
				enquanto(voto2!=1 e voto2!=2 e voto2!=3 e voto2!=4 e voto2!=5 e voto2!=6 e voto2!=10 e voto2!=0)
			{
				escreva("Informe um Voto correto (1,2,3,4,5,6,10,0) " )
				leia(voto2)
			}
				}
				senao
				{
				se(turma==3)
				{
					escreva("(Turma 3) Informe seu voto: ")
					leia(voto3)
					
				enquanto(voto3!=1 e voto3!=2 e voto3!=3 e voto3!=4 e voto3!=5 e voto3!=6 e voto3!=10 e voto3!=0)
				{
				escreva("Informe um Voto correto (1,2,3,4,5,6,10,0) " )
				leia(voto3)
			   }
			  }
			 }
			}
			escolha(voto1)
			{
				caso 1:
					ana_turma1++
					voto1=77
					eleitor++
					eleitor_valido++
					turma1++
				pare
				caso 2: 
					pedro_turma1++
					voto1=77
					eleitor++
					eleitor_valido++
					turma1++
					
				pare
				caso 3: 
					rita_turma1++
					voto1=77
					eleitor++
					eleitor_valido++
					turma1++
					
				pare
				caso 4:
					alfredo_turma1++		
					voto1=77
					eleitor++
					eleitor_valido++
					turma1++
					
				pare
				caso 5:
					regina_turma1++
					voto1=77
					eleitor++
					eleitor_valido++
					turma1++
					
				pare
				caso 6: 
					ricardo_turma1++
					voto1=77
					eleitor++
					eleitor_valido++
					turma1++
				
				pare
				caso 0:
					nulo++
					voto1=77
					voto2=77
					voto3=77
					eleitor++
				pare
				caso 10:
						
						branco++
						voto1=77
						voto2=77
						voto3=77
						eleitor++
			}
				escolha(voto2)
				{
					caso 1:
					ana_turma2++
					voto2=77
					eleitor++
					eleitor_valido++
					turma2++
				pare
				caso 2: 
					pedro_turma2++
					voto2=77
					eleitor++
					eleitor_valido++
					turma2++
				pare
				caso 3: 
					rita_turma2++
					voto2=77
					eleitor++
					eleitor_valido++
					turma2++
					pare
					caso 4:
					alfredo_turma2++
					voto3=77
					eleitor++
					eleitor_valido++
					turma2++
				pare
				caso 5:
					regina_turma2++
					voto3=77
					eleitor++
					eleitor_valido++
					turma2++
				pare
				caso 6: 
					ricardo_turma2++
					voto3=77
					eleitor++
					eleitor_valido++
					turma2++
				pare
				caso 0:
					nulo++
					voto1=77
					voto2=77
					voto3=77
					eleitor++
				pare
				caso 10:
						
						branco++
						voto1=77
						voto2=77
						voto3=77
						eleitor++
				}
				escolha(voto3)
				{
					caso 1:
					ana_turma3++
					voto3=77
					eleitor++
					eleitor_valido++
					turma3++
				pare
				caso 2: 
					pedro_turma3++
					voto3=77
					eleitor++
					eleitor_valido++
					turma3++
					
				pare
				caso 3: 
					rita_turma3++
					voto3=77
					eleitor++
					eleitor_valido++
					turma3++	
				pare
				caso 4:
					alfredo_turma3++
					voto3=77
					eleitor++
					eleitor_valido++
					turma3++
				pare
				caso 5:
					regina_turma3++
					voto3=77
					eleitor++
					eleitor_valido++
					turma3++
				pare
				caso 6: 
					ricardo_turma3++
					voto3=77
					eleitor++
					eleitor_valido++
					turma3++
				pare
				caso 0:
					nulo++
					voto1=77
					voto2=77
					voto3=77
					eleitor++
				pare
				caso 10:
						
						branco++
						voto1=77
						voto2=77
						voto3=77
						eleitor++
}}

limpa()

perc_valido=(eleitor_valido/eleitor)*100
perc_nulo=(nulo/eleitor)*100
perc_branco=(branco/eleitor)*100

perc_ana=((ana_turma1+ana_turma2+ana_turma3)/eleitor)*100
perc_pedro=((pedro_turma1+pedro_turma2+pedro_turma3)/eleitor)*100
perc_rita=((rita_turma1+rita_turma2+rita_turma3)/eleitor)*100
perc_alfredo=((alfredo_turma1+alfredo_turma2+alfredo_turma3)/eleitor)*100
perc_regina=((regina_turma1+regina_turma2+regina_turma3)/eleitor)*100
perc_ricardo=((ricardo_turma1+ricardo_turma2+ricardo_turma3)/eleitor)*100

perc_ana1=(ana_turma1/turma1)*100
perc_ana2=(ana_turma2/turma2)*100
perc_ana3=(ana_turma3/turma3)*100

perc_pedro1=(pedro_turma1/turma1)*100
perc_pedro2=(pedro_turma2/turma2)*100
perc_pedro3=(pedro_turma3/turma3)*100

perc_rita1=(rita_turma1/turma1)*100
perc_rita2=(rita_turma2/turma2)*100
perc_rita3=(rita_turma3/turma3)*100

perc_alfredo1=(alfredo_turma1/turma1)*100
perc_alfredo2=(alfredo_turma2/turma2)*100
perc_alfredo3=(alfredo_turma3/turma3)*100

perc_regina1=(regina_turma1/turma1)*100
perc_regina2=(regina_turma2/turma2)*100
perc_regina3=(regina_turma3/turma3)*100

perc_ricardo1=(ricardo_turma1/turma1)*100
perc_ricardo2=(ricardo_turma2/turma2)*100
perc_ricardo3=(ricardo_turma3/turma3)*100


escreva("Numero total de eleitores: ",eleitor,"\n")
escreva("Numero total de eleitores Validos: ",eleitor_valido,"\n")
escreva("Numero total de votos Nulos: ",nulo,"\n")
escreva("Numero total de votos Brancos: ",branco,"\n")
escreva("\n")
escreva(" % de votos Validos: ",perc_valido,"%\n")
escreva(" % de votos Nulos: ",perc_nulo,"%\n") 
escreva(" % de votos Brancos: ",perc_branco,"%\n")
escreva("\n")
escreva(" % de votos na Ana: ",perc_ana,"%\n")
escreva(" % de votos na Pedro: ",perc_pedro,"%\n")
escreva(" % de votos na Rita: ",perc_rita,"%\n")
escreva(" % de votos na Alfredo: ",perc_alfredo,"%\n")
escreva(" % de votos na Regina: ",perc_regina,"%\n")
escreva(" % de votos na Ricardo: ",perc_ricardo,"%\n")

escreva("\n")

escreva(" % de votos Turma 1 (Ana): ",perc_ana1,"%\n")
escreva(" % de votos Turma 2 (Ana): ",perc_ana2,"%\n")
escreva(" % de votos Turma 3 (Ana): ",perc_ana3,"%\n")

escreva("\n")

escreva(" % de votos Turma 1 (Pedro): ",perc_pedro1,"%\n")
escreva(" % de votos Turma 2 (Pedro): ",perc_pedro2,"%\n")
escreva(" % de votos Turma 3 (Pedro): ",perc_pedro3,"%\n")

escreva("\n")

escreva(" % de votos Turma 1 (Rita): ",perc_rita1,"%\n")
escreva(" % de votos Turma 2 (Rita): ",perc_rita2,"%\n")
escreva(" % de votos Turma 3 (Rita): ",perc_rita3,"%\n")

escreva("\n")

escreva(" % de votos Turma 1 (Alfredo): ",perc_alfredo1,"%\n")
escreva(" % de votos Turma 2 (Alfredo): ",perc_alfredo2,"%\n")
escreva(" % de votos Turma 3 (Alfredo): ",perc_alfredo3,"%\n")

escreva("\n")

escreva(" % de votos Turma 1 (Regina): ",perc_regina1,"%\n")
escreva(" % de votos Turma 2 (Regina): ",perc_regina2,"%\n")
escreva(" % de votos Turma 3 (Regina): ",perc_regina3,"%\n")

escreva("\n")

escreva(" % de votos Turma 1 (Ricardo): ",perc_ricardo1,"%\n")
escreva(" % de votos Turma 2 (Ricardo): ",perc_ricardo2,"%\n")
escreva(" % de votos Turma 3 (Ricardo): ",perc_ricardo3,"%\n")
	}
}
