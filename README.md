# Palindrome Check in Java

A simple Java program that checks whether a given integer is a palindrome by reversing the number and comparing it to the original. This program uses only arithmetic operations and is ideal for beginners learning loops and conditionals in Java.

## Code

package Simple;

public class PalindromeCheck {

text
public static void main(String[] args) {
    int num = 121, temp = num, rev = 0;

    while (temp != 0) {
        rev = rev * 10 + temp % 10;
        temp = temp / 10;
    }

    if (num == rev)
        System.out.println("Palindrome");
    else
        System.out.println("Not Palindrome");
}
}

text

## How it works

- Store the original number in `num` and make a copy in `temp`.
- Reverse the number stored in `temp` using a `while` loop.
- After the loop, compare `num` (original) and `rev` (reversed).
- If both are equal, print **Palindrome**; otherwise, print **Not Palindrome**.

## Example output

For input `121`, the program prints:

Palindrome

text

For input `123`, the program prints:

Not Palindrome

text

## How to run

1. Save this file as `PalindromeCheck.java` inside a folder named `Simple` (because of the package name).
2. Open your terminal or command prompt in the parent directory.
3. Compile the code:

javac Simple/PalindromeCheck.java

text

4. Run the program:

java Simple.PalindromeCheck

text

You’ll see the output based on the number set in the code.
