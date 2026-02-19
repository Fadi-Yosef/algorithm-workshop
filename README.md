# Workshop: Algorithm and Flowchart
For each question in this workshop, you must complete **two** things:

1.  **Write the pseudocode**
2.  **Draw the flowchart** using either
    - **Option 1:** Draw.io (recommended) → export image → upload to
      your repository → link it in this file
    - **Option 2 (optional):** Write a Mermaid flowchart directly in
      Markdown
    - **Option 3 (optional):** Any other valid method

👉 **IMPORTANT:** At the **bottom of each question**, add the
following sections:

### ✔ Pseudocode

### ✔ Flowchart

---

## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and
determine whether it is even or odd.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number % 2 == 0 THEN
        PRINT Even
    ELSE
        PRINT Odd
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> I[/Get input N/]
    I --> B{N % 2 == 0 ?}
    B -->|Yes| C[/Print Even/]
    B -->|No| D[/Print Odd/]
    C --> E([End])
    D --> E([End])
```


## 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs
marks for 3 subjects, calculates the total and average, and displays
both.

### ✔ Pseudocode

```text
Start

Input mark1, mark2, mark3

total ← mark1 + mark2 + mark3

average ← total / 3

Display total

Display average

End
```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[/Input mark1, mark2, mark3/]
B --> C[total = mark1 + mark2 + mark3]
C --> D[average = total / 3]
D --> E[/Display total/]
E --> F[/Display average/]
F --> G([End])
```

## 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its
multiplication table from 1 to 10 using a loop.

### ✔ Pseudocode

```text
Start

Input number

For i ← 1 to 10

result ← number × i

Display "number × i = result"

End For

End

```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[/Input number/]
B --> C[i = 1]
C --> D{Is i <= 10?}
D -- Yes --> E[result = number * i]
E --> F[/Display number x i = result/]
F --> G[i = i + 1]
G --> D
D -- No --> H([End])

```

## 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether
it is positive, negative, or zero.

### ✔ Pseudocode

```text
Start

Input n

If n > 0 then

Display "Positive"

Else if n < 0 then

Display "Negative"

Else

Display "Zero"

End If

End

```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[/Input n/]
B --> C{n > 0?}
C -- Yes --> D[/Display "Positive"/]
C -- No --> E{n < 0?}
E -- Yes --> F[/Display "Negative"/]
E -- No --> G[/Display "Zero"/]
D --> H([End])
F --> H
G --> H

```

## 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple
interest using the formula:

**SI = (P × R × T) / 100**

- **P = Principal** → original amount of money
- **R = Rate of Interest** → percentage per year
- **T = Time** → number of years

### ✔ Pseudocode

```text
Start

Input P, R, T

SI ← (P × R × T) / 100

Display SI

End

```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[/Input P R T/]
B --> C[SI = P * R * T]
C --> D[SI = SI / 100]
D --> E[/Display SI/]
E --> F([End])
```


## 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the
temperature of 7 days, finds the average temperature, and displays it.

### ✔ Pseudocode

```text
Start

sum ← 0

For day ← 1 to 7

Input temp

sum ← sum + temp

End For

average ← sum / 7

Display average

End

```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[sum = 0]
B --> C[day = 1]
C --> D{day <= 7?}
D -- Yes --> E[/Input temp/]
E --> F[sum = sum + temp]
F --> G[day = day + 1]
G --> D
D -- No --> H[average = sum / 7]
H --> I[/Display average/]
I --> J([End])

```

## 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate
the area (**Area = Length × Width**), and display the result.

### ✔ Pseudocode

```text
Start

Input length, width

area ← length × width

Display area

End


```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[/Input length, width/]
B --> C[area = length * width]
C --> D[/Display area/]
D --> E([End])

```

## 8. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a
student's average marks and displays **"Pass"** if average ≥ 50,
otherwise **"Fail"**.

### ✔ Pseudocode
```text
Start

Input average

If average ≥ 50 then

Display "Pass"

Else

Display "Fail"

End If

End

```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[/Input average/]
B --> C{average >= 50?}
C -- Yes --> D[/Display "Pass"/]
C -- No --> E[/Display "Fail"/]
D --> F([End])
E --> F

```

## 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and
calculate its factorial using a loop.

### ✔ Pseudocode

```text
Start

Input n

factorial ← 1

i ← 1

While i ≤ n

factorial ← factorial × i

i ← i + 1

End While

Display factorial

End

```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[/Input n/]
B --> C[factorial = 1]
C --> D[i = 1]
D --> E{Is i <= n?}
E -- Yes --> F[factorial = factorial * i]
F --> G[i = i + 1]
G --> E
E -- No --> H[/Display factorial/]
H --> I([End])

```
## 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the
purchase amount and gives a **10% discount** if the amount is greater
than 1000.

### ✔ Pseudocode

```text
Start

Input amount

If amount > 1000 then

discount ← amount × 0.10

final ← amount − discount

Else

discount ← 0

final ← amount

End If

Display discount

Display final

End

```
### ✔ Flowchart
```mermaid
flowchart TD
A([Start]) --> B[/Input amount/]
B --> C{amount > 1000?}
C -- Yes --> D[discount = amount * 0.10]
D --> E[final = amount - discount]
C -- No --> F[discount = 0]
F --> G[final = amount]
E --> H[/Display discount/]
G --> H
H --> I[/Display final/]
I --> J([End])

```