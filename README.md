# BasicGeminiApp

A basic .NET core console application for trading on Gemini.


```ps1: In C:\src\github.com\ongzhixian\BasicGeminiApp
dotnet new sln -n BasicGeminiApp
dotnet new console -n BasicGeminiApp.ConsoleApp
dotnet sln .\BasicGeminiApp.sln add .\BasicGeminiApp.ConsoleApp\


dotnet add .\BasicGeminiApp.ConsoleApp\ package Microsoft.Extensions.Configuration
dotnet add .\BasicGeminiApp.ConsoleApp\ package Microsoft.Extensions.Configuration.UserSecrets
dotnet add .\BasicGeminiApp.ConsoleApp\ package Microsoft.Extensions.Configuration.Json

dotnet user-secrets --project .\BasicGeminiApp.ConsoleApp\ init
dotnet user-secrets --project .\BasicGeminiApp.ConsoleApp\ set "apiKey" "<api-value>"
dotnet user-secrets --project .\BasicGeminiApp.ConsoleApp\ set "apiSecret" "<api-value>"

```


Other ways to extend configuration

```

Microsoft.Extensions.Configuration.CommandLine 
Microsoft.Extensions.Configuration.Binder 
Microsoft.Extensions.Configuration.EnvironmentVariables
```

## Sandbox URLs

Website
https://exchange.sandbox.gemini.com

REST API
https://api.sandbox.gemini.com

WebSocket Feed
wss://api.sandbox.gemini.com

Documentation
https://docs.sandbox.gemini.com