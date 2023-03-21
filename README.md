#include <stdlib.h>    
#include <stdio.h>    
    
int main(){    
    int a,b,count; //定義了三個變數，a、b、count   
    scanf("%d%d",&a,&b); //讀取兩個整數   
    int box[a*b]; //定義一個長度為a*b的數組。 
    for(int i=0;i<(a*b);i++){  //讀取a*b個整數，並將它們儲存在box
        scanf("%d",&box[i]);  
    }  
    for(int y=0;y<b;y++){  //當y<b執行當x<a條件滿足時執行count的值加1，結束後，count的值就等於a*b
        for(int x=0;x<a;x++){  
            count++;  
            printf("%d",box[x*b+y]);  
            if(count%a!=0){  
                printf(" ");  
            }  
        }  
        printf("\n"); //顯示換行 
    }  
}  
