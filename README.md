//
// Created by pekayprkr on 11/29/2022.
//for Checking Program

#include "stdio.h"
#include "stdlib.h"
#include "string.h"
///////////////////////////////////////////////////////////////////////

float perline2 =0.0;
float perInt2 =0.0;
float perChar2 =0.0;
float perForLoop2 =0.0;
float perIf2 =0.0;
float perVoid2=0.0;

///////////////////////////////////////////////////////////////////////

float sumPercentage=0.0;
float totalPercentage =0.0;

///////////////////////////////////////////////////////////////////////


float perline;
float perVoid;
float perInt;
float perChar;
float perForLoop;
float perIf;

///////////////////////////////////////////////////////////////////////
int difLine;
int difVoid;
int difInt;
int difChar;
int difForLoop;
int difIf;

///////////////////////////////////////////////////////////////////////
int sumLine;
int sumInt;
int sumVoid;
int sumChar;
int sumForLoop;
int sumIf;


///////////////////////////////////////////////////////////////////////

int count;
int ifcount;
int voidcount;
int intecout;
int integer;
int charcount;
int forloopcount;
char fileArr;
char line[100];

///////////////////////////////////////////////////////////////////////


int count2;
int ifcount2;
int intecout2;
int voidcount2;
int integer2;
int charcount2;
int forloopcount2;
char fileArr2;
char line2[100];

///////////////////////////////////////////////////////////////////////

//For Fiel One

int intForFile1;
int voidForFile1;
int charForFile1;
int forLoopForFile1;
int ifForFile1;
int lineForFile1;

///////////////////////////////////////////////////////////////////////

//For Fiel Two

int intForFile2;
int voidForFile2;
int charForFile2;
int forLoopForFile2;
int ifForFile2;
int lineForFile2;

///////////////////////////////////////////////////////////////////////

int main() {
    FILE *fptr1, *fptr2;

    fptr1 = fopen("examOne.txt", "r");
    fptr2 = fopen("examTwo.txt", "r");

    if (fptr1 == NULL) {
        printf("File Cannot Open!");
    } else {

        while ((fileArr=fgetc(fptr1)) != EOF) {
            if (fileArr == ';'){
                 count++;
                 lineForFile1=count;

            }

            if (fileArr == 'i'){
                if (fileArr == 'n'){
                    if (fileArr == 't'){
                        if (fileArr == ' '){
                        }

                    }
                }
                intecout++;
                intForFile1=intecout;
            }

            if (fileArr == 'v'){
                if (fileArr == 'o'){
                    if (fileArr == 'i'){
                        if (fileArr == 'd'){
                            if (fileArr == ' '){
                            }
                        }

                    }
                }
                voidcount++;
                voidForFile1=voidcount;
            }


            if (fileArr == 'c'){
                if (fileArr == 'h'){
                    if (fileArr == 'a'){
                        if (fileArr == 'r'){
                            if (fileArr == ' '){

                            }

                        }

                    }
                }
                charcount++;
                charForFile1=charcount;

            }

            if (fileArr == 'f'){
                if (fileArr == 'o'){
                    if (fileArr == 'r'){
                        if (fileArr == ' '){

                        }

                    }
                }
                forloopcount++;
                forLoopForFile1=forloopcount;
            }


            if (fileArr == 'i'){
                if (fileArr == 'f'){
                    if (fileArr == '('){
                    }
                }
                ifcount++;
                ifForFile1=ifcount;
            }

 //           printf("%c",fileArr);
        }
//////////////////////////////////////////////////////////////////////////////////////

        while ((fileArr2=fgetc(fptr2)) != EOF) {
            if (fileArr2 == ';'){
                count2++;
                lineForFile2 = count2;
            }

            if (fileArr2 == 'i'){
                if (fileArr2 == 'n'){
                    if (fileArr2 == 't'){
                        if (fileArr2 == ' '){
                        }

                    }
                }
                intecout2++;
                intForFile2 = intecout2;

            }

            if (fileArr2 == 'v'){
                if (fileArr2 == 'o'){
                    if (fileArr2 == 'i'){
                        if (fileArr2 == 'd'){
                            if (fileArr2 == ' '){
                            }
                        }

                    }
                }
                voidcount2++;
                voidForFile2 = voidcount2;

            }



            if (fileArr2 == 'c'){
                if (fileArr2 == 'h'){
                    if (fileArr2 == 'a'){
                        if (fileArr2 == 'r'){
                            if (fileArr2 == ' '){

                            }

                        }

                    }
                }
                charcount2++;
                charForFile2 = charcount2;

            }

            if (fileArr2 == 'f'){
                if (fileArr2 == 'o'){
                    if (fileArr2 == 'r'){
                        if (fileArr2 == ' '){
                        }

                    }
                }
                forloopcount2++;
                forLoopForFile2 = forloopcount2;
            }


            if (fileArr2 == 'i'){
                if (fileArr2 == 'f'){
                    if (fileArr2 == '('){
                    }
                }
                ifcount2++;
                ifForFile2 = ifcount2;
            }

            //           printf("%c",fileArr);
        }



//////////////////////////////////////////////////////////////////////////////////////


            printf("\nFor File One\n");
            printf("==========================\n");
            printf("Line Number         = %d\n",count);
            printf("Integer Number      = %d\n",intecout);
            printf("Char Number         = %d\n",charcount);
            printf("Void Number         = %d\n",voidcount);
            printf("ForLooop Number     = %d\n",forloopcount);
            printf("If statement Number = %d\n",ifcount);

        printf("\n\nFor File Two\n");
        printf("==========================\n");
        printf("Line Number         = %d\n",count2);
        printf("Integer Number      = %d\n",intecout2);
        printf("Void Number         = %d\n",voidcount2);
        printf("Char Number         = %d\n",charcount2);
        printf("ForLooop Number     = %d\n",forloopcount2);
        printf("If statement Number = %d\n",ifcount2);
        printf("==========================\n");


/////////////////////////////////////////////////////////////////////////////////////

        if (intForFile1 > intForFile2){
            difLine = voidForFile1 - voidForFile2;
        } else{
            difLine = voidForFile2 - voidForFile1;
        }



        if (intForFile1 > intForFile2){
            difInt = intForFile1 - intForFile2;
        } else{
            difInt = intForFile2 - intForFile1;
        }



        if (charForFile1 > charForFile2){
            difChar = charForFile1 - charForFile2;
        } else{
            difChar = charForFile2 - charForFile1;
        }


        if (forLoopForFile1 > forLoopForFile2){
            difForLoop = forLoopForFile1 - forLoopForFile2;
        } else{
            difForLoop = forLoopForFile2 - forLoopForFile1;
        }



        if (ifForFile1 > ifForFile2){
            difIf = ifForFile1 - ifForFile2;
        } else{
            difIf = ifForFile2 - ifForFile1;
        }


////////////////////////////////////////////////////////////////////////

        sumLine = lineForFile1 + lineForFile2;
        sumInt = intForFile1 + intForFile2;
        sumChar = charForFile1 + charForFile2;
        sumForLoop = forLoopForFile1 + forLoopForFile2;
        sumIf = ifForFile1 + ifForFile2;
        sumVoid = voidForFile1+ voidForFile2;

/////////////////////////////////////////////////////////////////////////

        perline = ((float)difLine * 100) / sumLine;
        perInt = ((float)difInt * 100) / sumInt;
        perChar =((float)difChar * 100) / sumChar;
        perForLoop=((float)difForLoop*100)/sumForLoop;
        perIf = ((float)difIf * 100) / sumIf;
        perVoid = ((float)difVoid * 100)/ sumVoid;
/////////////////////////////////////////////////////////////////////////

        perline2 = 100 - perline;
        perInt2 = 100 - perInt;
        perChar2 = 100 - perChar;
        perForLoop2 = 100 - perForLoop;
        perIf2 = 100 - perIf;

//////////////////////////////////////////////////////////////////////////////

sumPercentage = perline2+ perInt2 + perChar2 +perIf2 +perForLoop2;

totalPercentage =sumPercentage / 5;

/////////////////////////////////////////////////////////////////////////


        printf("Different OF Line    = %d\n",difLine);
        printf("Different OF Int     = %d\n",difInt);
        printf("Different OF Void    = %d\n",difVoid);
        printf("Different OF Char    = %d\n",difChar);
        printf("Different OF ForLoop = %d\n",difForLoop);
        printf("Different OF If      = %d\n",difIf);
        printf("==========================\n");


///////////////////////////////////////////////////////////////////////////////

        printf("Sum OF Line    = %d\n",sumLine);
        printf("Sum OF Int     = %d\n",sumInt);
        printf("Sum OF Void    = %d\n",sumVoid);
        printf("Sum OF ForLoop = %d\n",sumForLoop);
        printf("Sum OF Char    = %d\n",sumChar);
        printf("Sum OF If      = %d\n",sumIf);
        printf("==========================\n");


//////////////////////////////////////////////////////////////////////////////

        printf("Percentage OF Line    = %.2lf %%\n",perline2);
        printf("Percentage OF Int     = %.2f %%\n",perInt2);
        printf("Percentage OF Void    = %.2f %%\n",perVoid2);
        printf("Percentage OF Char    = %.2f %%\n",perChar2);
        printf("Percentage OF ForLoop = %.2f %%\n",perForLoop2);
        printf("Percentage OF If      = %.2f %%\n",perIf2);
//        printf("Sum OF Percentage     = %.2f %%\n",sumPercentage);

//////////////////////////////////////////////////////////////////////////////

        printf("\n\n=====================================\n");
        printf("Same Total Percentage     = %.2f %%\n",totalPercentage);
        printf("=====================================\n\n");


///////////////////////////////////////////////////////////////////////////////

        fclose(fptr1);
        fclose(fptr2);

    }
    return 0;
}

///////////////////////////////////////////////////////////////////////////////
