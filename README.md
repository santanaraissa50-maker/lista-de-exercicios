RSDS - 14.c

#include <stdio.h>

int main() {
    int a, b, c;

    printf("Tipo de Triangulo\n");
    printf("Digite os 3 lados: ");
    scanf("%d %d %d", &a, &b, &c);

    if (a == b && b == c) {
        printf("Triangulo Equilatero\n");
    } else if (a == b || a == c || b == c) {
        printf("Triangulo Isosceles\n");
    } else {
        printf("Triangulo Escaleno\n");
    }

    return 0;
}

RSDS - 15.c

 #include <stdio.h>

int main() {
    int altC, largC, compC;
    int altCx, largCx, compCx;
    int total;

    printf("Caixas no Caminhao\n");

    printf("Digite altura, largura e comprimento do caminhao: ");
    scanf("%d %d %d", &altC, &largC, &compC);

    printf("Digite altura, largura e comprimento da caixa: ");
    scanf("%d %d %d", &altCx, &largCx, &compCx);

    total = (altC / altCx) * (largC / largCx) * (compC / compCx);

    printf("Quantidade de caixas: %d\n", total);

    return 0;
}

RSDS -16.c

#include <stdio.h>

int main() {
    int pedido;

    printf("Multiplo de 3 e/ou 5\n");
    printf("Digite o numero do pedido: ");
    scanf("%d", &pedido);

    if (pedido % 3 == 0 && pedido % 5 == 0) {
        printf("Ganhou refrigerante e sobremesa\n");
    } else if (pedido % 3 == 0) {
        printf("Ganhou refrigerante\n");
    } else if (pedido % 5 == 0) {
        printf("Ganhou sobremesa\n");
    } else {
        printf("Nao ganhou brindes\n");
    }

    return 0;
}

RSDS - 17.c

  #include <stdio.h>

int main() {
    int altura;

    printf("Sensor do Parque\n");
    printf("Digite a altura em cm: ");
    scanf("%d", &altura);

    if (altura >= 140) {
        printf("Liberado\n");
    } else {
        printf("Barrado\n");
    }

    return 0;
}

RSDS -18.c

#include <stdio.h>
#include <string.h>

int main() {
    char usuario[20], senha[20];

    printf("Login Simples\n");

    printf("Usuario: ");
    scanf("%s", usuario);

    printf("Senha: ");
    scanf("%s", senha);

    if (strcmp(usuario, "admin") == 0 &&
        strcmp(senha, "1234") == 0) {
        printf("Acesso permitido\n");
    } else {
        printf("Acesso negado\n");
    }

    return 0;
}


RSDS - 19.c

#include <stdio.h>

int main() {
    int n1, n2, n3, temp;

    printf("Ordem Crescente\n");
    printf("Digite 3 numeros: ");
    scanf("%d %d %d", &n1, &n2, &n3);

    if (n1 > n2) {
        temp = n1;
        n1 = n2;
        n2 = temp;
    }

    if (n1 > n3) {
        temp = n1;
        n1 = n3;
        n3 = temp;
    }

    if (n2 > n3) {
        temp = n2;
        n2 = n3;
        n3 = temp;
    }

    printf("Ordem crescente: %d %d %d\n", n1, n2, n3);

    return 0;
}


RSDS - 20.c

#include <stdio.h>

int main() {
    int ano;

    printf("Ano Bissexto\n");
    printf("Digite um ano: ");
    scanf("%d", &ano);

    if ((ano % 4 == 0 && ano % 100 != 0) || (ano % 400 == 0))
        printf("Ano bissexto\n");
    else
        printf("Nao e bissexto\n");

    return 0;
}


RSDS - 21.c

#include <stdio.h>

int main() {
    int valor;

    printf("Positivo ou Negativo\n");
    printf("Digite um numero: ");
    scanf("%d", &valor);

    if (valor > 0)
        printf("Positivo\n");
    else if (valor < 0)
        printf("Negativo\n");
    else
        printf("Zero\n");

    return 0;
}

RSDS -22.c

#include <stdio.h>

int main() {
    int numero;

    printf("Par ou Impar\n");
    printf("Digite um numero: ");
    scanf("%d", &numero);

    if (numero % 2 == 0)
        printf("Par\n");
    else
        printf("Impar\n");

    return 0;
}


RSDS -23.c

#include <stdio.h>

int main() {
    int x, y;

    printf("Maior de Dois Numeros\n");
    printf("Digite dois numeros: ");
    scanf("%d %d", &x, &y);

    if (x > y)
        printf("Maior: %d\n", x);
    else
        printf("Maior: %d\n", y);

    return 0;
}

RSDS -24.c

#include <stdio.h>

int main() {
    int idade;

    printf("Pode Votar?\n");
    printf("Digite a idade: ");
    scanf("%d", &idade);

    if (idade >= 16)
        printf("Pode votar\n");
    else
        printf("Nao pode votar\n");

    return 0;
}

RSDS - 25.c


#include <stdio.h>

int main() {
    float media;

    printf("Notas e Aprovacao\n");
    printf("Digite a media: ");
    scanf("%f", &media);

    if (media >= 7)
        printf("Aprovado\n");
    else if (media >= 5)
        printf("Recuperacao\n");
    else
        printf("Reprovado\n");

    return 0;
}

 RSDS -26.c

#include <stdio.h>

int main() {
    int i;

    printf("Contar de 1 a 10\n");

    for(i = 1; i <= 10; i++) {
        printf("%d\n", i);
    }

    return 0;
}

RSDS-27.c

#include <stdio.h>

int main() {
    int num, i;

    printf("Tabuada\n");
    printf("Digite um numero: ");
    scanf("%d", &num);

    for(i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", num, i, num * i);
    }

    return 0;
}


RSDS-28.c

#include <stdio.h>

int main() {
    int i, soma = 0;

    printf("Soma de 1 a 100\n");

    for(i = 1; i <= 100; i++) {
        soma += i;
    }

    printf("Soma = %d\n", soma);

    return 0;
}


RSDS-29.c


#include <stdio.h>

int main() {
    int i;

    printf("Numeros Pares de 0 a 50\n");

    for(i = 0; i <= 50; i++) {
        if(i % 2 == 0) {
            printf("%d\n", i);
        }
    }

    return 0;
}


RSDS-30.c

#include <stdio.h>

int main() {
    int n, i, fatorial = 1;

    printf("Fatorial\n");
    printf("Digite um numero: ");
    scanf("%d", &n);

    for(i = 1; i <= n; i++) {
        fatorial *= i;
    }

    printf("Fatorial = %d\n", fatorial);

    return 0;
}

RSDS-31.c

#include <stdio.h>

int main() {
    int i;

    printf("Contagem Regressiva\n");

    for(i = 10; i >= 1; i--) {
        printf("%d\n", i);
    }

    return 0;
}


RSDS-32.c

#include <stdio.h>

int main() {
    int i;

    printf("Quadrado de 1 a 10\n");

    for(i = 1; i <= 10; i++) {
        printf("%d² = %d\n", i, i * i);
    }

    return 0;
}


RSDS-33.c

#include <stdio.h>

int main() {
    int i;

    printf("Multiplos de 3\n");

    for(i = 1; i <= 30; i++) {
        if(i % 3 == 0) {
            printf("%d\n", i);
        }
    }

    return 0;
}


RSDS-34.c

#include <stdio.h>

int main() {
    int primo, i, divisores = 0;

    printf("Numero Primo\n");
    printf("Digite um numero: ");
    scanf("%d", &primo);

    for(i = 1; i <= primo; i++) {
        if(primo % i == 0) {
            divisores++;
        }
    }

    if(divisores == 2)
        printf("Numero primo\n");
    else
        printf("Nao e primo\n");

    return 0;
}


RSDS-35.c

#include <stdio.h>

int main() {
    int termos, a = 0, b = 1, prox, i;

    printf("Fibonacci\n");
    printf("Digite a quantidade de termos: ");
    scanf("%d", &termos);

    for(i = 1; i <= termos; i++) {
        printf("%d ", a);
        prox = a + b;
        a = b;
        b = prox;
    }

    printf("\n");

    return 0;
}


RSDS-36.c

#include <stdio.h>

int main() {
    int cont = 1;

    printf("Contar ate 10 com while\n");

    while (cont <= 10) {
        printf("%d\n", cont);
        cont++;
    }

    return 0;
}

RSDS-37.c

#include <stdio.h>

int main() {
    int valor, total = 0;

    printf("Soma ate digitar 0\n");

    while (1) {
        printf("Digite um numero: ");
        scanf("%d", &valor);

        if (valor == 0)
            break;

        total += valor;
    }

    printf("Soma total = %d\n", total);

    return 0;
}


RSDS-38.c

#include <stdio.h>

int main() {
    int senha = 0;

    printf("Senha Correta\n");

    while (senha != 1234) {
        printf("Digite a senha: ");
        scanf("%d", &senha);
    }

    printf("Acesso liberado\n");

    return 0;
}


RSDS-39.c

#include <stdio.h>

int main() {
    int positivo = -1;

    printf("Numero Positivo\n");

    while (positivo <= 0) {
        printf("Digite um numero positivo: ");
        scanf("%d", &positivo);
    }

    printf("Numero aceito\n");

    return 0;
}


RSDS-40.c

#include <stdio.h>

int main() {
    int tabuada, j = 1;

    printf("Tabuada com while\n");
    printf("Digite um numero: ");
    scanf("%d", &tabuada);

    while (j <= 10) {
        printf("%d x %d = %d\n", tabuada, j, tabuada * j);
        j++;
    }

    return 0;
}


RSDS-41.c

#include <stdio.h>

int main() {
    int numero, div = 1, qtd = 0;

    printf("Primo com while\n");
    printf("Digite um numero: ");
    scanf("%d", &numero);

    while (div <= numero) {
        if (numero % div == 0)
            qtd++;

        div++;
    }

    if (qtd == 2)
        printf("Numero primo\n");
    else
        printf("Nao e primo\n");

    return 0;
}


RSDS-42.c


#include <stdio.h>

int main() {
    int i, impar = 0, numDigitado;

    printf("Quantidade de Impares\n");

    for (i = 1; i <= 10; i++) {
        printf("Digite um numero: ");
        scanf("%d", &numDigitado);

        if (numDigitado % 2 != 0)
            impar++;
    }

    printf("Quantidade de impares = %d\n", impar);

    return 0;
}


RSDS-43.c

#include <stdio.h>

int main() {
    int i = 1;
    int somaPares = 0;

    printf("Soma dos Pares\n");

    while (i <= 100) {
        if (i % 2 == 0) {
            somaPares += i;
        }
        i++;
    }

    printf("Soma = %d\n", somaPares);

    return 0;
}

RSDS-44.c

#include <stdio.h>

int main() {
    int digitos = 0, numeroDigitado;

    printf("Contar Digitos\n");
    printf("Digite um numero positivo: ");
    scanf("%d", &numeroDigitado);

    while (numeroDigitado > 0) {
        numeroDigitado /= 10;
        digitos++;
    }

    printf("Quantidade de digitos = %d\n", digitos);

    return 0;
}


RSDS-45.c

#include <stdio.h>

int main() {
    int opcao = 0;

    printf("Menu\n");

    while (opcao != 3) {
        printf("\n1 - Sacar\n");
        printf("2 - Depositar\n");
        printf("3 - Sair\n");
        printf("Escolha: ");
        scanf("%d", &opcao);
    }

    return 0;
}

RSDS-46.c

#include <stdio.h>

int main() {
    int i = 1;

    printf("Contar de 1 a 10\n");

    do {
        printf("%d\n", i);
        i++;
    } while (i <= 10);

    return 0;
}


RSDS-47.c

#include <stdio.h>

int main() {
    int numeroTabuada;
    int i = 1;

    printf("Tabuada com do while\n");
    printf("Digite um numero: ");
    scanf("%d", &numeroTabuada);

    do {
        printf("%d x %d = %d\n", numeroTabuada, i, numeroTabuada * i);
        i++;
    } while (i <= 10);

    return 0;
}


RSDS-48.c

#include <stdio.h>

int main() {
    int menu;

    printf("Menu com Sair\n");

    do {
        printf("\n1 - Mensagem\n");
        printf("2 - Sair\n");
        printf("Escolha: ");
        scanf("%d", &menu);

        if (menu == 1) {
            printf("Voce escolheu a mensagem!\n");
        }

    } while (menu != 2);

    return 0;
}


RSDS-49.c

#include <stdio.h>

int main() {
    int senhaLab;

    printf("Senha Laboratorio\n");

    do {
        printf("Digite a senha: ");
        scanf("%d", &senhaLab);
    } while (senhaLab != 1111);

    printf("Acesso liberado!\n");

    return 0;
}


RSDS-50.c

#include <stdio.h>

int main() {
    int deposito;

    printf("Numero Positivo Obrigatorio\n");

    do {
        printf("Digite um numero positivo: ");
        scanf("%d", &deposito);
    } while (deposito <= 0);

    printf("Valor aceito\n");

    return 0;
}


RSDS-51.c

#include <stdio.h>

int main() {
    int i = 10;

    printf("Contagem Regressiva\n");

    do {
        printf("%d\n", i);
        i--;
    } while (i >= 1);

    return 0;
}


RSDS-52.c

#include <stdio.h>

int main() {
    int numeroSoma, somaTotal = 0;

    printf("Soma ate multiplo de 10\n");

    do {
        printf("Digite um numero: ");
        scanf("%d", &numeroSoma);
        somaTotal += numeroSoma;
    } while (numeroSoma % 10 != 0);

    printf("Soma total = %d\n", somaTotal);

    return 0;
}


RSDS-53.c

#include <stdio.h>

int main() {
    char sair;

    printf("Confirmar Saida\n");

    do {
        printf("Menu executado\n");
        printf("Deseja sair? (s/n): ");
        scanf(" %c", &sair);
    } while (sair != 's');

    return 0;
}


RSDS-54.c

#include <stdio.h>

int main() {
    int nivel;

    printf("Validar Numero\n");

    do {
        printf("Digite um numero entre 1 e 5: ");
        scanf("%d", &nivel);
    } while (nivel < 1 || nivel > 5);

    printf("Nivel valido\n");

    return 0;
}


RSDS-55.c

#include <stdio.h>

int main() {
    int maior = 0, numeroMaior;

    printf("Mostrar Maior Numero\n");

    do {
        printf("Digite um numero: ");
        scanf("%d", &numeroMaior);

        if (numeroMaior > maior)
            maior = numeroMaior;

    } while (numeroMaior >= 0);

    printf("Maior numero digitado = %d\n", maior);

    return 0;
}


RSDS-56.c

#include <stdio.h>

int main() {
    int combo;

    printf("Fast Food\n");
    printf("Escolha um combo (1 a 4): ");
    scanf("%d", &combo);

    switch (combo) {
        case 1:
            printf("Combo Hamburguer + Batata + Refri - R$ 30,00\n");
            break;
        case 2:
            printf("Combo Pizza Brotinho + Refri - R$ 25,00\n");
            break;
        case 3:
            printf("Combo Salada + Suco Natural - R$ 22,00\n");
            break;
        case 4:
            printf("Combo Balde de Frango + Molho - R$ 35,00\n");
            break;
        default:
            printf("Opcao invalida!\n");
    }

    return 0;
}


RSDS-57.c

#include <stdio.h>
#include <string.h>

int main() {
    char cor[20];

    printf("Urso Eletronico\n");
    printf("Digite uma cor: ");
    scanf("%s", cor);

    if (strcmp(cor, "Verde") == 0)
        printf("Vamos brincar la fora!\n");
    else if (strcmp(cor, "Amarelo") == 0)
        printf("Estou ficando com soninho...\n");
    else if (strcmp(cor, "Vermelho") == 0)
        printf("Estou com fome, hora do lanche!\n");
    else
        printf("Cor desconhecida\n");

    return 0;
}


RSDS-58.c

#include <stdio.h>

int main() {
    float num1, num2, resultado;
    char operador;

    printf("Calculadora\n");

    printf("Digite dois numeros: ");
    scanf("%f %f", &num1, &num2);

    printf("Digite a operacao (+, -, * ou /): ");
    scanf(" %c", &operador);

    switch (operador) {
        case '+':
            resultado = num1 + num2;
            break;
        case '-':
            resultado = num1 - num2;
            break;
        case '*':
            resultado = num1 * num2;
            break;
        case '/':
            resultado = num1 / num2;
            break;
        default:
            printf("Operacao nao reconhecida!\n");
            return 0;
    }

    printf("Resultado = %.2f\n", resultado);

    return 0;
}


RSDS-59.c

#include <stdio.h>

int main() {
    char direcao;

    printf("GPS\n");
    printf("Digite uma letra: ");
    scanf(" %c", &direcao);

    switch (direcao) {
        case 'N':
            printf("Seguir para o Norte\n");
            break;
        case 'S':
            printf("Seguir para o Sul\n");
            break;
        case 'L':
            printf("Virar a Leste (Direita)\n");
            break;
        case 'O':
            printf("Virar a Oeste (Esquerda)\n");
            break;
        default:
            printf("Comando invalido\n");
    }

    return 0;
}


RSDS-60.c


#include <stdio.h>

int main() {
    int dia;

    printf("Dias Uteis\n");
    printf("Digite um numero de 1 a 7: ");
    scanf("%d", &dia);

    switch (dia) {
        case 2:
        case 3:
        case 4:
        case 5:
        case 6:
            printf("Dia Util. Acesso liberado.\n");
            break;

        case 1:
        case 7:
            printf("Fim de Semana. Predio fechado.\n");
            break;

        default:
            printf("Numero invalido.\n");
    }

    return 0;
}
