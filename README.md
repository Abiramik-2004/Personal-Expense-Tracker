# Personal Finance Tracker – ASP.NET Core MVC

A web-based Personal Finance Tracker developed using ASP.NET Core MVC to help users manage their income, expenses, and financial transactions. The application provides an organized way to track financial activities, manage categories, and monitor personal finances through a simple and responsive interface.

## Features

- **Transaction Management:** Create, view, update, and delete income and expense transactions.
- **Category Management:** Organize financial transactions using customizable categories.
- **Dashboard:** View financial summaries and transaction overviews.
- **User Authentication:** User registration and login functionality.
- **Account Management:** Manage personal account information and settings.
- **Responsive UI:** User-friendly interface for different screen sizes.
- **Data Management:** Store and retrieve financial records using SQL Server.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | C# |
| Framework | ASP.NET Core MVC (.NET 9) |
| Database | Microsoft SQL Server |
| ORM | Entity Framework Core |
| Authentication | ASP.NET Core Identity |
| Frontend | HTML5, CSS3, Bootstrap, JavaScript |
| Architecture | MVC, Repository Pattern, Service Layer |
| Database Management | Code First Migrations |

## Project Architecture

The application follows a layered architecture to maintain separation of concerns, code reusability, and maintainability.

```text
PersonalFinanceTracker/
│
├── Controllers/
│   └── Handles HTTP requests and application flow
│
├── Models/
│   └── Defines application data models
│
├── Views/
│   └── Contains Razor UI pages
│
├── Services/
│   └── Implements business logic
│
├── Repository/
│   └── Handles database operations
│
├── Interface/
│   └── Contains service and repository contracts
│
├── Data/
│   └── Contains Entity Framework DbContext
│
├── wwwroot/
│   └── Contains CSS, JavaScript and static assets
│
├── appsettings.json
│   └── Application configuration
│
└── Program.cs
    └── Application configuration and startup
```

## Database Design

The application uses Microsoft SQL Server for persistent data storage.

**Core Entities:**

- **Users:** Stores user account and authentication-related information.
- **Transactions:** Stores income and expense transaction details.
- **Categories:** Organizes transactions into different categories.
- **Accounts:** Maintains user account information.

Entity Framework Core is used to manage database operations and relationships between entities.

## Security

- User authentication and authorization using ASP.NET Core Identity.
- Secure password hashing.
- Input validation.
- CSRF protection using anti-forgery tokens.
- User session management.

## Prerequisites

Before running the application, install:

- [.NET 9 SDK](https://dotnet.microsoft.com/download/dotnet/9.0)
- [Microsoft SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- [Visual Studio 2022](https://visualstudio.microsoft.com/) or [Visual Studio Code](https://code.visualstudio.com/)

## Installation and Setup

**1. Clone the repository**

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd PersonalFinanceTracker
```

**2. Configure the database**

Update the connection string in `appsettings.json`:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=(localdb)\\MSSQLLocalDB;Database=PersonalFinanceTrackerDb;Trusted_Connection=True;MultipleActiveResultSets=true"
  }
}
```

Update the server details according to your SQL Server installation.

**3. Restore dependencies**

```bash
dotnet restore
```

**4. Install Entity Framework Core CLI (if not already installed)**

```bash
dotnet tool install --global dotnet-ef
```

**5. Apply database migrations**

```bash
dotnet ef database update
```

**6. Run the application**

```bash
dotnet run
```

**7. Open the application**

Use the local URL displayed in your terminal, usually:

```text
https://localhost:xxxx
```

## Future Enhancements

- Financial reports and analytics.
- Monthly and yearly budget planning.
- PDF and Excel report exports.
- Multi-currency support.
- Advanced financial dashboards.
- Automated financial insights.

## Learning Outcomes

Through this project, I explore and apply:

- ASP.NET Core MVC application development.
- C# programming and Object-Oriented Programming concepts.
- Entity Framework Core and database operations.
- SQL Server integration.
- Authentication and authorization.
- Repository Pattern and layered architecture.
- Responsive frontend development.
- Database migrations and application configuration.

## Author

**Abirami Kanthasamy**

Computer Science and Engineering Graduate

[GitHub](https://github.com/Abiramik-2004) | [LinkedIn](https://www.linkedin.com/in/abirami-kanthasamy/)

---

⭐ If you find this project useful, feel free to explore the repository and share your feedback.
