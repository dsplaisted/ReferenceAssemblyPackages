# .NET Framework Reference Assemblies NuGet Packages

This repo is a proof-of concept for creating NuGet packages which contain the .NET Framework reference assemblies.

To build, you'll need Visual Studio 2017 and the targeting packs installed for each version of .NET Framework for which reference assembly packages will be created.  Then, from the repo root, you can run:

```
msbuild Microsoft.NETFramework.ReferenceAssemblies\Microsoft.NETFramework.ReferenceAssemblies.csproj /t:restore
msbuild Microsoft.NETFramework.ReferenceAssemblies\Microsoft.NETFramework.ReferenceAssemblies.csproj
```

The NuGet packages will be produced in the `bin\Debug` folder at the root of the repo.