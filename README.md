# Comp 170 Assignment Two: Branching and Conditionals

## Due date: February 1, 2022, 6:00pm

### Step One - Fork the repository to your own GitHub space and clone your forked repository - 5 points

First, click the "Fork" button in the upper right-hand corner of the GitHub view.  This will
create a **fork** of this repository in your personal GitHub space.

Second, clone your forked repository.  **Do not clone the original repository!!**  Clone the repository
that you find in your personal space in GitHub.

### Step Two: Run the test Calculate Income Tax using if..else - 30 points

Consider the following table of income tax rate per annual income:

|              Annual Income              | Tax Rate  |
|:---------------------------------------:|:---------:|
|     Portion of income $1 to $20,000     |    10%    |
|  Portion of income $20,001 to $75,000   |    15%    |
|  Portion of income $75,001 to $150,000  |    25%    |
| Portion of income $150,001 to $250,000  |    28%    |
 | Portion of income $250,001 to $500,000  |    33%    |
 | Portion of income $500,001 to $750,000  |    35%    |
 |  Portion of income $750,001 and above   |    37%    |

Note that an individual’s income tax is based on ***portions*** of annual income, each portion
taxed at a different percentage.  For example, if an individual earns $80,000, then that individual’s 
income tax owed would be $11,500, calculated as shown below:

|             Annual Income             |    Tax Rate    | Tax Owed |
|:-------------------------------------:|:--------------:|:-------:|
|    Portion of income $1 to $20,000    | 10% of $20,000 |  $2,000 |
| Portion of income $20,001 to $75,000  | 15% of $55,000 |  $8,250 |
| Portion of income $75,001 to $150,000 | 25% of $5,000  |  $1,250 |
| Portion of income $150,001 to $250,000  |   28% of $0    | $0 |
| Portion of income $250,001 to $500,000  |   33% of $0    | $0 |
| Portion of income $500,001 to $750,000  |   35% of $0    | $0 |
|  Portion of income $750,001 and above   |   37% of $0    | $0 |
|                                       |   **Total**    | $11,500 |

### Step Three: Make the tests pass by implementing the `calculate(..)` method, using an `if..else if..else` block - 30 points

In the codebase you will find a class called `IncomeTaxCalculatorTest`, and another called `IncomeTaxCalculator`.

Open `IncomeTaxCalculatorTest` in IntelliJ and run the tests that it contains.  You will see that they fail, because
they call the method `calculate(..)` on the `IncomeTaxCalculator` class, and this method is not implemented.

Your goal is to make the tests in `IncomeTaxCalculatorTest` pass by adding code into the body of the `calculate(..)` method.
**Use _only_ the if..else (..else if..) branching construct!  Do not use a switch statement here!**

To do this, you should follow this routine:

1. Run the tests, see them fail
2. Add or change a ***small amount*** of code in `IncomeTaxCalculator.calculate(..)`.  You should not change any other code!
3. Run the tests again and decide what ***small*** change to make next
4. Make period commits and push your work in progress

**Notes:** 
* It will help you to work out a few examples on paper, you can start with the values specified in the tests
* You may find zyBook section 2.16 helpful for this part of the assignment

### Deliverable (Total of 35 pts):

* Commit and push your code
* Raise a Pull Request
* Submit a link to your Pull Request in Sakai
