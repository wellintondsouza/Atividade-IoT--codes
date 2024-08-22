#include <stdio.h>
#include <stdlib.h>

int main()
{
    int mmc = 0;
    int n, m;
    int i, j;

    printf("n = ");
    scanf("%d", &n);

    printf("m = ");
    scanf("%d", &m);

    for(i=1; i<=100000 && mmc==0; i++){
        for(j=1; j<=100000 && mmc==0; j++){
            if(n*i==m*j){
                mmc=n*i;
            }
        }
    }

    printf("mmc = %d\n", mmc);

    return 0;
}
