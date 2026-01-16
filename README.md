using System;

class Task3
{
    static void Main()
    {
        // Declare and initialize the array
        int[] numbers = { 3, 7, 12, 19, 21, 25, 30 };

        // Ask the user for input
        Console.Write("Enter a number to search for: ");
        int searchNumber = int.Parse(Console.ReadLine());

        bool found = false;

        // Use a for loop to search the array
        for (int i = 0; i < numbers.Length; i++)
        {
            // Compare user input with array elements
            if (numbers[i] == searchNumber)
            {
                Console.WriteLine($"Number found at position {i}!");
                found = true;

                // Exit the loop immediately
                break;
            }
        }

        // If the number was not found
        if (!found)
        {
            Console.WriteLine("Number not found in the list.");
        }
    }
}
