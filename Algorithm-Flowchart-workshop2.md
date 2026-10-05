# Workshop: Algorithm and Flowchart

## 1. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs
marks for 3 subjects, calculates the total and average, and displays
both.

### pseudocode

```
START

    INPUT A,B,C
    SET Total=a+b+c
    SET Average= Total/3
    Display Total
    Display Average

END

```

### Flowchart

``` mermaid
flowchart TD
    A([START])-->B[/GET INPUT A,B,C/]
    B --> C[SET Total = A + B + C]
    C --> D[SET Average = Total / 3]
    D --> E[/DISPLAY Total/]
    E --> F[/DISPLAY Average/]
    F --> G([END])

````


## 2. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its
multiplication table from 1 to 10 using a loop.


### Pseudocode

```
START

    INPUT X

    FOR i = 1 TO 10
        SET Result = X * i
        DISPLAY X, " x ", i, " = ", Result
    END FOR

END
```

### Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT X/]
    B --> C[SET i = 1]
    C --> D{i <= 10?}
    D -->|YES| E[SET Result = X * i]
    E --> F[/DISPLAY X, "x" , i = Result/]
    F --> G[SET i = i + 1]
    G --> |Continue looping|D
    D -->|NO| H([END])
```

## 3. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether
it is positive, negative, or zero.

### Pseudocode

```
START

    INPUT X

    IF X > 0 THEN
        DISPLAY "Positive"
    ELSE IF X < 0 THEN
        DISPLAY "Negative"
    ELSE
        DISPLAY "Zero"

END
```

### Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT X/]
    B --> C{X > 0?}

    C -->|YES| D[/DISPLAY "Positive"/]
    C -->|NO| E{X < 0?}

    E -->|YES| F[/DISPLAY "Negative"/]
    E -->|NO| G[/DISPLAY "Zero"/]

    D --> H([END])
    F --> H
    G --> H
```

## 4. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple
interest using the formula:

**SI = (P × R × T) / 100**

- **P = Principal** → original amount of money
- **R = Rate of Interest** → percentage per year
- **T = Time** → number of years


### pesudocode
```
START

    INPUT P, R, T

    SET SI = (P * R * T) / 100

    DISPLAY SI

END

```
### Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT P, R, T/]
    B --> C[SET SI = P * R * T / 100]
    C --> D[/DISPLAY SI/]
    D --> E([END])
```

## 5. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the
temperature of 7 days, finds the average temperature, and displays it.
### Pesudocode
```
START

    SET Total = 0

    FOR Day = 1 TO 7
        INPUT Temperature
        SET Total = Total + Temperature
    END FOR

    SET Average = Total / 7

    DISPLAY Average

END
```

### Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Set Total = 0]
    B --> C[Set Day = 1]
    C --> D{Day <= 7?}
    D -->|Yes| E[/Input Temperature/]
    E --> F[Total = Total + Temperature]
    F --> G[Day = Day + 1]
    G --> D
    D -->|No| H[Average = Total / 7]
    H --> I[/Display Average/]
    I --> J([End])
```

## 6. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate
the area (**Area = Length × Width**), and display the result.


### pseducode
```
START

    INPUT Length, Width
    SET Area = Length * Width
    DISPLAY Area

END
```

### Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Length, Width/]
    B --> C[Area = Length * Width]
    C --> D[/Display Area/]
    D --> E([End])
```

## 7. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a
student's average marks and displays **"Pass"** if average ≥ 50,
otherwise **"Fail"**.

## pseducode

```
START

    INPUT Average

    IF Average >= 50 THEN
        DISPLAY "Pass"
    ELSE
        DISPLAY "Fail"
    END IF

END
```

## Flowchart


```mermaid
flowchart TD
    A([Start]) --> B[/Input Average/]
    B --> C{Average >= 50?}
    C -->|Yes| D[/Display Pass/]
    C -->|No| E[/Display Fail/]
    D --> F([End])
    E --> F
```

## 8. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and
calculate its factorial using a loop.

### pseducode

```
START

    INPUT Number
    SET Factorial = 1

    FOR i = 1 TO Number
        SET Factorial = Factorial * i
    END FOR

    DISPLAY Factorial

END
```

### Flowchart


```mermaid
flowchart TD
    A([Start]) --> B[/Input Number/]
    B --> C[Set Factorial = 1]
    C --> D[Set i = 1]
    D --> E{i <= Number?}
    E -->|Yes| F[Factorial = Factorial * i]
    F --> G[i = i + 1]
    G --> E
    E -->|No| H[/Display Factorial/]
    H --> I([End])
```

## 9. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the
purchase amount and gives a **10% discount** if the amount is greater
than 1000.

### Pesudocode

```
START

    INPUT PurchaseAmount

    IF PurchaseAmount > 1000 THEN
        SET Discount = PurchaseAmount * 0.10
        SET FinalAmount = PurchaseAmount - Discount
    ELSE
        SET FinalAmount = PurchaseAmount
    END IF

    DISPLAY FinalAmount

END
```
### Flowchart


```mermaid
flowchart TD
    A([Start]) --> B[/Input Purchase Amount/]
    B --> C{Purchase Amount > 1000?}
    C -->|Yes| D[Discount = Purchase Amount * 0.10]
    D --> E[Final Amount = Purchase Amount - Discount]
    C -->|No| F[Final Amount = Purchase Amount]
    E --> G[/Display Final Amount/]
    F --> G
    G --> H([End])
```


## Optional Exercises (11–16)

## 11. Online Shopping Delivery Eligibility

Write the algorithm and draw the flowchart for a program that inputs a
customer's purchase amount and displays **"Free Delivery"** if the
amount is 500 SEK or more; otherwise display **"Delivery Charge
Applies"**.

---

### Pseducode
```
START

    INPUT User-PurchaseAmount

    IF PurchaseAmount >= 500 THEN
        DISPLAY "Free Delivery"
    ELSE
        DISPLAY "Delivery Charge Applies"
    END IF

END
```
### Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input User-Purchase Amount/]
    B --> C{Purchase Amount >= 500?}
    C -->|Yes| D[/Display Free Delivery/]
    C -->|No| E[/Display Delivery Charge Applies/]
    D --> F([End])
    E --> F
```

## 12. Employee Salary and Bonus Calculator

Write the algorithm and draw the flowchart for a program that inputs an
employee's monthly salary and years of service, calculates a bonus of
**10%** for employees with 5 or more years of service and **5%** for
others, then displays the bonus and total salary.


### Pseducode

```
START

    INPUT MonthlySalary, YearsOfService

    IF YearsOfService >= 5 THEN
        SET Bonus = MonthlySalary * 0.10
    ELSE
        SET Bonus = MonthlySalary * 0.05
    END IF

    SET TotalSalary = MonthlySalary + Bonus

    DISPLAY Bonus, TotalSalary

END

```
### Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Monthly Salary, Years of Service/]
    B --> C{Years of Service >= 5?}
    C -->|Yes| D[Bonus = Monthly Salary * 0.10]
    C -->|No| E[Bonus = Monthly Salary * 0.05]
    D --> F[Total Salary = Monthly Salary + Bonus]
    E --> F
    F --> G[/Display Bonus, Total Salary/]
    G --> H([End])
```


## 13. Mobile Data Usage Monitor

Write the algorithm and draw the flowchart for a program that inputs a
user's monthly data limit and data usage, then displays whether the user
has exceeded the limit or how much data remains.

### Pseducode

```
START
    INPUT MontlyDataLimit, DataUsage

    IF DataUsage > MonthlyDataLimit THEN
    DISPLAY "Exceeded Limit"
    Else
    SET RemainingData = MonthlyDataLimit -DataUsage
    DISPLAY RamainingData
    ENDIF
END

```

### Flowchart


```mermaid
flowchart TD
    A([Start]) --> B[/Input Monthly Data Limit, Data Usage/]
    B --> C{Data Usage > Monthly Data Limit?}
    C -->|Yes| D[/Display Exceeded Limit/]
    C -->|No| E[Remaining Data = Monthly Data Limit - Data Usage]
    E --> F[/Display Remaining Data/]
    D --> G([End])
    F --> G
```

## 14. Login System (Maximum 3 Attempts)

Create an algorithm and flowchart for a login system that allows a user
up to 3 attempts to enter the correct password. Display **"Access
Granted"** if the password is correct; otherwise display **"Account
Locked"** after 3 failed attempts.

---

### Pseducode

```
START
    SET Attempts = 0
    WHILE Attempts < 3
    INPUT Password
    IF Password = CorrectPassword THEN
    DISPLAY "Access Granted"
    END
    ELSE
    SET Attempts = Attempts + 1
    END IF
    END WHILE
    DISPLAY "Account Locked"
END
```

### flowchart


```mermaid
flowchart TD
    A([Start]) --> B[Set Attempts = 0]
    B --> C{Attempts less than 3?}
    C -->|Yes| D[/Input Password/]
    D --> E{Password correct?}
    E -->|Yes| F[/Display Access Granted/]
    F --> G([End])
    E -->|No| H[Attempts = Attempts + 1]
    H --> C
    C -->|No| I[/Display Account Locked/]
    I --> G
```


## 14. Store Checkout with Multiple Items

Write the algorithm and draw the flowchart for a program that inputs the
number of items purchased, calculates the total purchase amount using a
loop, and applies a **15% discount** if the total exceeds 5000 SEK.

### pseducode

```
START

    INPUT NumberOfItems
    SET Total = 0
    FOR i = 1 TO NumberOfItems
    INPUT Price
    SET Total = Total + Price
    END FOR
    IF Total > 5000 THEN
    SET Discount = Total * 0.15
    SET FinalAmount = Total - Discount
    ELSE
    SET FinalAmount = Total
    END IF
    DISPLAY FinalAmount
    
END
```

### flowchart



```mermaid
flowchart TD
    A([Start]) --> B[/Input NumberOfItems/]
    B --> C[Set Total = 0]
    C --> D[Set i = 1]
    D --> E{i <= NumberOfItems?}
    E -->|Yes| F[/Input Item Price/]
    F --> G[Total = Total + Price]
    G --> H[i = i + 1]
    H --> E
    E -->|No| I{Total > 5000?}
    I -->|Yes| J[Discount = Total * 0.15]
    J --> K[FinalAmount = Total - Discount]
    I -->|No| L[FinalAmount = Total]
    K --> M[/Display FinalAmount/]
    L --> M
    M --> N([End])
```
## 15. Electricity Bill Calculator

Write the algorithm and draw the flowchart for a program that inputs the
number of electricity units consumed and calculates the total bill using
the following rates: first 100 units at 1.5 SEK per unit, next 200
units at 2.0 SEK per unit, and all remaining units at 3.0 SEK per unit.

---
## pseducode

```
START

    INPUT Units
    IF Units <= 100 THEN
    Bill = Units * 1.5
    ELSE IF Units <= 300 THEN
    Bill = (100 * 1.5) + ((Units - 100) * 2.0)
    ELSE
    Bill = (100 * 1.5) + (200 * 2.0) + ((Units - 300) * 3.0)
    END IF
    DISPLAY Bill

END
```

## flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Units/]
    B --> C{Units <= 100?}
    C -->|Yes| D[Bill = Units * 1.5]
    C -->|No| E{Units <= 300?}
    E -->|Yes| F[Bill = 100 * 1.5 + Units - 100 * 2.0]
    E -->|No| G[Bill = 100 * 1.5 + 200 * 2.0 + Units - 300 * 3.0]
    D --> H[/Display Bill/]
    F --> H
    G --> H
    H --> I([End])
```