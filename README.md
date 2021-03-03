# Iv-n-Alonzo-Chapter-5
EXERCISE1
//Write a program that converts Centigrade to Fahrenheit.
#include <stdio.h>

char line[100];

float celsius;
float fahrenheit;

int main()
{
  printf("Enter celsius quantity: ");

  fgets(line, sizeof(line), stdin);
  sscanf(line, "%f", &celsius);

  fahrenheit = 9.0 / 5.0 * celsius + 32;

  printf("%f°C are %f°F\n", celsius, fahrenheit);

  return 0;
}

EXERCISE 2
//Write a program to calculate the volume of a sphere.
#include <stdio.h>

const float PI = 3.1416;

char line[100];

float volume;
float radius; 

int main()
{
  printf("Enter the radius of the sphere in cm: ");

  fgets(line, sizeof(line), stdin);
  sscanf(line, "%f", &radius);

  volume = 4.0 / 3.0 * PI * (radius * radius * radius);

  printf("The volume of the sphere is: %f cm^3\n", volume);

  return 0;
}

EXERCISE 3
//Write a program that prints the perimeter of a rectangle given its height and width. 
#include <stdio.h>

char line[100];

float width;
float height;
float perimeter;

int main()
{
  printf("Enter width of the rectangle in cm: ");
  fgets(line, sizeof(line), stdin);
  sscanf(line, "%f", &width);

  printf("Enter heigth of the rectangle in cm: ");
  fgets(line, sizeof(line), stdin);
  sscanf(line, "%f", &height);

  perimeter = 2 * (width + height);

  printf("The perimeter of the rectangle is: %f cm\n", perimeter);

  return 0;
}

EXERCISE 4
//Write a program that converts kilometers per hour to miles per hour. 
#include <stdio.h>

char line[100];

float kilometers;
float miles;

int main()
{
  printf("Enter the km/h to convert them to mi/h: ");

  fgets(line, sizeof(line), stdin);
  sscanf(line, "%f", &kilometers);

  miles = kilometers * 0.6213712;

  printf("mi/h: %f\n", miles);

  return 0;
}

EXERCISE 5
//Write a program that takes hours and minutes as input, and then outputs the total number of minutes. 
#include <stdio.h>

char line[100];

float hours;
unsigned int minutes;

int main()
{
  printf("Enter quantity of hours: ");

  fgets(line, sizeof(line), stdin);
  sscanf(line, "%f", &hours);

  printf("Enter quantity of minutes: ");

  fgets(line, sizeof(line), stdin);
  sscanf(line, "%d", &minutes);

  minutes = minutes + (hours * 60);

  printf("%d minutes\n", minutes);

  return 0;
}

EXERCISE 6
//Write a program that takes an integer as the number of minutes, and outputs the total hours and minutes
#include <stdio.h>

char line[100];

int minutes;
int hours;

int main()
{
  printf("Enter the quantity of minutes: ");

  fgets(line, sizeof(line), stdin);
  sscanf(line, "%d", &minutes);

  hours = minutes / 60;
  
  minutes = minutes - (hours * 60);

  printf("%d hours %d minutes\n", hours, minutes);

  return 0;
}

EXERCISE 7
//Write a program that converts centimeters to inches. 
#include <stdio.h>

char line[100];

float centimeters;
float inches;

int main()
{
  printf("Enter centimeters quantity: ");

  fgets(line, sizeof(line), stdin);
  sscanf(line, "%f", &centimeters);

  inches = centimeters / 2.54;

  printf("%f cm is equal to %f inches\n", centimeters, inches);

  return 0;
}
