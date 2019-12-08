# coin-change
#include<stdio.h>
int main()
{
    int coin[9]= {1,2,5,10,20,50,100,500,100};
    int cost,i,coinNumber[10],j=0,Note=0;
    scanf("%d",&cost);
    for(i=9-1; i>=0; i--)
    {
        while(cost>=coin[i])
        {
            cost=cost-coin[i];
 
            coinNumber[j]=coin[i];
            j++;
 
        }
 
    }
    for (i = 0; i < j; i++)
    {
        printf("%d ", coinNumber[i]);
    }
 
}
