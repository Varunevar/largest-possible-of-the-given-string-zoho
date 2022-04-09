# largest-possible-of-the-given-string-zoho

#include<stdio.h>
#include<conio.h> 
int main()
{ 
    char str[100], chTemp; int i, j, len; printf("Enter any string: "); 
    gets(str);
    len = strlen(str); 
    for(i=0; i<len; i++)
    {
        for(j=0; j<(len-1); j++) 
        {
            if(str[j]>=65 && str[j]<=90)
            { 
                if(str[j+1]>=65 && str[j+1]<=90)
                { 
                    if(str[j]<str[j+1]) { chTemp = str[j];
                    str[j] = str[j+1];
                    str[j+1] = chTemp;
                } 
                    
             }
         } 
                if(str[j]>=97 && str[j]<=122)
                {
                    if(str[j+1]>=97 && str[j+1]<=122)
                    { 
                        if(str[j]<str[j+1]) 
                        { 
                            chTemp =str[j]; 
                            str[j] = str[+1]; 
                            str[j+1] = chTemp;
                         }
                           
                     } 
                    
                } 
            
        } 
        
    } 
  printf("\nLargest possible of the given string:\n%s", str); 
  getch(); 
  return 0;
    }
