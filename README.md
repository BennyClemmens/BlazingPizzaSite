# BlazorPizzaSite

Folowing the tutorial at <https://learn.microsoft.com/en-us/training/modules/interact-with-data-blazor-web-apps/2-create-user-interfaces-with-blazor-components>

## Repo and project creation

```bash
Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP
$ dotnet new blazorserver -o BlazingPizzaSite
No templates or subcommands found matching: 'blazorserver'.

To list installed templates similar to 'blazorserver', run:
   dotnet new list blazorserver
To search for the templates on NuGet.org, run:
   dotnet new search blazorserver


For details on the exit code, refer to https://aka.ms/templating-exit-codes#103

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP
$ dotnet new list blazorserver
No templates found matching: 'blazorserver'.

To search for the templates on NuGet.org, run:
   dotnet new search blazorserver


For details on the exit code, refer to https://aka.ms/templating-exit-codes#103

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP
$ dotnet new search blazorserver
Searching for the templates...
Matches from template source: NuGet.org
These templates matched your input: 'blazorserver'

Template Name                                 Short Name                        Language  Package Name / Owners                                         Trusted  Downloads
--------------------------------------------  --------------------------------  --------  ------------------------------------------------------------  -------  ---------
DevExpress Blazor Server Reporting Project    dx.blazor.reporting.blazorserver  [C#]      DevExpress.DotNet.Web.ProjectTemplates / devexpress              ✓        150k
Blazor Server App (minimum)                   blazorservermin                   [C#]      Toolbelt.AspNetCore.Blazor.Minimum.Templates / jsakamoto                  67k
Blazor Server App (Microsoft identity pla...  blazorserver2                     [C#]      Microsoft.Identity.Web.ProjectTemplates / AzureAD, Microsoft     ✓        49k
FluentUI Blazor Server App                    fluentuiblazorserver              [C#]      Microsoft.Fast.Templates.FluentUI / fast, Microsoft              ✓        38k
bit BlazorServer                              bit-ssb                           [C#]      Bit.BlazorServer / bit-foundation                                         29k
Auth0 Blazor Server App                       auth0blazorserver                 [C#]      Auth0.Templates / auth0                                          ✓        13k
Clean Blazor Server App                       cleanblazorserver                 [C#]      FriscoVInc.DotNet.Templates.CleanBlazor / friscov                ✓        13k
Clean Architecture for Blazor Server Solu...  ca-blazorserver-sln               [C#]      CleanArchitecture.Blazor.Solution.Template / neozhu                        5k
Blazor Server App                             blazorserver                      F#        FSharp.Blazor.Templates / reaptor                                          4k
EC.Dataverse.Web.BlazorServer                 EC.Dataverse.Web.BlazorServer     [C#]      EC.ProjectTemplates / charles.kuperus                                      4k
Blazor Server Tailwind Project Template       blazorservertw                    [C#]      PracticalDotNet.TailwindStarterProject / jonhilt                           3k
Blazor Serverside + Tailwind CSS              blazorservertailwind              [C#]      Cethien.Templates / cethien                                                3k
MudBlazor Server Application                  mudblazorserver                   [C#]      GeekHour.AspNetCore.MudBlazor.Templates / GeekHour                         2k
Clean Architecture Template - Blazor Server   cleanarch-blazorserver            [C#]      CleanArch.Templates / netcodr                                              1k
FusionAuth ASP.NET Core Blazor Server App     fusionauthblazorserver            [C#]      FusionAuth.Templates / FusionAuth                                         <1k
Telerik Blazor Server App                     dimodi-blazorserver               [C#]      Dimodi.Telerik.Blazor.Templates / dimodi                                  <1k


To use the template, run the following command to install the package:
   dotnet new install [<package>...]
Example:
   dotnet new install Microsoft.Identity.Web.ProjectTemplates

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP
$ dotnet new install Microsoft.Identity.Web.ProjectTemplates
The following template packages will be installed:
   Microsoft.Identity.Web.ProjectTemplates

Success: Microsoft.Identity.Web.ProjectTemplates::1.26.0 installed the following templates:
Template Name                                                              Short Name      Language  Tags
-------------------------------------------------------------------------  --------------  --------  ------------------------
ASP.NET Core Web API (Microsoft.Identity.Platform)                         webapi2         [C#]      Web/WebAPI
ASP.NET Core Web App (Microsoft identity platform)                         webapp2,razor2  [C#]      Web/MVC/Razor Pages
ASP.NET Core Web App (Model-View-Controller, Microsoft identity platform)  mvc2            [C#]      Web/MVC
Azure Functions                                                            func2           [C#]      Azure Functions/Solution
Blazor Server App (Microsoft identity platform)                            blazorserver2   [C#]      Web/Blazor
Blazor WebAssembly App                                                     blazorwasm2     [C#]      Web/Blazor/WebAssembly
Worker Service                                                             worker2         [C#]      Common/Worker/Web


Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP
$ dotnet new blazorserver2 -o BlazingPizzaSite
The template "Blazor Server App (Microsoft identity platform)" was created successfully.
This template contains technologies from parties other than Microsoft, see https://aka.ms/aspnetcore/5.0-third-party-notices for details.

Processing post-creation actions...
Restoring C:\DATA\GIT\CSHARP\BlazingPizzaSite\BlazingPizzaSite.csproj:
  Determining projects to restore...
C:\Program Files\dotnet\sdk\8.0.403\Sdks\Microsoft.NET.Sdk\targets\Microsoft.NET.EolTargetFrameworks.targets(32,5): warning NETSDK1138: The target framework 'netcoreapp3.
1' is out of support and will not receive security updates in the future. Please refer to https://aka.ms/dotnet-core-support for more information about the support policy
. [C:\DATA\GIT\CSHARP\BlazingPizzaSite\BlazingPizzaSite.csproj]
C:\Program Files\dotnet\sdk\8.0.403\Sdks\Microsoft.NET.Sdk\targets\Microsoft.NET.EolTargetFrameworks.targets(32,5): warning NETSDK1138: The target framework 'netcoreapp3.
1' is out of support and will not receive security updates in the future. Please refer to https://aka.ms/dotnet-core-support for more information about the support policy
. [C:\DATA\GIT\CSHARP\BlazingPizzaSite\BlazingPizzaSite.csproj]
  Restored C:\DATA\GIT\CSHARP\BlazingPizzaSite\BlazingPizzaSite.csproj (in 10,29 sec).
Restore succeeded.



Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP
$ cd BlazingPizzaSite/

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP/BlazingPizzaSite
$ ls
_Imports.razor  appsettings.Development.json  BlazingPizzaSite.csproj  obj/    Program.cs   Shared/     wwwroot/
App.razor       appsettings.json              Data/                    Pages/  Properties/  Startup.cs

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP/BlazingPizzaSite
$ git init
Initialized empty Git repository in C:/DATA/GIT/CSHARP/BlazingPizzaSite/.git/

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP/BlazingPizzaSite (main)
$ git add .
warning: in the working copy of 'App.razor', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'BlazingPizzaSite.csproj', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Data/WeatherForecast.cs', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Data/WeatherForecastService.cs', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Pages/Counter.razor', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Pages/Error.cshtml', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Pages/FetchData.razor', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Pages/Index.razor', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Pages/_Host.cshtml', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Program.cs', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Properties/launchSettings.json', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Shared/MainLayout.razor', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Shared/NavMenu.razor', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Shared/SurveyPrompt.razor', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'Startup.cs', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of '_Imports.razor', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'appsettings.Development.json', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'appsettings.json', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'obj/BlazingPizzaSite.csproj.nuget.dgspec.json', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'obj/BlazingPizzaSite.csproj.nuget.g.props', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'obj/BlazingPizzaSite.csproj.nuget.g.targets', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'obj/project.assets.json', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'obj/project.nuget.cache', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'wwwroot/css/bootstrap/bootstrap.min.css', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'wwwroot/css/open-iconic/FONT-LICENSE', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'wwwroot/css/open-iconic/ICON-LICENSE', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'wwwroot/css/open-iconic/README.md', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'wwwroot/css/open-iconic/font/fonts/open-iconic.svg', CRLF will be replaced by LF the next time Git touches it
warning: in the working copy of 'wwwroot/css/site.css', CRLF will be replaced by LF the next time Git touches it

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP/BlazingPizzaSite (main)
$ git commit -m 'initial commit BlazingPizzaSite'
[main (root-commit) cf36113] initial commit BlazingPizzaSite
 36 files changed, 4279 insertions(+)
 create mode 100644 App.razor
 create mode 100644 BlazingPizzaSite.csproj
 create mode 100644 Data/WeatherForecast.cs
 create mode 100644 Data/WeatherForecastService.cs
 create mode 100644 Pages/Counter.razor
 create mode 100644 Pages/Error.cshtml
 create mode 100644 Pages/FetchData.razor
 create mode 100644 Pages/Index.razor
 create mode 100644 Pages/_Host.cshtml
 create mode 100644 Program.cs
 create mode 100644 Properties/launchSettings.json
 create mode 100644 Shared/MainLayout.razor
 create mode 100644 Shared/NavMenu.razor
 create mode 100644 Shared/SurveyPrompt.razor
 create mode 100644 Startup.cs
 create mode 100644 _Imports.razor
 create mode 100644 appsettings.Development.json
 create mode 100644 appsettings.json
 create mode 100644 obj/BlazingPizzaSite.csproj.nuget.dgspec.json
 create mode 100644 obj/BlazingPizzaSite.csproj.nuget.g.props
 create mode 100644 obj/BlazingPizzaSite.csproj.nuget.g.targets
 create mode 100644 obj/project.assets.json
 create mode 100644 obj/project.nuget.cache
 create mode 100644 wwwroot/css/bootstrap/bootstrap.min.css
 create mode 100644 wwwroot/css/bootstrap/bootstrap.min.css.map
 create mode 100644 wwwroot/css/open-iconic/FONT-LICENSE
 create mode 100644 wwwroot/css/open-iconic/ICON-LICENSE
 create mode 100644 wwwroot/css/open-iconic/README.md
 create mode 100644 wwwroot/css/open-iconic/font/css/open-iconic-bootstrap.min.css
 create mode 100644 wwwroot/css/open-iconic/font/fonts/open-iconic.eot
 create mode 100644 wwwroot/css/open-iconic/font/fonts/open-iconic.otf
 create mode 100644 wwwroot/css/open-iconic/font/fonts/open-iconic.svg
 create mode 100644 wwwroot/css/open-iconic/font/fonts/open-iconic.ttf
 create mode 100644 wwwroot/css/open-iconic/font/fonts/open-iconic.woff
 create mode 100644 wwwroot/css/site.css
 create mode 100644 wwwroot/favicon.ico

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP/BlazingPizzaSite (main)
$ git branch -M main

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP/BlazingPizzaSite (main)
$ git remote add origin https://github.com/BennyClemmens/BlazingPizzaSite.git

Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP/BlazingPizzaSite (main)
$ git push -u origin main
Enumerating objects: 50, done.
Counting objects: 100% (50/50), done.
Delta compression using up to 8 threads
Compressing objects: 100% (49/49), done.
Writing objects: 100% (50/50), 223.45 KiB | 6.77 MiB/s, done.
Total 50 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/BennyClemmens/BlazingPizzaSite.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
```

### Create Blazor components

Note: the app was allready created in the previous step.

```bash
Benny@FLAB2021 MINGW64 /c/DATA/GIT/CSHARP/BlazingPizzaSite (main)
$ dotnet new razorcomponent -n PizzaBrowser -o Pages
The template "Razor Component" was created successfully.
```
