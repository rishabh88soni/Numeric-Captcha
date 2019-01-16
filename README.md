# Numeric-Captcha
#how to generate numeric captcha using C language



#include<stdio.h>
#include<stdlib.h>
#include<time.h>
#include<windows.h>

main()

{

                int x,y,z;

                START:

                                {

                        printf("-------------------------------\n");

                        printf("Welcome to Rishabh's project\n");

               printf("-------------------------------");

               printf("\n\n");

               printf("Enter the captcha given below\t or\tPress 1 to Refresh the Captcha.");

               printf("\n");   

                        srand(time(NULL));

                        x=rand();

                        printf("%d",x);

                        printf("\n");

                        printf("Enter here = ");

                        scanf("%d",&y);

                        if(x==y)

                        {

                                        system("cls");

                                        printf("-------------------------------------------------------------------------------\n");

                                        printf("Chose any of the option given below with which you want to proceed further\n");

                                        printf("-------------------------------------------------------------------------------\n\n");

                printf("1 : Add one more captcha \n2 : Delete the captcha \n3 : Verify using captcha \n4 : Exit the program");

                printf("\n");

                                        printf("Enter your choice\n");

                scanf("%d",&z);

                switch(z)

                {

                       case 1 :

                                       {

                                                       system("cls");

                                                       int p,q;

                                                       STA :

                                                                                                        {   

                                                               printf("-----------------------------------------------------------\n");

                                                               printf("As you have chosed to ADD one more captcha to your program\n");

                                                               printf("-----------------------------------------------------------\n\n");

                                                   printf("It is displayed below\n");

                                                   srand(time(NULL));

                                                   p=rand();

                                                   printf("%d",p);

                                                   printf("\n");

                                                   printf("Enter the above CAPTCHA\t or\t Press 1 to refresh the Captcha\n");

                                                   scanf("%d",&q);

                                                   if(p==q)

                                                   {

                                                               system("cls");

                                                               printf("ThankYou\nYou have added new CAPTCHA and it has been verified\n");

                                                                                                }

                                                                                                else if(q==1)

                                                                                                {

                                                                                                                system("cls");

                                                                                                                goto STA;

                                                                                                }

                                                                                                else

                                                                                                {

                                                                                                                system("cls");

                                                                                                                printf("Your Captcha has been created\n\nBut you have Entered Wrong Captcha\n\nVerification could not be completed");

                                                                                                }

                                                                                                break;

                                                                                }

                                                                        }

                                                        case 2 :

                                                            {

                                                                        system("cls");

                                                                        printf("-----------------------------------------\n");

                                                                        printf("Your above CAPTCHA has been deleted\n");

                                                                        printf("-----------------------------------------\n\n");

                                                                        printf("Now you can proceed to my folder directly\n");

                                                                        Sleep(3000);

                                                                        system("cls");

                                                                FILE *fpt,*fptr;

                                                               char cht,chtr;

                                                               fpt=fopen("Document1.txt","r");

                                                               while((cht=getc(fpt))!=EOF)

                                                                        {

                                                                                        printf("%c",cht);

                                                                            }

                                                                        fclose(fpt);

                                                                        printf("\n");

                                                                        fptr=fopen("Document2.txt","r");

                                                                        while((chtr=getc(fptr))!=EOF)

                                                                        {

                                                                                        printf("%c",chtr);

                                                                        }

                                                                        fclose(fptr);

                                                                        break;

                                            }

                                                        case 3 :

                                                {

                                                       system("cls");

                                                            FILE *fp,*fpt;

                                        char ch,cha;

                                        int n,i,a;

                                        STAR :

                                                      {

                                                             printf("--------------------------------------------\n");

                                                printf("Verify wether you are a HUMAN or a ROBOT\n");

                                                printf("--------------------------------------------\n\n");

                                                printf("Enter the CAPTCHA given below\t or\tPress 1 to refresh your Captcha.\n");

                                                srand(time(NULL));

                                    n=rand();

                                    printf("%d",n);  

                                    printf("\n");

                                    scanf("%d",&i);

                                                if(n==i)

                                                                               {

                                                                printf("Accepted\n");

                                              Sleep(2000);

                                              system("cls");

                                              printf("\n");

                                              printf("Now you can proceed further.\n");

                                              printf("____________________________________________________________________________________");

                                                                                                                                                                printf("____________________________________________________________________________________\n");

                                              printf("____________________________________________________________________________________");

                                                                                                                                                                printf("____________________________________________________________________________________\n");

                                              printf("____________________________________________________________________________________");

                                                                                                                                                                printf("____________________________________________________________________________________\n");

                                                                                                                                                                printf("\n");

                                              fp=fopen("Rishabh.txt","r");

                                              while((ch=getc(fp))!=EOF)

                                        {

                                             printf("%c",ch);

                                        }

                                        fclose(fp);

                                        printf("\n\n");

                                              printf("To access my folder you need to give answer of Security Question\n\n");

                                              Sleep(10000);

                                              system("cls");

                                              printf("What is my age?\n");

                                              scanf("%d",&a);

                                              if(a==18)

                                        {

                                            Sleep(1000);

                                                        system("cls");

                                                        printf("\nYour identification has been Approved");

                                            Sleep(2000);

                                                        system("cls");

                                                        fpt=fopen("RishabhSoni.txt","r");

                                                                    while((cha=getc(fpt))!=EOF)

                                                        {

                                                                  printf("%c",cha);

                                                        }

                                                        fclose(fpt);

                                        }

                                                    else

                                                    {

                                                            system("cls");

                                                            printf("-------------------------------------\n");

                                                                  printf("Your identification is not approved\n");

                                                                  printf("-------------------------------------\n\n");

                                                                  printf("-------------\n");

                                                                    printf("Thank You!");

                                                                    printf("-------------\n");

                                                    }     

                                                                                    }

                                                                                    else if(i==1)

                                                                                    {

                                                                                                system("cls");

                                                                                                goto STAR;

                                                                                                }

                                                else

                                   {

                                             system("cls");

                                                   printf("-------------------\n");

                                                                                                                                                                printf("You are a robot\n");

                                                                                                                                                                printf("-------------------\n\n");

                                                                                                                                                                printf("---------------------------------------\n");

                                                   printf("You cannot proceed further\nTHANKYOU");

                                                   printf("---------------------------------------\n");

                                                }

                                                break;

                                            }

                                    }

                                case 4 :

                                       {

                                                       system("cls");

                                                       printf("--------------------------------------\n");

                                                       printf("Your program is ended successfully\n");

                                                       printf("--------------------------------------\n\n");

                                                       printf("-------------\n");

                                                       printf("Thank You!");

                                                       printf("-------------\n");

                                                       break;

                                                                        }

                                                        default :

                                                                        {

                                                                               system("cls");

                                                                               printf("-----------------------------------\n");

                                                                                        printf("You have entered wrong detail.\n");

                                                                                        printf("-----------------------------------\n\n");

                                                                                        printf("------------\n");

                                                                                        printf("Thank You!\n");

                                                                                        printf("------------\n");

                                                                        }

                                        }

                        }

               else if(y==1)

                        {

                                        system("cls");

                                        goto START;

                        }

                        else

                        {

                               system("cls");

                               printf("-------------------------------------------------\n");

                                        printf("Make sure that you have entered correct captcha.\n");

                                        printf("-------------------------------------------------\n\n");

                                        printf("-----------\n");

                                                                printf("ThankYou!\n");

                                                                printf("-----------\n");

                        }

        }

}
