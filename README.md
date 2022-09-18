# Project Tye test

## Getting Started

<!-- Prerequisites -->

### Prerequisites

To install Tye you can follow the [official documentation](https://github.com/dotnet/tye/blob/main/docs/getting_started.md) of project tye.

Since this repo contains:

- Two .NET Core 3.1 REST APIs
- One .NET 6 Razor app
- A React SPA

You will need to install:

- The [.NET 6](https://dotnet.microsoft.com/en-us/download) SDK
- [Node.js](https://nodejs.org/es/)
- Tye

<!-- Installation -->

### Installation

To install Tye, open a powershell terminal and run the command:

```pwsh
dotnet tool install -g Microsoft.Tye --version "0.11.0-alpha.22111.1"
```

##### \*This way of installing tye might be deprecated, go to the official documentation to see the latest way to install project tye.

<!-- Usage -->

## Usage

To start the applications just open a terminal, go to the repo folder and type the command:

```pwsh
  tye run
```

In the `tye.yaml` configuration file you will find a series of _tags_. These tags can be use to launch a subset of the applications registered in the repo.

To use tye in combination with tags run the command:

```pwsh
  tye run --tags [tag]
```

For example with the `backend` tag you will launch all the backend applications registered, the two .NET Core 3.1 REST APIs.

```pwsh
  tye run --tags backend
```

You can launch several subsets of applications combining tags

```pwsh
  tye run --tags backend frontend
```

### Have fun!
