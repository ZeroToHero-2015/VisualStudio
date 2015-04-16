# Despre Visual Studio & alte unelte

## De bază

- folosim Visual Studio 2013 Community Edition (bun & gratis)

- e important să învățați [shortcut-uri][shortcut], eventual [gamificat][foo]

- arătat fereastră New Project (`ctrl-shift-N`)

    + versiuni de framework
    + template-uri: Windows Desktop, Web
    + project: iese un executabil sau dll (de cele mai multe ori)
    + soluție: colecție de proiecte
    + Name, Location, Solution Name, Create directory for solution, Add to
      source control

- creat HelloWorld
  ![New Project][newProject]

- cum arată Solution Explorer (`ctrl-W ctrl-S`)
  ![Solution Explorer][solutionExplorer]
    + `AssemblyInfo.cs`
    + References
    + Fișiere sursă
    + Adăugat clasă cu `shift-alt-C`

- pluginuri, mai ales ReSharper

- `Program.Main()` echivalent cu `main()` din C (dar args nu conține numele
  programului)

- `Console.WriteLine(...)` e printf

## run & debug

- Build: build solution (`F6` sau `ctrl-shift-B`); build current project
  (`shift-F6` sau altceva)

- Run: `F5`; de ce nu vedem nimic?

- Start debugging, start without debugging (`ctrl-F5`)

- Add breakpoint: `F9`

- Step: `F10`, step into: `F11`

- build în linia de comandă: `Developer Tools`, `msbuild *.csproj`

- `/t:Clean` etc.

## nuget

- managementul dependințelor (versiuni etc.)

- ![Manage NuGet Packages][nuget]

- install package:
    + `packages.config`
    + adăugat referința
    + `packages`

- pachetele for avea la rîndul lor dependințe

[shortcut]: http://visualstudioshortcuts.com/2013/
[foo]:      https://www.shortcutfoo.com/app/dojos/microsoft-visual-studio-win

[newProject]:       NewProject.png       "Fereastra New Project"
[solutionExplorer]: SolutionExplorer.png "Solution Explorer (ctrl-W ctrl-S)"
[nuget]:            ManageNugetPackages.png "Manage NuGet Packages"