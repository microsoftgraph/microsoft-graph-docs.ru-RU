---
title: Установка пакета SDK microsoft Graph
description: Инструкции по установке пакетов SDK Microsoft Graph для .NET, Go, Java, JavaScript, PHP, PowerShell и Python.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 7d1192b54736958858848084ae4786ef946f4c11
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577604"
---
# <a name="install-a-microsoft-graph-sdk"></a>Установка пакета SDK microsoft Graph

Пакеты SDK Microsoft Graph можно включить в проекты с помощью GitHub и популярных диспетчеров пакетов платформы. В этой статье описывается, как установить пакет SDK Microsoft Graph в проект.

Пакеты SDK доступны на следующих языках:

- [.NET](#install-the-microsoft-graph-net-sdk)
- [Go (предварительная версия)](#install-the-microsoft-graph-go-sdk-preview)
- [Java](#install-the-microsoft-graph-java-sdk)
- [JavaScript](#install-the-microsoft-graph-javascript-sdk)
- [PHP](#install-the-microsoft-graph-php-sdk)
- [PowerShell](#install-the-microsoft-graph-powershell-sdk)
- [Python (предварительная версия)](#install-the-microsoft-graph-python-sdk-preview)

## <a name="install-the-microsoft-graph-net-sdk"></a>Установка пакета SDK .NET Microsoft Graph

Пакет SDK .NET Microsoft Graph входит в следующие пакеты NuGet:

- [Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet): содержит модели и конструкторы запросов для доступа к `v1.0` конечной точке с помощью текучих API. Microsoft.Graph зависит от Microsoft.Graph.Core.
- [Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet): содержит модели и конструкторы `beta` запросов для доступа к конечной точке с помощью текучих API. Microsoft.Graph.Beta зависит от Microsoft.Graph.Core.
- [Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet): основная библиотека для выполнения вызовов к Microsoft Graph.

Чтобы установить пакеты Microsoft.Graph в проект, можно использовать пользовательский интерфейс диспетчера пакетов [в Visual Studio или консоль диспетчера пакетов](/nuget/quickstart/install-and-use-a-package-in-visual-studio). Следующие команды консоли диспетчера пакетов устанавливают библиотеки Microsoft.Graph и Microsoft.Graph.Core. Microsoft.Graph.Core устанавливается как зависимость Microsoft.Graph.

```PowerShell
Install-Package Microsoft.Graph
```

## <a name="install-the-microsoft-graph-go-sdk-preview"></a>Установка пакета SDK Microsoft Graph Go (предварительная версия)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Пакет SDK Microsoft Graph Go входит в следующие пакеты:

- [Пакет SDK Microsoft Graph для Go](https://github.com/microsoftgraph/msgraph-sdk-go): `v1.0` содержит модели и конструкторы запросов для доступа к конечной точке с помощью текучих API.
- [Бета-пакет SDK Microsoft Graph для Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go): `beta` содержит модели и конструкторы запросов для доступа к конечной точке с помощью текучих API.
- [Microsoft Graph Core SDK для Go](https://github.com/microsoftgraph/msgraph-sdk-go-core): основная библиотека для выполнения вызовов к Microsoft Graph.

```Shell
go get github.com/microsoftgraph/msgraph-sdk-go
go get github.com/Azure/azure-sdk-for-go/sdk/azidentity
go get github.com/microsoft/kiota-authentication-azure-go
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Установка пакета SDK Java для Microsoft Graph

Пакет SDK Java для Microsoft Graph входит в следующие пакеты:

- [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java): содержит модели и конструкторы запросов для доступа к `v1.0` конечной точке с помощью текучих API.
- [microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java): содержит модели и конструкторы `beta` запросов для доступа к конечной точке с помощью текучих API.
- [microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core): основная библиотека для выполнения вызовов к Microsoft Graph.
- [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth): предоставляет оболочку на основе сценария проверки подлинности библиотеки проверки подлинности Майкрософт (MSAL) для использования с пакетом SDK Microsoft Graph.

Чтобы установить пакет SDK Java для Microsoft Graph, выполните одно из следующих действий:

- Установите пакет SDK Java для Microsoft Graph с помощью Gradle. Добавьте репозиторий и зависимость компиляции для microsoft-graph в файл build.gradle проекта:
    
  ```Gradle
    repository {
        mavenCentral()
    }
    
    dependency {
        // Include the sdk as a dependency
        implementation 'com.microsoft.graph:microsoft-graph:5.+'
        // Include Azure identity for authentication
        implementation 'com.azure:azure-identity:1.+'
    }
  ```

- Установите пакет SDK Java для Microsoft Graph с помощью Maven. Добавьте зависимость в элемент в `dependencies` pom.xml:
    
  ```xml
    <dependency>
        <groupId>com.microsoft.graph</groupId>
        <artifactId>microsoft-graph</artifactId>
        <version>[5.0,)</version>
    </dependency>
    <dependency>
        <groupId>com.azure</groupId>
        <artifactId>azure-identity</artifactId>
        <version>[1.3,)</version>
    </dependency>
  ```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Установка пакета SDK JavaScript для Microsoft Graph

Пакет SDK JavaScript для Microsoft Graph входит в следующие пакеты:

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)): основная библиотека для выполнения вызовов к Microsoft Graph.
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)): типы TypeScript для сущностей Microsoft Graph.

Используйте [npm](https://www.npmjs.com) для установки пакета SDK JavaScript для Microsoft Graph:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-php-sdk"></a>Установка пакета SDK PHP для Microsoft Graph

Пакет [SDK PHP для Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-php) доступен packagist.org [](https://packagist.org/packages/microsoft/microsoft-graph) и может быть установлен следующими способами:

- Используйте composer для установки пакета SDK PHP для Microsoft Graph вручную:

    ```Shell
    composer require microsoft/microsoft-graph
    ```

- Используйте composer.json для установки пакета SDK PHP для Microsoft Graph:

    ```json
    {
        "require": {
            "microsoft/microsoft-graph": "^1.8"
        }
    }
    ```

## <a name="install-the-microsoft-graph-powershell-sdk"></a>Установка пакета SDK PowerShell для Microsoft Graph

Все модули публикуются [на коллекция PowerShell.](https://www.powershellgallery.com/packages/Microsoft.Graph) Чтобы установить:

``` powershell
Install-Module Microsoft.Graph
```

При обновлении модулей предварительной `Install-Module` `AllowClobber` `Force` версии выполните команду с параметрами и выполните их, чтобы избежать конфликтов имен команд:

``` powershell
 Install-Module Microsoft.Graph -AllowClobber -Force
```

## <a name="install-the-microsoft-graph-python-sdk-preview"></a>Установка пакета SDK Python Microsoft Graph (предварительная версия)

[!INCLUDE [python-sdk-preview](../../includes/python-sdk-preview.md)]

[Клиентская библиотека Microsoft Graph Core Python (предварительная версия)](https://github.com/microsoftgraph/msgraph-sdk-python-core) доступна в [PyPI](https://pypi.org/).

```Shell
python -m pip install msgraph-core
python -m pip install azure-identity
```

## <a name="see-also"></a>См. также

- Дополнительные сведения о функциях и возможностях пакета SDK см. в документации по требованиям к [проектированию пакета SDK](https://github.com/microsoftgraph/msgraph-sdk-design). 
- Список примеров для Microsoft Graph см. на странице ресурсов [Microsoft Graph](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples).
- Пошаговые инструкции по созданию приложения Microsoft Graph см. в руководствах [по Microsoft Graph](/graph/tutorials).