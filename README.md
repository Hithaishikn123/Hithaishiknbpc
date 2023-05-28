# Hithaishiknbpc
//1 wacp to read 2 nums and add


#include <stdio.h>
int main() {    

    int number1, number2, sum;
    
    printf("Enter two integers: ");
    scanf("%d %d", &number1, &number2);

    // calculate the sum
    sum = number1 + number2;      
    
    printf("%d + %d = %d", number1, number2, sum);
    return 0;
}


//2 wacp to find a area of circle

#include <stdio.h>
#include <math.h>
int main()
{
  float radius, area;

  printf("Enter the radius of a circle\n");

  scanf("%f", &radius);

  area = 3.14159*radius*radius;

  printf("Area of the circle = %.2f\n", area);  // printing upto two decimal places

  return 0;
}



//3 wacp to print largest of twonumbers using if statement
#include<stdio.h>
int main ()
{
  int num1, num2;
  num1=12,num2=13;

  if (num1 == num2)
    printf("both are equal");
  else if (num1 > num2) 
    printf("%d is greater", num1);
  else
    printf("%d is greater", num2);

  return 0;
}




//4 wacp to perform multiplication of 2 float values

#include <stdio.h>
int main() {
    double a, b, product;
    printf("Enter two numbers: ");
    scanf("%lf %lf", &a, &b);  
 
    // Calculating product
    product = a * b;

    // %.2lf displays number up to 2 decimal point
    printf("Product = %.2lf", product);
    
    return 0;
}


//5 wacp to cheack the number is odd or even
#include <stdio.h>
int main() {
    int num;
    printf("Enter an integer: ");
    scanf("%d", &num);

    // true if num is perfectly divisible by 2
    if(num % 2 == 0)
        printf("%d is even.", num);
    else
        printf("%d is odd.", num);
    
    return 0;
}


//6 wacp to check if a number is divisible by 5

#include <stdio.h>
 
void main()
{
    int i, num1, num2, count = 0, sum = 0;
 
    printf("Enter the value of num1 and num2 \n");
    scanf("%d %d", &num1, &num2);
    /* Count the number and compute their sum*/
    printf("Integers divisible by 5 are \n");
    for (i = num1; i < num2; i++)
    {
        if (i % 5 == 0)
        {
            printf("%3d,", i);
            count++;
            sum = sum + i;
        }
    }
    
    //7 wacp to check if a number is divisible by 2
    #include<stdio.h>
int main()
{
	int num;
	printf("Enter a number: ");
	scanf("%d"&num);
	if(num%3==0)
	{
		printf("%d is divisible by 3",num);
	}
	else
	{
		printf("%d is not divisible by 3",num);
	}
	return 0;
}


    printf("\n Number of integers divisible by 5 between %d and %d =
 %d\n", num1, num2, count);
    printf("Sum of all integers that are divisible by 5 = %d\n", sum);
}


//8 wacp to print the power of a number without using math.h


#include <stdio.h>

double power(double base, int exponent) {
    double result = 1.0;

    if (exponent >= 0) {
        for (int i = 0; i < exponent; i++) {
            result *= base;
        }
    } else {
        for (int i = 0; i > exponent; i--) {
            result /= base;
        }
    }

    return result;
}

int main() {
    double base;
    int exponent;

    printf("Enter the base number: ");
    scanf("%lf", &base);

    printf("Enter the exponent: ");
    scanf("%d", &exponent);

    double result = power(base, exponent);
    printf("Result: %lf\n", result);

    return 0;
}

//9 c program to print the message hello if the number divisible by 2 and print the message world if the number divisible by 3,print the message hello world if the number is divisible by both 2 and 3
#include <stdio.h>

int main() {
    int number;

    printf("Enter a number: ");
    scanf("%d", &number);

    if (number % 2 == 0 && number % 3 == 0) {
        printf("Hello World\n");
    } else if (number % 2 == 0) {
        printf("Hello\n");
    } else if (number % 3 == 0) {
        printf("World\n");
    }

    return 0;
}


// 10 c program to generate odd number without using loop
#include <stdio.h>

void generateOdd(int n) {
    if (n <= 0) {
        return;
    }

    generateOdd(n - 1);

    if (n % 2 != 0) {
        printf("%d ", n);
    }
}

int main() {
    int limit;

    printf("Enter the limit: ");
    scanf("%d", &limit);

    printf("Odd numbers up to %d: ", limit);
    generateOdd(limit);
    printf("\n");

    return 0;
}

// 11 write a c++ program to print tables of 5
#include <iostream>

void printTableOf5(int limit) {
    for (int i = 1; i <= limit; i++) {
        std::cout << "5 x " << i << " = " << 5 * i << std::endl;
    }
}

int main() {
    int limit;

    std::cout << "Enter the limit: ";
    std::cin >> limit;

    std::cout << "Table of 5 up to " << limit << ":" << std::endl;
    printTableOf5(limit);

    return 0;
}

// 12 write a c program to print tables of 5	
	#include <stdio.h>

void printTableOf5(int limit) {
    for (int i = 1; i <= limit; i++) {
        printf("5 x %d = %d\n", i, 5 * i);
    }
}

int main() {
    int limit;

    printf("Enter the limit: ");
    scanf("%d", &limit);

    printf("Table of 5 up to %d:\n", limit);
    printTableOf5(limit);

    return 0;
}
			      
// 13 wap  to generate numbers divisible by 2 and divisible by 3,but if the number is divisible by both 2 and 3 print the message pass			      
#include <stdio.h>

int main() {
    int start, end;

    printf("Enter the starting number: ");
    scanf("%d", &start);

    printf("Enter the ending number: ");
    scanf("%d", &end);

    printf("Numbers divisible by 2 and 3:\n");
    for (int num = start; num <= end; num++) {
        if (num % 2 == 0 && num % 3 == 0) {
            printf("%d (Pass)\n", num);
        } else if (num % 2 == 0) {
            printf("%d\n", num);
        }
    }

    return 0;
}
				    

				    
				    

