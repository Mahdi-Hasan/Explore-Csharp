The book i am following:
**C# 8 Quick Syntax Reference**
Author: **Mikael Olsson**

# Introduction
The C# programming language is an object-oriented language created by
Microsoft for the .NET Framework. It is a general-purpose
programming language, so it is useful for creating a wide range of
programs. Everything from small utilities to computer games, desktop
applications, or even operating systems can be built in C#. The language
can also be used with ASP.NET to create web-based applications.

# CHAPTER 1 Hello World
wanna print on the console :
```c#
System.Console.WriteLine("Hello World");
```
# Chapter 2 Compile and Run

Main(): signaling the default entry point of execution
source code: .cs file -> Compile -> Assembly
Assembly:
	unit of packaging and deployment in .NET, 
	.exe: with entry point(executable)
	.dll: whitout entry point(library)

C# compiler: csc.exe (%SystemRoot%\Microsoft.NET\Framework\<framework-version>)

csc MyProgram.cs -> MyProgram.exe
csc /target:library MyProgram -> MyProgram.dll

From <https://github.com/monoshade/C-Sharp/blob/master/2-Basics/1-Compile.txt> 
## commenting
``
// single-line comment
``
`
/* multi-line
comment */
`
# Chapter 3 Variable

**Int**
##### Declare and Assignment
int myInt = 10, myInt2 = 20, myInt3;
```c#
// Signed integers
sbyte myInt8 = 2; // -128 to +127
short myInt16 = 1; // -32768 to +32767
int myInt32 = 0; // -2^31 to +2^31-1
long myInt64 =-1; // -2^63 to +2^63-1
```
```c#
// Unsigned integers
byte uInt8 = 0; // 0 to 255
ushort uInt16 = 1; // 0 to 65535
uint uInt32 = 2; // 0 to 2^32-1
ulong uInt64 = 3; // 0 to 2^64-1
```

```c#
int myHex = 0xF; // 15 in hexadecimal (base 16)
int myBin = 0b0100; // 4 in binary (base 2)
```
Float
```
float myFloat = 3.14F; // 7 digits of precision
double myDouble = 3.14; // 15-16 digits of precision
decimal myDecimal = 3.14M; // 28-29 digits of precision
```
```
// explicit cast
myFloat = (float) myDecimal; 
```
**exponential notation:**
``
myDouble = 3e2;
``
