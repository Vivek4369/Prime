//Write a program to find input number is Prime or not
#include<stdio.h>
#include<math.h>
int main()
{
    int n, flag=0;
    printf("Enter the number\n");
    scanf("%d",&n);

    if(n<=1){
        flag = 1;
    }
    else if(n==2);
    else if(n>2){
        if(n%2==0){
            flag = 1;
        }
        else{
            for(int i = 3; i <= sqrt(n); i++){
                if(n%i==0){
                    flag = 1;
                    break ;
                }
            }
        }
    }
    if(flag == 0){
        printf("%d is prime",n);
    }
    else{
        printf("%d is not prime",n);
    }
    return 0;
}
