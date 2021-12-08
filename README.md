# ApiExample

```shellscript
mkdir ApiExample
cd ApiExample
dotnet new sln ApiExample
mkdir ApiProducts
cd ApiProducts
dotnet new webapi
cd Controllers
mkdir App
mkdir Domain
mkdir Infra/Data
mkdir Infra/IoC
cd App
dotnet new classlib
cd ..
cd Domain
dotnet new classlib
cd ..
cd Infra/Data
dotnet new classlib
cd ../..
cd Infra/IoC
dotnet new classlib
cd ../..


cd ..
dotnet sln add ApiProducts/Domain/Domain.csproj
dotnet sln add ApiProducts/App/App.csproj
dotnet sln add ApiProducts/Infra/Data/Data.csproj
dotnet sln add ApiProducts/Infra/IoC/IoC.csproj
```