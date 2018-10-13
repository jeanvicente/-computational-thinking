# -computational-thinking
QUESTIONS FROM THE COMPUTER THOUGHT LESSON "URI JUDGE"    /////QUESTÕES DA AULA DE PENSAMENTO COMPUTACIONAL "URI JUDGE"    1037 1038 1040 1041 1042 1043 1044 1046 1047 1048 1050 1052 1060 1065 10
/* questao 1024 URI*/
#include<stdio.h>
#include<string.h>

int main()
{
    int i,j,k=3,l,n,o,p;
    char ch[1002],ch1[1002];
    scanf("%d",&n);
    getchar();
    for(i = 0;i < n;i++)
    {
        gets(ch);
        l = strlen(ch);
        for(j=0;j<l;j++){
            if((ch[j]>='A' && ch[j]<='Z') || (ch[j]>='a' && ch[j]<='z'))ch[j] += 3;
        }
        p=l-1;
        for(j=0;j<l;j++){
            ch1[j]=ch[p];
            p--;
        }
        ch1[j]='\0';
        for(j = l/2;j < l;j++)
            ch1[j] -= 1;
        printf("%s\n",ch1);
    }
    return 0;
    }
/*questao  1037*/#include <stdio.h>
int main()
{
    double a;
    scanf ("%lf",&a);
    if(a<0||a>100)
        printf ("Fora de intervalo\n");
    else if(a>=0&&a<=25)
        printf ("Intervalo [0,25]\n");
    else if(a>25&&a<=50)
        printf ("Intervalo (25,50]\n");
    else if (a>50&&a<=75)
        printf ("Intervalo (50,75]\n");
    else if (a>75&&a<=100)
        printf ("Intervalo (75,100]\n");
    return 0;
}
/* questao  1038*/
#include<stdio.h>
int main(void){
    float x,y,price;
    scanf("%f%f",&x,&y);
    if(y==1)
        y=4.00;
    else if(y==2)
        y=4.50;
    else if(y==3)
        y=5.00;
    else if(y==4)
        y=2.00;
    else if(y==5)
        y=1.50;
        
    if(x==1)
        price=y+4.00;
    else if(x==2)
        price=y+4.50;
    else if(x==3)
        price=y+5.00;
    else if(x==4)
        price=y+2.00;
    else if(x==5)
        price=y+1.50;
    printf("Total: R$ %.2f\n",price);
    return 0;
}
/*questao 1040*/
#include <stdio.h>
int main()
{
    double N1, N2, N3, N4, N5, a,b;
    scanf ("%lf%lf%lf%lf", &N1,&N2,&N3,&N4);
    a=((N1*2)+(N2*3)+(N3*4)+N4)/10;
    printf ("Media: %.1lf\n",a);
    if(a>=7)
        printf ("Aluno aprovado.\n");
    else if(a<5)
        printf("Aluno reprovado.\n");
    else if(a>=5&&a<=6.9)
    {
        printf ("Aluno em exame.\n");
        scanf("%lf", &N5);
        printf ("Nota do exame: %.1lf\n",N5);
        b=(N5+a)/2;
        if(b>=5)
            printf ("Aluno aprovado.\n");
        else if(b<=4.9)
            printf ("Aluno reprovado.\n");
        printf ("Media final: %.1lf\n",b);
    }
    return 0;
}
/* questao 1041 URI */
#include <stdio.h>
int main()
{
    double X,Y;
    scanf ("%lf%lf", &X, &Y);
    if(X==0&&Y==0) printf("Origem\n");
    else if(X==0) printf("Eixo Y\n");
    else if(Y==0) printf("Eixo X\n");
    else if(X>0&&Y>0) printf("Q1\n");
    else if(X<0&&Y>0) printf("Q2\n");
    else if(X<0&&Y<0) printf("Q3\n");
    else if(X>0&&Y<0) printf("Q4\n");
    return 0;
}

/* questao 1042* /
#include <stdio.h>
int main()
{
    int A,B,C;
    scanf ("%d%d%d", &A,&B,&C);
    if(A<B&&A<C)
    {
        if(B<C)
            printf("%d\n%d\n%d\n",A,B,C);
        else printf("%d\n%d\n%d\n",A,C,B);
    }
    if(B<A&&B<C)
    {
        if(A<C)
            printf("%d\n%d\n%d\n",B,A,C);
        else printf("%d\n%d\n%d\n",B,C,A);
    }
    if(C<B&&C<A)
    {
        if(B<A)
            printf("%d\n%d\n%d\n",C,B,A);
        else printf("%d\n%d\n%d\n",C,A,B);
    }
    printf ("\n%d\n%d\n%d\n",A,B,C);
    return 0;
}

