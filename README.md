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
    if(x==1)
        price=y*4.00;
    else if(x==2)
        price=y*4.50;
    else if(x==3)
        price=y*5.00;
    else if(x==4)
        price=y*2.00;
    else if(x==5)
        price=y*1.50;
    printf("Total: R$ %.2f\n",price);
    return 0;
}
