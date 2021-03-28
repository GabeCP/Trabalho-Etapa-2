#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#define tam 10

int main()
{
    system("color 70");

    char NomeOs[tam][20],Status[tam][20],NomeCliente[tam][20],Bairro[tam][20],Observacao[tam][20];

    int NumeroOS[tam],CodigoServico[tam],UnidadeConsumidora[tam],Medidor[tam],Leitura[tam],Veiculo[tam],Matricula[tam],Cliente,NovoCadastro,Busca,NovaBusca,Seguir,Opcao,Sair,element;

    Sair=1;



    for(Cliente=0;Cliente<tam;Cliente++)
    {
        printf("\n\n \t >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>");
        printf("\n\n \t\t\t\t\t  SISTEMA DE ORDENS DE SERVICO ");
        printf("\n\n \t <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<");

        printf("\n\n");
        system("pause");

        printf("\n\n \t CADASTRAR NOVA ORDEM DE SERVICO: ");

        fflush(stdin);
        printf("\n\n \t INFORME O NOME DA OS: ");
        gets(NomeOs[Cliente]);
        fflush(stdin);

        printf("\n\n \t INFORME O NUMERO DA OS: ");
        scanf("%d",&NumeroOS[Cliente]);

        fflush(stdin);
        printf("\n\n \t INFORME O STATUS DA OS: ");
        gets(Status[Cliente]);
        fflush(stdin);

        do
        {
            printf("\n\n \t INFORME O CODIGO DE SERVICO: ");
            printf("\n\n \t OPCOES DISPONIVEIS: ");
            printf("\n\n \t ----------------------------------------");
            printf("\n\n \t 1");
            printf("\n\n \t 5");
            printf("\n\n \t 12");
            printf("\n\n \t 13");
            printf("\n\n \t 18");
            printf("\n\n \t 28");
            printf("\n\n \t 59");
            printf("\n\n \t 148");
            printf("\n\n \t 149");
            printf("\n\n \t 741");
            printf("\n\n \t ----------------------------------------");
            printf("\n\n \t:");
        
            scanf("%d",&CodigoServico[Cliente]);

            if((CodigoServico[Cliente]!=1)&&(CodigoServico[Cliente]!=5)&&(CodigoServico[Cliente]!=12)&&(CodigoServico[Cliente]!=13)&&(CodigoServico[Cliente]!=18)&&(CodigoServico[Cliente]!=28)&&(CodigoServico[Cliente]!=59)&&(CodigoServico[Cliente]!=148)&&(CodigoServico[Cliente]!=149)&&(CodigoServico[Cliente]!=741))
            {
                printf("\n\n\t\t\t\t    >>>>CODIGO DE SERVICO INVALIDO!<<<<");
                printf("\n\n\t\t\t\t >>>>INFORME CODIGO DE SERVICO VALIDO!<<<<\n\n");
                system("pause");
            }
        }while((CodigoServico[Cliente]!=1)&&(CodigoServico[Cliente]!=5)&&(CodigoServico[Cliente]!=12)&&(CodigoServico[Cliente]!=13)&&(CodigoServico[Cliente]!=18)&&(CodigoServico[Cliente]!=28)&&(CodigoServico[Cliente]!=59)&&(CodigoServico[Cliente]!=148)&&(CodigoServico[Cliente]!=149)&&(CodigoServico[Cliente]!=741));

        fflush(stdin);
        printf("\n\n \t INFORME O NOME DO CLIENTE: ");
        gets(NomeCliente[Cliente]);
        fflush(stdin);

        printf("\n\n \t INFORME A UNIDADE CONSUMIDORA: ");
        scanf("%d",&UnidadeConsumidora[Cliente]);

        printf("\n\n \t INFORME O MEDIDOR: ");
        scanf("%d",&Medidor[Cliente]);

        printf("\n\n \t INFORME A LEITURA: ");
        scanf("%d",&Leitura[Cliente]);

        fflush(stdin);
        printf("\n\n \t INFORME O BAIRRO DO CLIENTE: ");
        gets(Bairro[Cliente]);
        fflush(stdin);

        fflush(stdin);
        printf("\n\n \t INFORME OBSERVACOES: ");
        gets(Observacao[Cliente]);
        fflush(stdin);

        do
        {
        printf("\n\n \t INFORME O VEICULO: ");
        printf("\n\n \t OPCOES DISPONIVEIS: ");
        printf("\n\n \t ----------------------------------------");
        printf("\n\n \t 1100");
        printf("\n\n \t 1140");
        printf("\n\n \t 2230");
        printf("\n\n \t 3145");
        printf("\n\n \t 4444");
        printf("\n\n \t 4778");
        printf("\n\n \t 5160");
        printf("\n\n \t 6422");
        printf("\n\n \t 8900");
        printf("\n\n \t 9132");
        printf("\n\n \t ----------------------------------------");
        printf("\n\n \t:");
        
        scanf("%d",&Veiculo[Cliente]);

        if ((Veiculo[Cliente]!=1100)&&(Veiculo[Cliente]!=1140)&&(Veiculo[Cliente]!=2230)&&(Veiculo[Cliente]!=3145)&&(Veiculo[Cliente]!=4444)&&(Veiculo[Cliente]!=4778)&&(Veiculo[Cliente]!=5160)&&(Veiculo[Cliente]!=6422)&&(Veiculo[Cliente]!=8900)&&(Veiculo[Cliente]!=9132))
        {
            printf("\n\n\t\t\t\t    >>>>NUMERO DE VEICULO INVALIDO!<<<<");
            printf("\n\n\t\t\t\t >>>>INFORME NUMERO DE VEICULO VALIDO!<<<<\n\n");
            system("pause");
        }
        } while ((Veiculo[Cliente]!=1100)&&(Veiculo[Cliente]!=1140)&&(Veiculo[Cliente]!=2230)&&(Veiculo[Cliente]!=3145)&&(Veiculo[Cliente]!=4444)&&(Veiculo[Cliente]!=4778)&&(Veiculo[Cliente]!=5160)&&(Veiculo[Cliente]!=6422)&&(Veiculo[Cliente]!=8900)&&(Veiculo[Cliente]!=9132));

        do
        {
            printf("\n\n \t INFORME A MATRICULA: ");
            printf("\n\n \t OPCOES DISPONIVEIS: ");
            printf("\n\n \t ----------------------------------------");
            printf("\n\n \t 37092");
            printf("\n\n \t 30192");
            printf("\n\n \t 30465");
            printf("\n\n \t 36789");
            printf("\n\n \t 35015");
            printf("\n\n \t 36487");
            printf("\n\n \t 34850");
            printf("\n\n \t 36065");
            printf("\n\n \t 36519");
            printf("\n\n \t 31184");
            printf("\n\n \t ----------------------------------------");
            printf("\n\n \t:");
        
            scanf("%d",&Matricula[Cliente]);

            if((Matricula[Cliente]!=37092)&&(Matricula[Cliente]!=30192)&&(Matricula[Cliente]!=30465)&&(Matricula[Cliente]!=36789)&&(Matricula[Cliente]!=35015)&&(Matricula[Cliente]!=36487)&&(Matricula[Cliente]!=34850)&&(Matricula[Cliente]!=36065)&&(Matricula[Cliente]!=35619)&&(Matricula[Cliente]!=31184))
            {
                printf("\n\n\t\t\t\t    >>>>MATRICULA INVALIDA!<<<<");
                printf("\n\n\t\t\t\t >>>>INFORME MATRICULA VALIDA!<<<<\n\n");
                system("pause");
            }
        }while((Matricula[Cliente]!=37092)&&(Matricula[Cliente]!=30192)&&(Matricula[Cliente]!=30465)&&(Matricula[Cliente]!=36789)&&(Matricula[Cliente]!=35015)&&(Matricula[Cliente]!=36487)&&(Matricula[Cliente]!=34850)&&(Matricula[Cliente]!=36065)&&(Matricula[Cliente]!=35619)&&(Matricula[Cliente]!=31184));

        printf("\n\n \t DESEJA REALIZAR NOVO CADASTRO? (SIM-DIGITE 1 / NAO-DIGITE 0 ): ");
        scanf("%d",&NovoCadastro);
        printf("%d",NovoCadastro);

        if(NovoCadastro==0)
           Cliente=tam;

           system("cls");

    }

    do
    {

    printf("\n\n \t >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>");
    printf("\n\n \t\t\t\t\t\t\t  MENU ");
    printf("\n\n \t\t\t\t\t DIGITE O NUMERO CORRESPONDENTE A ACAO ");
    printf("\n\n \t <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<");

    printf("\n\n \t  0 - SAIR ");
    printf("\n\n \t  1 - PESQUISAR ORDEM DE SERVICO ");
    printf("\n\n \t  2 - EDITAR ORDEM DE SERVICO \n");
    printf("\n\n \t  OPCAO: ");
    scanf("%d",&Opcao);

    switch (Opcao)

    {
    case 0:
    {
        Sair=0;
    }
    break;
    case 1:
        {
           printf("\n\n \t  DIGITE O NUMERO DA OS QUE DESEJA BUSCAR INFORMACOES DE CADASTRO: ");
            scanf("%d",&Busca);

            for(Cliente=0;Cliente<tam;Cliente++)
        {
            NumeroOS[Cliente];
            if (NumeroOS[Cliente]==Busca)
            {
                Busca=Cliente;
                Cliente=tam;
            }
        }
            printf("\n\n \t NOME DA OS: %s ",NomeOs[Busca]);

            printf("\n\n \t NUMERO DA OS: %d ",NumeroOS[Busca]);

            printf("\n\n \t STATUS: %s ",Status[Busca]);

            printf("\n\n \t CODIGO DE SERVICO: %d ",CodigoServico[Busca]);

            printf("\n\n \t NOME DO CLIENTE: %s ",NomeCliente[Busca]);

            printf("\n\n \t UC: %d ",UnidadeConsumidora[Busca]);

            printf("\n\n \t MEDIDOR: %d ",Medidor[Busca]);

            printf("\n\n \t LEITURA: %d ",Leitura[Busca]);

            printf("\n\n \t BAIRRO: %s ",Bairro[Busca]);

            printf("\n\n \t OBSERVACAO: %s ",Observacao[Busca]);

            printf("\n\n \t VEICULO: %d ",Veiculo[Busca]);

            printf("\n\n \t MATRICULA: %d ",Matricula[Busca]);



    break;
    }

    case 2:
        {
        printf("\n\n \t  DIGITE O NUMERO DA OS QUE DESEJA ALTERAR AS INFORMACOES DE CADASTRO: ");
        scanf("%d",&Busca);

        for(Cliente=0;Cliente<tam;Cliente++)
        {
            NumeroOS[Cliente];
            if(NumeroOS[Cliente]==Busca)
            {
                Busca=Cliente;
                Cliente=tam;
            }
        }

        printf("\n\n \t  INFORME O NUMERO DO ELEMENTO QUE DESEJA ALTERAR\n\n \t(1) - NOME DA OS\n\n \t(2) - NUMERO OS\n\n \t(3) - STATUS\n\n \t(4) - CODIGO SERVICO\n\n \t(5) - NOME CLIENTE\n\n \t(6) - UNIDADE CONSUMIDORA\n\n \t(7) - MEDIDOR\n\n \t(8) - LEITURA\n\n \t(9) - BAIRRO\n\n \t(10) - OBSERVACAO\n\n \t(11) - VEICULO\n\n \t(12) - MATRICULA\n\n");
        printf("\n\n \t  OPCAO: ");
        scanf("%d",&element);
        switch(element)

        {

        case 1:
            {
                fflush(stdin);
                printf("\n\n \t INFORME SEU NOME DA OS: ");
                gets(NomeOs[Busca]);
                fflush(stdin);
            }
            break;

        case 2:
            {
                printf("\n\n \t INFORME O NUMERO DA OS: ");
                scanf("%d",&NumeroOS[Busca]);
            }
            break;

        case 3:
            {
                fflush(stdin);
                printf("\n\n \t INFORME SEU STATUS DA OS: ");
                gets(Status[Busca]);
                fflush(stdin);
            }
            break;

        case 4:
            {
                do
        {
            printf("\n\n \t INFORME O CODIGO DE SERVICO: ");
            printf("\n\n \t OPCOES DISPONIVEIS: ");
            printf("\n\n \t ----------------------------------------");
            printf("\n\n \t 1");
            printf("\n\n \t 5");
            printf("\n\n \t 12");
            printf("\n\n \t 13");
            printf("\n\n \t 18");
            printf("\n\n \t 28");
            printf("\n\n \t 59");
            printf("\n\n \t 148");
            printf("\n\n \t 149");
            printf("\n\n \t 741");
            printf("\n\n \t ----------------------------------------");
            printf("\n\n \t:");
            scanf("%d",&CodigoServico[Busca]);

            if((CodigoServico[Busca]!=1)&&(CodigoServico[Busca]!=5)&&(CodigoServico[Busca]!=12)&&(CodigoServico[Busca]!=13)&&(CodigoServico[Busca]!=18)&&(CodigoServico[Busca]!=28)&&(CodigoServico[Busca]!=59)&&(CodigoServico[Busca]!=148)&&(CodigoServico[Busca]!=149)&&(CodigoServico[Busca]!=741))
            {
                printf("\n\n\t\t\t\t    >>>>CODIGO DE SERVICO INVALIDO!<<<<");
                printf("\n\n\t\t\t\t >>>>INFORME CODIGO DE SERVICO VALIDO!<<<<\n\n");
                system("pause");
            }
        }while((CodigoServico[Busca]!=1)&&(CodigoServico[Busca]!=5)&&(CodigoServico[Busca]!=12)&&(CodigoServico[Busca]!=13)&&(CodigoServico[Busca]!=18)&&(CodigoServico[Busca]!=28)&&(CodigoServico[Busca]!=59)&&(CodigoServico[Busca]!=148)&&(CodigoServico[Busca]!=149)&&(CodigoServico[Busca]!=741));
            }
            break;

        case 5:
            {
                fflush(stdin);
                printf("\n\n \t INFORME SEU NOME DO CLIENTE: ");
                gets(NomeCliente[Busca]);
                fflush(stdin);
            }
            break;

        case 6:
            {
                printf("\n\n \t INFORME A UNIDADE CONSUMIDORA: ");
                scanf("%d",&UnidadeConsumidora[Busca]);
            }
            break;

        case 7:
            {
                printf("\n\n \t INFORME O MEDIDOR: ");
                scanf("%d",&Medidor[Busca]);
            }
            break;

        case 8:
            {
                printf("\n\n \t INFORME A LEITURA: ");
                scanf("%d",&Leitura[Busca]);
            }
            break;

        case 9:
            {
                fflush(stdin);
                printf("\n\n \t INFORME SEU BAIRRO DO CLIENTE: ");
                gets(Bairro[Busca]);
                fflush(stdin);
            }
            break;

        case 10:
            {
                fflush(stdin);
                printf("\n\n \t INFORME OBSERVACOES: ");
                gets(Observacao[Busca]);
                fflush(stdin);
            }
            break;

        case 11:
            {
                do
        {
        printf("\n\n \t INFORME O VEICULO: ");
        printf("\n\n \t OPCOES DISPONIVEIS: ");
        printf("\n\n \t ----------------------------------------");
        printf("\n\n \t 1100");
        printf("\n\n \t 1140");
        printf("\n\n \t 2230");
        printf("\n\n \t 3145");
        printf("\n\n \t 4444");
        printf("\n\n \t 4778");
        printf("\n\n \t 5160");
        printf("\n\n \t 6422");
        printf("\n\n \t 8900");
        printf("\n\n \t 9132");
        printf("\n\n \t ----------------------------------------");
        printf("\n\n \t:");
        
        scanf("%d",&Veiculo[Busca]);

        if ((Veiculo[Busca]!=1100)&&(Veiculo[Busca]!=1140)&&(Veiculo[Busca]!=2230)&&(Veiculo[Busca]!=3145)&&(Veiculo[Busca]!=4444)&&(Veiculo[Busca]!=4778)&&(Veiculo[Busca]!=5160)&&(Veiculo[Busca]!=6422)&&(Veiculo[Busca]!=8900)&&(Veiculo[Busca]!=9132))
        {
            printf("\n\n\t\t\t\t    >>>>NUMERO DE VEICULO INVALIDO!<<<<");
            printf("\n\n\t\t\t\t >>>>INFORME NUMERO DE VEICULO VALIDO!<<<<\n\n");
            system("pause");
        }
        } while ((Veiculo[Busca]!=1100)&&(Veiculo[Busca]!=1140)&&(Veiculo[Busca]!=2230)&&(Veiculo[Busca]!=3145)&&(Veiculo[Busca]!=4444)&&(Veiculo[Busca]!=4778)&&(Veiculo[Busca]!=5160)&&(Veiculo[Busca]!=6422)&&(Veiculo[Busca]!=8900)&&(Veiculo[Busca]!=9132));
            }
            break;

        case 12:
            {
                do
        {
            printf("\n\n \t INFORME A MATRICULA: ");
            printf("\n\n \t OPCOES DISPONIVEIS: ");
            printf("\n\n \t ----------------------------------------");
            printf("\n\n \t 37092");
            printf("\n\n \t 30192");
            printf("\n\n \t 30465");
            printf("\n\n \t 36789");
            printf("\n\n \t 35015");
            printf("\n\n \t 36487");
            printf("\n\n \t 34850");
            printf("\n\n \t 36065");
            printf("\n\n \t 36519");
            printf("\n\n \t 31184");
            printf("\n\n \t ----------------------------------------");
            printf("\n\n \t:");
            scanf("%d",&Matricula[Busca]);

            if((Matricula[Busca]!=37092)&&(Matricula[Busca]!=30192)&&(Matricula[Busca]!=30465)&&(Matricula[Busca]!=36789)&&(Matricula[Busca]!=35015)&&(Matricula[Busca]!=36487)&&(Matricula[Busca]!=34850)&&(Matricula[Busca]!=36065)&&(Matricula[Busca]!=35619)&&(Matricula[Busca]!=31184))
            {
                printf("\n\n\t\t\t\t    >>>>MATRICULA INVALIDA!<<<<");
                printf("\n\n\t\t\t\t >>>>INFORME MATRICULA VALIDA!<<<<\n\n");
                system("pause");
            }
        }while((Matricula[Busca]!=37092)&&(Matricula[Busca]!=30192)&&(Matricula[Busca]!=30465)&&(Matricula[Busca]!=36789)&&(Matricula[Busca]!=35015)&&(Matricula[Busca]!=36487)&&(Matricula[Busca]!=34850)&&(Matricula[Busca]!=36065)&&(Matricula[Busca]!=35619)&&(Matricula[Busca]!=31184));
            }
            break;

        default:
            {
                printf("\n\n\t\t\t\t    >>>>OPCAO INVALIDA!<<<<");
                printf("\n\n\t\t\t\t >>>>INFORME OPCAO VALIDA!<<<<\n\n");
                system("pause");
            }
            break;
            }
        }
           break;

           default: {
           printf("\n\n\t\t\t\t    >>>>OPCAO INVALIDA!<<<<");
           printf("\n\n\t\t\t\t >>>>INFORME OPCAO VALIDA!<<<<\n\n");
           }
    }
            do
            {
            printf("\n\n \t DIGITE 1 PARA VOLTAR PARA O MENU OU 0 PARA SAIR: ");
            scanf("%d",&Sair);
            system("cls");
            if ((Sair!=1 && Sair!=0))
            {
                printf("\n\n \t OPCAO INVALIDA");
                printf("\n\n \t INFORME UMA OPCAO INVALIDA \n");
                system("pause");
            }

    } while ((Sair!=1 && Sair!=0));

} while (Sair!=0);

return 0;

}
