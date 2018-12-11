# Gaia Backend
This app is built with Asp.net Core 2, please download the SDK from dot.net
This repo uses the /Gaia UI repo as a submodule please clone using 
```sh
git clone --recurse-submodules https://github.com/GaiaCarbon/backend.git
```
and switch "/GaiaMain/ClientApp" to your desired UI branch.
### Build
```sh
cd ./GaiaMain/
dotnet build
dotnet run
```
### Develop
Visual Studio and VS Code have been pre-configured with 2 run profies.
| Profile | ASPNETCORE_ENVIRONMENT |  |
| ------ | ------ | ------ |
| GaiaMain |Development |Launches the Asp.net Core app and internally runs the create-react-app server |
| GaiaMainUI|Development-UI | Launches the Asp.net Core app and proxies the react app from http://localhost:3000  |
JetBrains rider will require you to create a run profile for the specific environment variable.
