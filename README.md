# EX. NO: 1(A) : IMPLEMENTATION OF CAESAR CIPHER

## AIM:
To implement the simple substitution technique named Caesar cipher using C language.

## ALOGORITHM:

STEP-1: Read the plain text from the user.

STEP-2: Read the key value from the user.

STEP-3: If the key is positive then encrypt the text by adding the key with each character in the plain text.

STEP-4: Else subtract the key from the plain text.

STEP-5: Display the cipher text obtained above.

## PROGRAM:
```
#include <stdio.h>
#include <string.h>
void caesarCipher(char *text, int shift)
{
for (int i = 0; text[i]; i++)
{
if (text[i] >= 'A' && text[i] <= 'Z')
text[i] = ((text[i]- 'A' + shift) % 26) + 'A';
}
}
int main()
{
char text[] = "NUMBER";
caesarCipher(text, 3);
printf("Encrypted Message: %s\n", text);
caesarCipher(text,-3);
printf("Decrypted Message: %s\n", text);
return 0;
}
```

## OUTPUT:
<img width="1640" height="726" alt="Screenshot 2025-11-20 221335" src="https://github.com/user-attachments/assets/1070de5a-7b8a-48b2-a863-4bf169d763af" />


## RESULT :
 Thus the implementation of ceasar cipher had been executed successfully.
