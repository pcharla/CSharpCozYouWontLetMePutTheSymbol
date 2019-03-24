# CSharpCozYouWontLetMePutTheSymbol
Learning C#

C# VS .NET
Common Language Runtime (CLR)- Runtime enviroment for .NET applications (essentially an app in memeory) - app compiled to Intermediate Language code (IL code) which is independednt of computer(hardware and OS) it is running. IL code to native code of machine in run time--> CLR-- (just in time compilation)
Architecture of .NET applications:
Classes: collaborate with each other in run time and application provides some functionality
Namespaces: container for related classes(way to organize increased number of classes in an application)
and Assemblies:  as namespaces grow we need a way to partition our application (next level to namespaces): assemblu is a container for related namespaces- physically a file on the disk (dll or exe) -  when you compile ur entire application the compiler builds one or more assemblies depending on how you partition ur code.(assembly is single unit of deployment of .NET applications)
C# - programming language
.NET - framework for building applications on the windows
.NET is not limited to C#. There are other languages that target .NET framework to build applications and use the framework (F#, VB.NET)
Componenets of .NET - CLR + CLass Library
console app: learning tool: no GUI
VS - Solution can have one or more projects
Properties->AssemblyInfo(executable): Identification/assembly that will be produced as a result of compiling this application- check it out
Assembly Identification/ Assembly manifest
Refrences: other asemblies a project uses(all part of .NET framework)
app.config-- > xml where we store the configuration of the application (connection strings to the database, other settings)
program.cs- write code
using sttaments to use classes defined in different namespace
run app- CLR executes code in main method
An EXE file represents a program that can be executed. A DLL is a file that includes code that can be re-used across different programs
Primitives:
int Number  = 1;
const float Pi = 3.14f;
camelcase: firstName
pascalcase: FirstName - use it for constants
hungarian notation: strFirstName (don't use)
