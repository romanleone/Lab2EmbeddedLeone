#include <msp430.h> 


int sum(int i,int j);

int main(void)
{
    WDTCTL = WDTPW | WDTHOLD;   
    
    int i = 0b10000011000111101; 
    int j = 0b10001011110010001;
    int result;

    result = sum(i,j);

    while(1);

    return 0;
}

int sum(int i,int j)
{
    int result = i+j;

    return result;
}
