# -computational-thinking
QUESTIONS FROM THE COMPUTER THOUGHT LESSON "URI JUDGE"    /////QUESTÕES DA AULA DE PENSAMENTO COMPUTACIONAL "URI JUDGE"    1037 1038 1040 1041 1042 1043 1044 1046 1047 1048 1050 1052 1060 1065 1024

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
          for(j=0;j<l;j++)
      { 
        if((ch[j]>='A' && ch[j]<='Z') || (ch[j]>='a' && ch[j]<='z'))ch[j] += 3;
                  }      
        p=l-1;
         for(j=0;j<l;j++) 
      {
            ch1[j]=ch[p];
           p--;   }
        ch1[j]='\0';
          for(j = l/2;j < l;j++)
            ch1[j] -= 1;
              printf("%s\n",ch1);
                 }
    return 0;
                 }
/*questao URI 1037*/#include <stdio.h>
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

/* questao URI 1038*/
#include<stdio.h>
int main(void)
{
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

/*questao URI 1040*/
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
        printf ("Media final: %.1lf\n",b);  }
    return 0;
   }
   
/* questao 1041 URI*/
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

/*questao URI 1042*/
/* questao 1042*/
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
/*1042 ACHEI OUTRA FORMA DE SOLUCIANAR */

#include <stdio.h>

int main()
{  int A, B, C;
    int x,y,z;
    int temp;
    scanf( "%d %d %d", &A, &B, &C );
    x=A;
    y=B;
    z=C;
  if(x > y)
    {temp=x;
     x=y;
     y=temp;}
 if(z>y) 
    {temp=x;
     x=z;
     z=temp;}
 if(y>z)
    {temp=y;
     y=z;
     z=temp;}
      printf("%d\n%d\n%d\n", x, y ,z);
      printf("\n");
      printf("%d\n%d\n%d\n", A, B,C);
 return 0;
}
/* questao 1043 */ 
#include<stdio.h>
int main()
{
   float A, B, C, area, perimetro ;
    scanf("%f %f %f", &A, &B, &C);
   if ((A < (float)(B+C)) && (B < (float)(A+C)) && (C < (float)(B+A)))
    {
        perimetro = A + B + C;
        printf("Perimetro = %.1f\n",perimetro);}
   else
    {
        area= ((A + B) * C) / 2;
        printf("Area = %.1f\n",area);}
    return 0;
}

/*questao 1044*/
#include <stdio.h>

int main()
{
    int A,B;
     scanf("%d %d",&A,&B) ;
      if( B%A == 0 || A%B == 0)
   { 
   printf("são multiplos:\n");}
    else
    {
      printf("não são multiplos:\n");}
    return 0;
}

/* questao 1046*/
#include <stdio.h>

    int tempo (int x, int y){
        int t;
        if(y <= x) y += 24;
        t = y - x;
        return t;
    }
int main(){
    int inicial, final;
    scanf("%d %d", &inicial, &final);
    printf("o jogo durou %d horas(s) \n", tempo(inicial, final));
    return 0;
}
/* questao 1047*/

#include <stdio.h>
int main()
{
    int a,b,c,d,x,y;
    scanf("%d%d%d%d", &a, &x, &b, &y);
    if(a == y && b == y && y == x)
    {
        c =x-y;
        d =24+a-b;
        printf( "O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c );
    }
    else if(a==b && y>x)
    {
        c =y-x;
        d =a-b;
        printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c );
    }
    else if(a == b && x>y )
    {
        c =60-x+y;
        d =24-a+b-1;
        printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c );
    }
    else if(x==y && a<b)
    {
        c =0;
        d =b-a;
        printf( "O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c );
    }
    else if(x==y && a>b)
    {
        c =0;
        d =24-a+b;
        printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c);
    }
    else if(b>a && y>x)
    {
        c =y-x;
        d =b-a;
        printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c );
    }
    else if(a<b && x>y)
    { 
        c= 60-x+y;
        d= b-a-1;
        printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c );
    }
    else if(a>b && x<y)
    {
        c=y-x;
        d=24-a-1+b;
        printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c);
    }
    else if(a > b && x > y)
    { c= 60+y-x;
    d= 24+b-a-1;
    printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", d, c);
    }
    return 0;
}

   /*questao 1048*/
   #include<stdio.h>
int main()
{
 float n;
        scanf("%f", &n);
    if (n <= 400.0)
         printf("Novo salário: %.2f\nReajuste ganho: %.2f\nEm percentual: 15 %%\n", n * 1.15, n * 0.15);
         else if (n <= 800.0)
         printf("Novo salário: %.2f\nReajuste ganho: %.2f\nEm percentual: 12 %%\n", n * 1.12, n * 0.12);
         else if (n <= 1200.0)
         printf("Novo salário: %.2f\nReajuste ganho: %.2f\nEm percentual: 10 %%\n", n * 1.10, n * 0.10);
         else if (n <= 2000.0)
         printf("Novo salário: %.2f\nReajuste ganho: %.2f\nEm percentual: 7 %%\n", n * 1.07, n * 0.07);
         else
         printf("Novo salário: %.2f\nReajuste ganho: %.2f\nEm percentual: 4 %%\n", n * 1.04, n * 0.04);
    return 0;
    }
    /* questao 1050*/
    int main()
{
   int N;
    scanf("%d",&N);
    if(N==61)
        printf("Brasilia\n");
    else if(N==71)
        printf("Salvador\n");
    else if(N==11)
        printf("São Paulo\n");
    else if(N==21)
        printf("Rio de Janeiro\n");
    else if(N==32)
        printf("Juiz de Fora\n");
    else if(N==19)
        printf("Campinas\n");
    else if(N==27)
        printf("Vitoria\n");
    else if(N==31)
        printf("Belo Horizonte\n");
    else if(N==84)
        printf("Rio grande do norte\n");
    else if(N==85)
        printf("Fortaleza\n");
    else if(N==83)   
        printf("joão pessoa\n");
    else if(N==88)
        printf("ceara\n");
    else
        printf(" DDD nao cadastrado\n");
    return 0;
}
/* questao 1052*/
#include<stdio.h>
int main()
{
    int N;
    scanf("%d", &N);
    switch (N)
    {
    case 1:
    printf("January\n");break;
    case 2:
    printf("February\n");break;
    case 3:
    printf("March\n");break;
    case 4:
    printf("April\n");break;
    case 5:
    printf("May\n");break;
    case 6:
    printf("June\n");break;
    case 7:
    printf("July\n");break;
    case 8:
    printf("August\n");break;
    case 9:
    printf("September\n");break;
    case 10:
    printf("October\n");break;
    case 11:
    printf("November\n");break;
    case 12:
    printf("December\n");break;
    default:
        break;
    }
}
/*questao 1060*/
#include <stdio.h>

int main()
{ int x;
  int p;
  int i;
  
  
  p = 0;
  for(i = 1; i <= 6; i++){
    scanf("%d, &x ");
    if(x%2==0) p++;
  }

    printf("%d numeros pares");
    return 0;
}

   

