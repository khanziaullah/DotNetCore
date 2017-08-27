# DotNetCore


.Net Core is platform independent .Net. It can run on:
	• Windows
	• Linux, and
	• Mac
	• Android (I assume).

I am running .Net Core 2.0 and its installation/configuration has improved since .Net Core 1.0.
It comes with Visual Studio 2017.
For other platforms the steps are straight forward and goes like this:

	• Configure the OS (Linux/Mac) to know the package source for .Net Core
	• Use the appropriate installation tool (apt-get for Linux) to request an install
	• Use the .Net Core tooling to create and run projects

Here is the sequence I followed for Hello World

	• dotnet new Console
		○ This created a hello world console project for me with the below files
			§ HelloWorld.csproj
			§ Program.cs
	• dotnet restore
		○ This restores all the required packages to the Users home directory, and NOT along side the project
	• dotnet build
		○ Built the project
	• dotnet run
		○ Displayed Hello World on the console.
Unlike .Net standard, Console Application project do not create an executable file, in stead creates a DLL. When we execute dotnet run it loads the DLL and executes the code in it. Very similar to Java.
