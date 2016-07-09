---
title: dotnet-new
description: dotnet-new
keywords: .NET, .NET Core
author: mairaw
manager: wpickett
ms.date: 06/20/2016
ms.topic: article
ms.prod: .net-core
ms.technology: .net-core-technologies
ms.devlang: dotnet
ms.assetid: 263c3d05-3a47-46a6-8023-3ca16b488410
---

dotnet-new
==========

## NAME
dotnet-new -- Creates a new .NET Core project

## SYNOPSIS
`dotnet new [--type] [--lang]`

## DESCRIPTION
The `dotnet new` command provides a convenient way to initialize a valid .NET Core project and sample source code to try out the Command Line Interface (CLI) toolset. 

This command is invoked in the context of a directory. When invoked, the command will result in two main artifacts being dropped to the directory: 

1. A `Program.cs` (or `Program.fs`) file that contains a sample "Hello World" program.
2. A valid `project.json` file.

After this, the project is ready to be compiled and/or edited further. 

## Options

`-l`, `--lang [C#|F#]`

Language of the project. Defaults to `C#`. `csharp` (`fsharp`) or `cs` (`fs`) are also valid options.

`-t`, `--type`

Type of the project. Valid values are `console`, `web`, `lib` and `xunittest`. 

## EXAMPLES

`dotnet new`
    
Drops a C# project in the current directory.

`dotnet new --lang f#`
    
Drops an F# project in the current directory.

`dotnet new --lang c#`
    
Drops an C# project in the current directory.

`dotnet new -t web`
    
Drops a new ASP.NET Core project in the current directory. 
