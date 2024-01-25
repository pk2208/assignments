# assignments
Question 1
Write a python code for converting integer values to Indian currency notations, without using the currency libraries.
Function Definition:def convert_to_indian_currency_notation(number):
This line defines a function named convert_to_indian_currency_notation that takes an integer number as its parameter.Convert to String: num_str = str(number)
Converts the input integer number to a string (num_str) using the str() function.
Determine Comma Positions: length = len(num_str) comma_positions = [i for i in range(length - 1, 0, -2)]
Calculates the length of the string (num_str) to determine the number of digits.Creates a list comma_positions containing the positions where commas should be inserted. It starts from the second-to-last digit and goes backward by twos.Insert Commas:for position in comma_positions:
num_str = num_str[:position] + ',' + num_str[position:] Iterates over the positions in comma_positions. Inserts a comma at each specified position using string slicing.
Return Result: return num_str
Returns the final string with commas inserted, representing the Indian currency notation.
Example Usage:
input_number = 504678 output_currency_notation = convert_to_indian_currency_notation(input_number)
print("Input:", input_number) print("Output:", output_currency_notation) Sets input_number to 504678.Calls the convert_to_indian_currency_notation function with input_number and stores the result in output_currency_notation.
Prints the input and the converted output.

Question 2
You won’t get caught if you hide behind someone.”Sang-Woo advises Gi-Hun to hide behind someone to avoid getting shot.Gi-Hun follows Sang-Woo's advice and hides behind Ali, who saved his life earlier. Gi-Hun and Ali both have the same height, K Many players saw this trick and also started hiding behind Ali. Now, there are Nplayers standing between Gi-Hun and Ali in a straight line, with the ith player having height Hi.Gi-Hun wants to know the minimum number of players who need to get shot so that Ali is visible in his line of sight.

Explanation:
I = int(input()): Read the number of test cases (n).
for i in range(n):: Loop over each test case.
c = 0: Initialize a counter variable (c) to count the number of players who need to get shot.
p, k = list(map(int, input().split())): Read two space-separated integers, n (number of players between Gi-Hun and Ali) and k (the height of Gi-Hun and Ali).
heights = list(map(int, input().split())): Read the heights of the players between Gi-Hun and Ali.
for i in heights:: Iterate through each player's height.
if p > k:: Check if the height of the current player is greater than the height of Gi-Hun and Ali (k).
c += 1: If the condition is true, increment the counter.
print(c): Print the final count for the current test case, representing the minimum number of players who need to get shot so that Ali is visible in Gi-Hun's line of sight.
for result in results:: Loop through the results list.
print(result): Print each result, representing the minimum number of players who need to get shot for Ali to be visible in Gi-Hun's line of sight in a particular test case. Each result is printed on a new line.
