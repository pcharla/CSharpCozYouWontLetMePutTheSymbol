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
https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/built-in-types-table
double -default type for real numbers
float number  = 1.2f; --> f=> treat this number as  a flota and not double
decimal number  = 1.2m;
Non Primitive: 
String
Array
Enum
Class
overflowing: exceeding the boundary memory capabilities of datatypes, in C# by default we do not have overflow check

checked //overflow will not happen but exception will be thrown which we can handle
{
byte number = 255;
number += 1;
}
Scope: where a constant or variable has meaning or is accessible

before accesing  a varibale declare it and set (initialize/assign) it
character :  single quotes, string : double quotes
if yo have to use reserved words for anything use @ before that and use it like @int
declaring with var keyborad lets compiler decide and tel what kind of datatype it is

Struct: 

Type conversion:
Implicit: byte b = 1; int i =b; (no data loss and types are compatible)
in cas of data loss:
int i;
byte b= (byte) i ; //casting, does conversion anyway despite data loss
Explicit(casting)

conversion between non-compatible types:
string and int for example
str t = "123"
int i = (int) t // wont work coz of non-compatible types
so int i  = convert.Toint32(t)
int i = int.parse(t)
Operators:

Arithmatic:
Comparison:
Assignment:
Logical: &&, ||, !
Bitwise: &, | --> lower level programing -like working with windows API, SOCKETS, encryption

use IS/HAS for boolean result names

floating division with integers: cast them : (float) a/ (float) b;


comments to explain whys, hows, constraints etc not the whats
C# is a statically typed language: once you delare a variable, u nned to specify its type (that type cannot change during the lifetime of that variable)







