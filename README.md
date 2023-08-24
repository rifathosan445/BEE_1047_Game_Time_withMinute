Code

    #include <stdio.h>

    int main() {
    int h1, h2, m1, m2, dis1, dis2, n, ho, min;
    scanf("%d %d %d %d", &h1, &m1, &h2, &m2);
    
    dis1 = h1 * 60 + m1;
    dis2 = h2 * 60 + m2;

    if (dis2 <= dis1) {
        dis2 += 24 * 60;
    }

    n = dis2 - dis1;
    ho = n / 60;
    min = n % 60;

    printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", ho, min);

    return 0;
     }
