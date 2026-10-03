# Learning C# 14 with .NET 10

📖 **Read the tutorial: [https://stahe.github.io/en-csharp-oct-2026/](https://stahe.github.io/en-csharp-oct-2026/)**

This course teaches the [C#](https://learn.microsoft.com/fr-fr/dotnet/csharp/) 14 language and the [.NET](https://dotnet.microsoft.com) platform 10 **through practical examples**: over two hundred programs (nearly 300 C# files), commented line by line, with their execution results reproduced. It starts with the basics of the language and covers database access, network programming, and web services.

This is a rewrite, for C# 14 and .NET 10, of the course [Learning the C# Language, Version 3.0, with the .NET 3.5 Framework](https://stahe.github.io/en-csharp-mai-2008/) (2008): same outline, same examples, same overarching theme, but with up-to-date code. All programs compile **without errors or warnings** using the .NET 10 SDK and have been run; the results shown in the course are those of these runs.

| C# 3.0 Course (2008) | C# 14 Course (2026) |
|---|---|
| C# 3.0, .NET 3.5 framework, Windows only | C# 14, .NET 10 (LTS), Windows, Linux, macOS |
| Visual C# 2008 Express | VS Code + C# Dev Kit or Visual Studio 2026, `dotnet` command |
| `.sln` projects and solutions | single-file applications (`dotnet run prog.cs`), `.slnx` solutions |
| Windows Forms graphical user interfaces | chapter removed (interfaces are now web-based) |
| LINQ “not covered” | LINQ covered in detail |
| `ArrayList`, `Hashtable`, `BinaryFormatter` | generic collections, `System.Text.Json` |
| NUnit 2.4, Spring.NET | MSTest 4, Microsoft.Extensions.DependencyInjection |
| `BackgroundWorker`, `BeginXxx` / `EndXxx` pattern | `Task`, `async` / `await`, cancellation, `IAsyncEnumerable` |
| SQL Server 2005, ODBC, OLE DB | MySQL 8 (Laragon), MySqlConnector, Entity Framework Core |
| `WebClient`, `WebRequest` | Asynchronous `HttpClient`, `TcpClient` / `TcpListener` |
| SOAP ASMX web services | REST / JSON web services with ASP.NET Core Minimal API |

## Course Outline

| Chapter | Content |
|---|---|
| Installation | .NET 10 SDK, VS Code / Visual Studio 2026, the `dotnet` command, single-file applications, projects, `.slnx` solutions |
| Language Basics | types, literals, nullable types, conversions, arrays, indexes and ranges, operators (`??`, `??=`), `switch` expressions and pattern matching, exceptions, enumerations, parameter passing, local functions, tuples |
| Classes, Structures, Interfaces | properties (`init`, `required`, the C# 14 `field` keyword), inheritance, polymorphism, operators, indexers, structures, interfaces, generics, records, primary constructors, C# 14 extension members, nullable reference types |
| Commonly Used .NET Classes | strings, arrays, collections, **LINQ**, text and binary files, JSON, regular expressions (`[GeneratedRegex]`) |
| Layered Architectures | [DAO] / [business] / [UI] layers, **MSTest** unit tests, **dependency injection** |
| Delegates, lambdas, and events | `Func`, `Action`, lambda expressions, closures, events, expression trees |
| Execution threads | `Thread`, synchronization (C# 13 `Lock`, `Monitor`, `Interlocked`…), concurrent collections, `Parallel` |
| **Asynchronous programming** (new) | `Task`, `async` / `await`, `WhenAll`, cancellation, progress, asynchronous streams, `Parallel.ForEachAsync`, `Channel<T>` |
| Database access with ADO.NET | MySQL, `MySqlConnector`, parameterized queries and SQL injection, transactions, asynchronous methods, `DbProviderFactory` |
| **Entity Framework Core** (new) | model, CRUD, LINQ-to-SQL, relationships, migrations, optimistic concurrency, raw SQL, dependency injection |
| Web Programming | TCP/IP, IPv6, asynchronous TCP clients and servers, HTTP, `HttpClient`, SMTP |
| Web Services | REST / JSON with ASP.NET Core Minimal API, console clients, JavaScript web client |

## The Common Thread: An Income Tax Calculator in 9 Versions

Throughout the course, version by version, we build an **income tax calculator** application:

- **version 1**: a single program; **version 2**: classes and interfaces; **version 3**: data read from a text or JSON file;
- **versions 4 and 5**: a layered architecture, tested with MSTest and integrated via dependency injection;
- **versions 6 and 7**: data in a MySQL database, read using ADO.NET and then Entity Framework Core;
- **version 8**: a TCP server for tax calculation and its client;
- **version 9**: a REST web service, its console client, and its web client.

## Technologies

C# 14 · .NET 10 · VS Code · Visual Studio 2026 · MSTest 4 · Microsoft.Extensions.DependencyInjection · System.Text.Json · MySQL 8 · MySqlConnector · Entity Framework Core 9 · Pomelo.EntityFrameworkCore.MySql · ASP.NET Core 10 · Laragon

## Prerequisites

- Previous programming experience in any language.
- The [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) and a code editor ([VS Code](https://code.visualstudio.com) with the C# Dev Kit extension, or Visual Studio 2026); [Laragon](https://laragon.org) for MySQL (chapters on databases). Installation instructions are provided in the course.

## Author

This course and its code were written by **Claude**, the AI from [Anthropic](https://www.anthropic.com) (October 2026), at the request of Serge Tahé, based on his 2008 C# course.

Reviewer: [Serge Tahé](https://stahe.github.io)
