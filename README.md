# Mendix CLI Extension for Mendix Studio Pro

This is still early stage of development. Follow this project for future updates.

## Requirements

### OSX (MacOS)

- Visual Studio Code
- Mendix Studio Pro
- dotNet core SDK vscode
- C# dev kit VSCode extension

### Windows

- TODO

## Build

```bash
dotnet build mendix-cli-studio-pro-extension.generated.sln /property:GenerateFullPaths=true /consoleloggerparameters:NoSummary /p:Configuration=Debug /p:Platform="Any CPU"

```

## Test

```bash
cp bin/Debug/net8.0 resources/App/extensions/com.cinaq.MendixCLI

/Applications/Studio\ Pro\ 10.12.2.41995-Beta.app/Contents/MacOS/studiopro --enable-extension-development
```

Open local project located in `resources/App`