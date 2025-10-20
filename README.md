# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main(){
    int n=44;
    int shift = 3;
    int result;
    result = n << shift;
    printf("After Left Shift Operation value of a is:%d",result);
    return 0;
}
```
## OUTPUT
<img width="970" height="202" alt="image" src="https://github.com/user-attachments/assets/b556c986-e673-46bd-a020-f627f04fdf06" />









## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TO CHECK WHETHER THE NUMBER IS POSITIVE OR NEGATIVE OR ZERO USING SIMPLE IF 


## AIM
Write a C program to check positive negative or zero using simple if statement

## ALGORITHM
1. Start the program.
2. Declare an integer variable n to store the input number.
3. Read the value of n from the user using scanf.
4. Check if n is greater than 0:
If true, print "Number is POSITIVE".
5. Check if n is less than 0:
If true, print "Number is NEGATIVE".
6. Check if n is equal to 0:
If true, print "Number is ZERO".
7. End the program.

## PROGRAM
```
#include<stdio.h>
int main(){
    int n;
    scanf("%d",&n);
    if(n>0){
        printf("Number is POSITIVE\n");
    }
    if(n<0){
        printf("Number is NEGATIVE\n");
    }
    if(n==0){
        printf("Number is ZERO\n");
    }return 0;
}
```

## OUTPUT
<img width="987" height="311" alt="image" src="https://github.com/user-attachments/assets/7150cc1d-d328-4487-bfcf-7400152c2459" />
           
## RESULT

Thus the program to check positive negative or zero using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <string.h>
#include <ctype.h> 
int main() {
    char str[100];
    int i;
    scanf("%[^\n]", str);
    for(i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]); 
    }
    printf("Lower case String is:%s", str);
    return 0;
}
```
## OUTPUT
<img width="981" height="261" alt="image" src="https://github.com/user-attachments/assets/8257295b-ca32-444f-9d9b-55a546361c44" />




## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using for loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
#include<string.h>
int main(){
    char str[100];
    int i,words=1;
    scanf("%[^\n]",str);
    for(i=0;str[i]!='\0';i++){
        if(str[i]==' '){
            words++;
        }
    }printf("%d",words);
    return 0;
}
```
## OUTPUT
<img width="986" height="263" alt="image" src="https://github.com/user-attachments/assets/e088bae9-3235-4b13-abf3-411670f10a72" />





## RESULT
Thus the program to count the total number of words in a given string using for loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
#include <stdio.h>  
int compare(char[],char[]);  
int main()  
{  
   char str1[20];  
   char str2[20];   
   scanf("%s",str1);  
   scanf("%s",str2);  
   int c= compare(str1,str2);
   if(c==0)  
   printf("strings are same");  
   else  
   printf("strings are not same");    
}   
int compare(char a[],char b[])  
{  
    int flag=0,i=0;   
    while(a[i]!='\0' &&b[i]!='\0')  
    {  
       if(a[i]!=b[i])  
       {  
           flag=1;  
           break;  
       }  
       i++;  
    }  
    if(flag==0)  
    return 0;  
    else  
    return 1;
}  

## OUTPUT
<img width="985" height="311" alt="image" src="https://github.com/user-attachments/assets/068eb485-144f-4257-a4d6-cabd1d3a3791" />
 

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

