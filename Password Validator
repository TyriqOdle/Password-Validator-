
#include <cs50.h>
#include <stdio.h>
#include <ctype.h>

bool valid(string  password);

int main(void)
{

     string password = get_string("Enter your password: ");


    if (valid(password))
    {
        printf("Your password is valid!\n");
    }
    else
    {
        printf("Your password needs at least one uppercase letter, lowercase letter, number and symbol\n");
    }
}

//Function that iterates through the array "password" and returns true or false if they match the criteria using the ctype library 
bool valid(string password)
{
    bool uppercase = false;
    bool lowercase = false;
    bool number = false;
    bool symbol = false;

    for (int i = 0; password[i] != '\0'; i++){
        if (isupper(password[i]))
        {
            uppercase = true;
            continue;
        }

        if (islower(password[i]))
        {
            lowercase = true;
            continue;
        }

        if (isdigit(password[i]))
        {
            number = true;
            continue;
        }

        if (isprint(password[i]))
        {
            symbol = true;
            continue;

        }
    }

    if (uppercase == true && lowercase == true && number == true && symbol == true)
    {
        return true;
    }else {
        return false;
    }

}
