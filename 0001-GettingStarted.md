# Getting Started #  

## Your first task will be to get your computer setup for the term ##
The following document will help you get setup to succeed for the term.  In order to do this, you will need to have your machine configured.  As a computer science student, and eventual professional, it is expected that you would know how to get and install programs, run, and use programs.  

This guide will help you to learn how to work with those tools, as well as help you to know what to set up and how to proceed with getting started, so that you are not 100% lost from day one.

## Expectations ##  
It is not expected that you would know what to do or how to do it right away.  This is the purpose of learning.  However, if you can't get a program to install and run, then you are in for a very long term, and and even longer career.  Of course there are issues, and things happen, and when they arise we can troubleshoot them.  In the end, however, if you can't get a free tool to install and run for weeks on end, you aren't going to do well in the term.  It is not a valid excuse to say "My SQL Server won't install" for 7 weeks.  

## Tools That you will Need##  
In order to make the system work, you are going to need a number of tools.  They are listed below.  With each tool, it is expected you would install the tool and validate that it works by running it to see that it runs without issue (even if you don't know what to do with it).  

1. GIT.  
	
    The main thing you need from GIT is just to have it installed on your machine.  That being said, it offers a powerful BASH tool that works great when running GIT commands.  BASH is especially handy if you are used to Linux and are working on a Windows box.

    [Get GIT Download](https://git-scm.com/downloads)  

2. Powershell [version 7].

    Powershell is built into Windows.  If you are not on a windows box, you don't need powershell as you have a terminal.  In the end, the **main** thing you need here is a tool that lets you run NPM [Node] and YARN commands.

    [Get Powershell Download](https://github.com/PowerShell/PowerShell/releases/tag/v7.0.3)  

3. Node JS.

    In order to work on the front-end, you will need to get Node.js installed on your machine, specifically so that you have the ability to run NPM commands.  Make sure to get the latest LTS version (NOT the current version with latest features, use the LTS version only).

    [Get Node.js Latest LTS Download](https://nodejs.org/en/)  

4. Visual Studio Community.  

    In order to do the C#.Net work, you will need Visual Studio Community (VSC).  VSC is free for learning and developing non commercial or opensource work.  The tool provides all the stuff you will need free of charge in order to work with C#.Net and the .Net Ecosystem.  Additionally, VSC has some very nice built-in tools for working with GIT.  We will also install some essential extensions to aid in your work.  

    Extensions are nice, but not required.  I recommend three extensions:  

    -    AddFile [Mads Kristensen]  
    -    Open In Command [Mads Kristensen]  
    -    Open in Visual Studio Code [Mads Kristensen]  

    [Get Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)  

5. Visual Studio Code.  

    When you are working on the front-end [Angular] side of the application, you will want to make sure that you are using Visual Studio Code.  The capabilities of Code are great and it's got the ability to do some things like built-in terminals that aid in your front-end work.  

    Extensions here are also recommended:  

    -    GitLens
    -    JSON tools
    -    XML Tools

    For windows users, make sure to get the `System Installer`.  I also recommend you allow adding to `PATH` as well as making sure to allow `Open With` commands in your shell.

    [Use the System Installer on Windows, or the correct installer for your linux/mac machine](https://code.visualstudio.com/Download#)  

6.  Sql Server Developer Edition.

    This is the database that you will use to store all of your data for the solution.  You can likely get by with SQLExpress, but SQLDeveloper is recommended and using it will mean you shouldn't have to make any changes to the connection string.  

    Look for the `Developer` download under the `Or, download a free specialized version`:  

    [Scroll down a bit to get the Developer Download](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)  

7.  Sql Server Management Studio.  

    This tool is how you can easily view your database.  You don't actually need it, but you will likely want it.  

    [Download SSMS](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15)  

8.  YARN.  

    You don't actually need `Yarn`, but it is an extremely useful tool for getting node packages.

    [Download YARN here](https://classic.yarnpkg.com/en/)  

    
## Final Thoughts ##  

Ok, that is a LOT of tools.  Yes, it is, but each has a highly useful purpose, and each will aid you in some part of the development lifecycle.  The truth is you can pretty much do everything in Visual Studio, but it is not as useful and easy to do, so it's better to set your machine, and you, up for success.

An additional final thought.  Powershell and/or Yarn might ask you to install [Chocolatey](https://chocolatey.org/).  If they do, you will find it is also a nice tool for installing programs on Windows.

Please do not hesitate to reach out if you get stuck or have any questions.  I promise this initial setup will be worth it to you in the long run.

## Next Steps ##

After getting all the tools set up and working on your machine, you are ready to move to the next task: `Getting the project up and running`.  
    