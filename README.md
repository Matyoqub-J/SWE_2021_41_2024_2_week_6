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
