# dezAlgoritmosC
Em uma lista de exercício, foram elaborados 10 algoritmos utilizando linguagem C



1 - 

#include <stdio.h>
#include <stdio.h>

int main()
{
    float na = 0;
    float nb = 0;
    float nc = 0;
    float nab = 0;
    
    printf("Indique o valor de A: \n");
    scanf("%f", &na);
    printf("Indique o valor de B: \n");
    scanf("%f", &nb);
    printf("Indique o valor de C: \n");
    scanf("%f", &nc);
    
    nab = na + nb;
    
    if(nab<nc){
        printf("A soma de A + B é: %0.2f", nab);
    }

    return 0;
}

2 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    int n1 = 0;
    
    printf("Indique o número: ");
    scanf("%d", &n1);

    if(n1%2 == 0){
        printf("Seu número é PAR!");
    }else{
        printf("Seu número é ÍMPAR!");
    }

    return 0;
}

3 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    int va = 0;
    int vb = 0;
    int vc = 0;
    
    printf("Indique o primeiro número: ");
    scanf("%d", &va);
    printf("Indique o segundo número: ");
    scanf("%d", &vb);

    if(va == vb){
        
        vc = va + vb;
        printf("Seu resultado é: %d", vc);
    }else{
        
        vc = va * vb;
        printf("Seu resultado é: %d", vc);
    }

    return 0;
}

4 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    int n = 0;
    int dobroNumero = 0;
    int triploNumero = 0;
    
    printf("Indique o número: ");
    scanf("%d", &n);

    if(n > 0){
        
        dobroNumero = n * 2;
        printf("Seu resultado é: %d", dobroNumero);
    }else if(n < 0){
        
        triploNumero = n * 3;
        printf("Seu resultado é: %d", triploNumero);
    }else{
        printf("Seu número é: %d", n);
    }

    return 0;
}

5 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    int n = 0;
    int nPar = 0;
    int nImpar = 0;
    
    printf("Indique o número: ");
    scanf("%d", &n);

    if(n%2 == 0){
        
        nPar = n + 5;
        printf("Seu resultado é: %d", nPar);
    }else{
        
        nImpar = n + 8;
        printf("Seu resultado é: %d", nImpar);
    }

    return 0;
}

6 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    int n1 = 0;
    int n2 = 0;
    int n3 = 0;
    
    printf("Indique o primeiro número: ");
    scanf("%d", &n1);
    printf("Indique o segundo número: ");
    scanf("%d", &n2);
    printf("Indique o terceiro número: ");
    scanf("%d", &n3);

    if(n1>n2 && n1>n3 &&n2>n3){
        
        printf("Seus números em ordem decrescente são: %d, %d, %d", n1, n2, n3);
        
    }else if(n2>n3 && n2>n1 && n3>n1){
        
        printf("Seus números em ordem decrescente são: %d, %d, %d", n2, n3, n1);
    }else if(n3>n1 && n3>n2 && n1>n2){
        
        printf("Seus números em ordem decrescente são: %d, %d, %d", n3, n1, n2);
    }else if(n2>n1 && n2>n3 && n1>n3){
        
        printf("Seus números em ordem decrescente são: %d, %d, %d", n2, n1, n3);
    }else if(n3>n1 && n3>n2 && n1>n2){
        
        printf("Seus números em ordem decrescente são: %d, %d, %d", n3, n1, n2);
    }else if(n1>n3 && n1>n2 && n3>n2){
        
        printf("Seus números em ordem decrescente são: %d, %d, %d", n1, n3, n2);
    
    }else if(n3>n2 && n3>n1 && n2>n1){
        
        printf("Seus números em ordem decrescente são: %d, %d, %d", n3, n2, n1);
    }else{
        printf("Opção inválida, alguns números são iguais.");
    }
    
    return 0;
}

7 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    int sexo = 0;
    int h = 0;
    float peso = 0;

    printf("PESO IDEAL!\n");
    printf("Indique o sexo (1 - Masculino e 0 - Feminino): ");
    scanf("%d", &sexo);
    printf("Indique a altura: ");
    scanf("%d", &h);

    if(sexo == 1){
        
        peso = (72.7 * h) - 58;
        printf("O peso ideal é = %0.2f", peso);
        
    }else if(peso == 0){
        
        peso = (62.1 * h) - 44.7;
        printf("O peso ideal é = %0.2f", peso);
    }else{
        
        printf("Valores inválidos!");
    }
    
    return 0;
}

8 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    float imc = 0;
    float h = 0;
    float peso = 0;

    printf("Cálculo IMC!\n");
    printf("Indique o peso: ");
    scanf("%f", &peso);
    printf("Indique a altura: ");
    scanf("%f", &h);
    
    imc = peso/(h*h);

    if(imc<18.5){
        
        printf("IMC = %0.2f - Abaixo do peso.", imc);
        
    }if (imc>=18.5 && imc<=25){
        
        printf("IMC = %0.2f - Peso normal.", imc);
        
    }if (imc>=25 && imc<=30){
        
        printf("IMC = %0.2f - Acima do peso.", imc);
        
    }else if(imc>30){
        
        printf("IMC = %0.2f - Obeso.", imc);
        
    }else{
        
    }
    
    return 0;
}

9 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    float produto = 0;
    int escolha = 0;
    float parcela = 0;

    printf("Indique o valor do produto: ");
    scanf("%f", &produto);
    printf("1- À vista em dinheiro ou cheque. \n");
    printf("2- À vista no cartão de crédito. \n");
    printf("3- Em duas vezes. \n");
    printf("4- Em três vezes. \n");
    printf("Indique a forma de pagamento: \n");
    scanf("%d", &escolha);
    
    switch (escolha){
        case 1:{
        
            produto = produto * 0.9;
            printf("Valor final: R$%0.2f", produto);
            break;
        }    
        case 2:{
        
            produto = produto * 0.85;
            printf("Valor final: R$%0.2f", produto);
            break;
        }
        case 3:{
        
            parcela = produto/2;
            printf("Valor final: 2x de R$%0.2f", parcela);
            break;
        }
        case 4:{
        
            parcela = (produto/3) + (produto*0.1);
            printf("Valor final: 3x de R$%0.2f", parcela);
            break;
        }
        default:{
            
            printf("Opção inválida!");
            break;
        }
    }
    
    return 0;
}

10 -

#include <stdio.h>
#include <stdio.h>

int main()
{
    int i = 0;
    float n1, n2, n3, mE, mA;

    printf("Indique o número de identificação do aluno: ");
    scanf("%d", &i);
    printf("\nDigite a primeira nota: ");
    scanf("%f", &n1);
    printf("\nDigite a segunda nota: ");
    scanf("%f", &n2);
    printf("\nDigite a terceira nota: ");
    scanf("%f", &n3);
    printf("\nDigite a média dos exercícios: ");
    scanf("%f", &mE);
    
    mA = (n1 + n2*2 + n3*3 + mE)/7;
    
    printf("Dados do Aluno: ");
    printf("\nIdentificação do aluno: %d", i);
    printf("\nPrimeira nota: %0.2f", n1);
    printf("\nSegunda nota: %0.2f", n2);
    printf("\nTerceira nota: %0.2f", n3);
    printf("\nMédia de exercícios: %0.2f", mE);
    printf("\nMédia de aproveitamento: %0.2f", mA);
    
    if (mA>=90){
        printf("\nConceito A.");
        printf("\nAprovado!");
    }if (mA>=75 && mA<90){
        printf("\nConceito B.");
        printf("\nAprovado!");
    }if (mA>=60 && mA<75){
        printf("\nConceito C.");
        printf("\nAprovado!");
    }if (mA>=40 && mA<60){
        printf("\nConceito D.");
        printf("\nReprovado!");
    }else if(mA<40){
        printf("\nConceito E.");
        printf("\nReprovado!");
    }else{
        
    }
    
    return 0;
}
