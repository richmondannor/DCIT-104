# DCIT-104
Programming Fundamentals


#include <stdio.h>

int main()  {

    float sum = 0, count = 0, average;
    int number;
    printf("Enter Any Number :");
    scanf("%d" ,&number);
    for(int i=1; i<number; i++){
        for(int j=2; j<=i; j++){
            if(j==i){
                sum+=i;
                count++;
            }else if(i%j==0){
                break;
            }
        }
    }
    average=sum/count;
    printf("Average = %.2f!", average);
    return 0;
}



