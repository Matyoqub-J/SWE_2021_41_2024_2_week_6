# SWE_2021_41_2024_2_week_6
summarize the work you have done for the week 4 and week 5 assignments

# Week 4 Assingment
[Assingment 4 Link](https://github.com/Matyoqub-J/SWE_2021_41_2024_2_week_4.git)

## Code 
```
def isHappy(n):
  seen = set();
  remainder = sum = 0;
  result = False;

  while ( sum != 1 and n not in seen):
    seen.add(n);
    sum = 0;
    while (n > 0):
      remainder = n%10;
      sum += remainder*remainder;
      n //= 10;
    n=sum;

  if ( sum == 1 ):
    result = True;

  return result;

number = int(input("Input: "));
print(number);
print(isHappy(number));
```
### Description

In `while ( sum != 1 and n not in seen):` loop continues until the sum of the squared digits is equal to 1, 
or if the "n" is already inside the "seen" set(which means that number is stuck in a cycle). 

`seen.add(n)` adds all the values to the set to rack the numbers encountered, and `sum = 0` resets the sum of the past squared digits. 

Inside the `while (n > 0):` variable `remainder = n%10` calculates the digits of a number and which are then squared and added to total sum `sum += remainder*remainder;`,
then `n //= 10;` perfoms division of n by 10 removing the extracted digit. 

In the final steps `if ( sum == 1 ):` in case of the sum of the square digits being equal to 1 `result = True;` changes the output to `True`.



# Week 5 Assingment
