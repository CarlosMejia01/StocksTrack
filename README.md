# StocksPortfolio

## Description

This project is a backend API built with ASP.NET Core. Its main purpose is to handle user authentication and manage information related to stocks, comments, portfolios. The API allows you to register new users, log in, and perform CRUD (Create, Read, Update, Delete) operations on the associated stocks, comments and portfolios<br>

## Index

- [StocksPortfolio](#stocksportfolio)
  - [Description](#description)
  - [Index](#index)
  - [Technologies used](#technologies-used)
  - [Installation](#installation)
  - [Backend Setup](#backend-setup)
  - [Usage](#usage)
  - [QA Analysis](#qa-analysis)
  - [Contributors](#contributors)
  - [Special thanks](#special-thanks)


## Technologies used

| Frontend   | Backend   | QA & UX/UI |
| ---------- | --------- | ---------- |
|            | .NET      | Postman    |
|            | SqlServer |            |
|            |           |            |



## Installation

1. Clone the repository:

```bash
    git clone git@github.com:CarlosMejia01/StocksTrack.git
   ```

2. Navigate to the project directory:

```bash
    cd api
```

## Backend Setup

Before setting up the backend for the project, ensure you have the following installed:
- [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- [Visual Studio](https://visualstudio.microsoft.com/) or [Visual Studio Code](https://code.visualstudio.com/)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) or another supported database
- [DotnetEf](https://learn.microsoft.com/en-us/ef/core/cli/dotnet)

1. Open the `backend` project in your preferred IDE (Visual Studio or Visual Studio Code).

2. Update the database connection string in `appsettings.json` located in the root directory of the backend project:

   ```json
   {
     "ConnectionStrings": {
       "DefaultConnection": "Data Source=(localdb);Initial Catalog=StocksPortfolioDB;Integrated Security=True;Connect Timeout=30;Encrypt=False;TrustServerCertificate=False;ApplicationIntent=ReadWrite;MultiSubnetFailover=False"
     }
   }

- Make sure the name of the database is *StocksPortfolioDB*

## Running the Backend

**Run the following commands**:

- For the creation of the database and the table.

```bash
  dotnet ef migrations add InitialCreate
  dotnet ef database update
```

**Run the backend project***:
```bash
    dotnet watch run
```

1. Start the backend application by clicking the start button ("Start" or "Run") in your IDE preferably with ([Microsoft-Visual-Studio](https://visualstudio.microsoft.com/)).

2. The backend API will be hosted at `https://localhost:5218/swagger/index.html` or `https://localhost:7283/swagger/index.html` (or another port depending on your configuration).

3. Open your web browser and navigate to `https://localhost:5218/swagger/index.html` or `https://localhost:7283/swagger/index.html` to verify the backend is running correctly. Ensure the page loads without any connection errors or HTTP errors.

4. Perform local testing to confirm that all API functionalities are operational and that endpoints respond correctly to requests.


## Usage

1. Ability to create, login new users.
2. Ability to handled comments.
3. Ability to handled stocks.
4. Ability to have a user portfolios based on comments and stocks.

## QA Analysis

## Contributors 


| Developed Role     | Name and Lastname | Contact/Networks                                                                                                                                                                                                                                                                                                          |
| ------------------ | ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Software Developer | Carlos Mejia      | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/CarlosMejia01) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/carlos-alberto-mejia-perez-683600206) |

## Special thanks

<p>We appreciate your comments and contributions to improve this application</p>
