🧮 Arithmetic Operations Console App in C# (.NET)

A structured C# console application that performs fundamental arithmetic operations including:

➕ Addition

➖ Subtraction

✖ Multiplication

➗ Division

🧮 Modulus

⚠ Safe division check (division-by-zero prevention)

This project demonstrates core C# programming concepts, .NET CLI project setup, and solution-based structure with unit testing support.

📂 Project Structure
SimpleAdditionOOP/
│
├── src/
│   └── SimpleAdditionOOP/
│       └── Program.cs
│
├── tests/
│   └── SimpleAdditionOOP.Tests/
│
└── SimpleAdditionOOP.sln

⚙️ How to Set Up This Project

Follow these steps using the .NET CLI:

1️⃣ Create the Solution
dotnet new sln -n SimpleAdditionOOP

2️⃣ Create the Console Application
dotnet new console -n SimpleAdditionOOP -o src/SimpleAdditionOOP


Replace the generated Program.cs file with your arithmetic operations code.

3️⃣ Create the Test Project (xUnit)
dotnet new xunit -n SimpleAdditionOOP.Tests -o tests/SimpleAdditionOOP.Tests

4️⃣ Add Projects to the Solution
dotnet sln add src/SimpleAdditionOOP/SimpleAdditionOOP.csproj
dotnet sln add tests/SimpleAdditionOOP.Tests/SimpleAdditionOOP.Tests.csproj
dotnet add tests/SimpleAdditionOOP.Tests/SimpleAdditionOOP.Tests.csproj reference src/SimpleAdditionOOP/SimpleAdditionOOP.csproj

5️⃣ Restore, Build & Run Tests
dotnet restore
dotnet build
dotnet test


To run the application:

dotnet run --project src/SimpleAdditionOOP

📊 Sample Output
This is Addition 30
The subtraction is -10
The Multiplication is 200
The division is 0
Safe Division Result: 0
Modulus Result: 10

🧠 Concepts Demonstrated

C# Console Application development

Arithmetic Operators: +, -, *, /, %

Conditional Statements (if-else)

Division-by-zero prevention

.NET CLI workflow

Solution-based project structure

Basic unit test integration with xUnit

📈 Future Improvements

Accept dynamic user input using Console.ReadLine()

Refactor into a reusable Calculator class (stronger OOP design)

Add unit tests for each arithmetic operation

Implement structured exception handling

Add input validation for robust CLI behavior

🛠 Technologies Used

C#

.NET SDK

.NET CLI

xUnit Testing Framework
