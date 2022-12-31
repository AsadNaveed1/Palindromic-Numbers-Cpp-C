// Author : Muhammad Asad Naveed
// U.No : 3035957848
// Assignment 1 Question 1
// Description : A C++ program to find Palindromic and Product of two 3-digit numbers.



#include <iostream>
#include <cmath>
#include <string>
using namespace std;

bool isPalindrome( int o )          // function to find palindrome return true if the integer is palindrome otherwise returns false
{                                       
    int newinteger, multiply;    
    multiply=0;
    int temp=o;

    while(o!=0)                       // this whole while loop first takes out the last digit of the input number and then
    {                                 //regenerates the number in reverse order
        newinteger= o%10;            
        multiply= (multiply*10) + newinteger;
        o= o/10;
    }    

    if(multiply==temp)                //proceeds if the new integer mathces the original number
    {
        return true;
    }    
    else
    {
        return false;
    }            


}

bool isProduct(int x)    // this function takes in an integer and checks if the number is a product of 2 3 digit numbers returns true
{                         //if yes otherwise returns false

    int j,i;
    for(int i=100; i<1000; i++)  //we need 3 digit number, so range from 100 to 1000
        for(int j=100; j<1000; j++)

            if(i*j==x)
            {
                return true;
            }
    return false;            

}

///////////////////////////MAIN FUNCTION/////////////////////////////////////
int main()   //program starts here
{
    int M, N;
    char opt;

    cin>>M>>N>>opt;

    
    if(M<N && M>= 10000 && N<=999999)
    {    
        if(opt=='p')
        {
            for(int i=M; i<=N; ++i)
            {

                if(isPalindrome(i))
                {
                    cout<<i<<endl;
                }    
            
            } 
        }
        else if(opt=='t')
            for(int i=M; i<=N; ++i)
            {
                if(isProduct(i))
                {
                    cout<<i<<endl;
                }



            }


        else if(opt=='b')
         for(int i=M; i<=N; i++)
         {
             if(isProduct(i) && isPalindrome(i))   //to find if the number is both the product of two, 3 digit number and is a palindrome returns true if yes otherwise false
             {
                 cout<<i<<endl;

             }



         }






    }



}
