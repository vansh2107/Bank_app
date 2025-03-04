#include<stdio.h>

int main()
{
    int choice,pin=123;
    float balance = 10000.0;
    printf("enter your pin : ");
    scanf("%d",&choice);

    if (choice == pin){
        while (1)
     {
            printf("1.Deposit\n");
            printf("2.Withdrawl\n");
            printf("3.Cheak Balance\n");
            printf("4.exit\n");
            printf("Enter Your Choice : ");
            scanf("%d",&choice);

            switch (choice)
            {
            case 1:
                printf("enter Amount : ");
                scanf("%f",&balance);
                balance+=balance;
                printf("new balance:%.2f\n",balance);
                break;
            case 2:
                printf("enter Amount : ");
                scanf("%f",&balance);
                balance-=balance;
                printf("new balance:%.2f\n",balance);
                printf("************************************");
                break;
             case 3:
                printf("new balance:%.2f\n",balance);
                printf("************************************\n");
                break;
             case 4:
                break;

            default:
            printf("invalid choice\n");
            break;

            return 0;
            
          
            }
        }
    }

    return 0;
}
