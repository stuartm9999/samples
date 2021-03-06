Visio Demo
================

This is a basic Visio demo sample in .NET Core. It is designed to work with .NET Core 3.0. It is based on the Excel Demo sample found here:
* [https://github.com/dotnet/samples/tree/master/core/extensions/ExcelDemo](https://github.com/dotnet/samples/tree/master/core/extensions/ExcelDemo)

Key Features
------------

Demonstrates how to consume Office Primary Interop Assemblies (PIA) with .NET Core 3.0 Preview 2.

- Embedding of Interop types (i.e. [No-PIA](https://docs.microsoft.com/en-us/dotnet/framework/interop/type-equivalence-and-embedded-interop-types)).
- Support for the [`IDispatch`](https://docs.microsoft.com/en-us/windows/desktop/winauto/idispatch-interface) interface.

**Note** Adding COM references to .NET Core projects from Visual Studio is not currently supported. The workaround is to create a .NET Framework project, add the COM references, and then copy the relevant `COMReference` elements in the project. See `ExcelDemo.csproj` for further details.

Build and Run
-------------

To build and run the sample, the project must be loaded in Visual Studio 2017. Build support for `COMReference` elements is not supported in the `dotnet` tool for the Preview 2 release, but the scenario is demoable from within Visual Studio 2017.

1) Install .NET Core 3.0 Preview 2.

1) Load `VisioDemo.csproj` in Visual Studio 2017.
    - Double click on `VisioDemo.csproj` in File Explorer.

    or

    - Open a Developer Command prompt and open with `devenv.exe VisioDemo.csproj`.

1) Press F5 to build and debug the project.
