# Library App

## Description

Library App is a console-based library management system. It allows users to manage patrons, books, and loans through a simple console interface. The application is built using .NET 8.0 and follows a clean architecture with separate layers for application core, infrastructure, and console interface.

## Project Structure

- `AccelerateDevGitHubCopilot.sln`
- `src/`
  - `Library.ApplicationCore/`
    - `Entities/`
    - `Enums/`
    - `Interfaces/`
    - `Services/`
    - `Library.ApplicationCore.csproj`
  - `Library.Console/`
    - `appSettings.json`
    - `CommonActions.cs`
    - `ConsoleApp.cs`
    - `ConsoleState.cs`
    - `Json/`
    - `Library.Console.csproj`
    - `Program.cs`
  - `Library.Infrastructure/`
    - `Data/`
    - `Library.Infrastructure.csproj`
- `tests/`
  - `UnitTests/`
    - `ApplicationCore/`
    - `UnitTests.csproj`

## Key Classes and Interfaces

- **Library.ApplicationCore**
  - `Entities/`
    - `Author`
    - `Book`
    - `BookItem`
    - `Patron`
    - `Loan`
  - `Enums/`
    - `CommonActions`
    - `ConsoleState`
  - `Interfaces/`
    - `IPatronRepository`
    - `ILoanRepository`
    - `ILoanService`
    - `IPatronService`
  - `Services/`
    - `LoanService`
    - `PatronService`

- **Library.Console**
  - `ConsoleApp`
  - `CommonActions`
  - `ConsoleState`
  - `Program`

- **Library.Infrastructure**
  - `Data/`
    - `JsonData`
    - `JsonPatronRepository`
    - `JsonLoanRepository`

## Usage Instructions

1. **Clone the repository**:

   ```sh
   git clone https://github.com/yourusername/LibraryApp.git
   cd LibraryApp