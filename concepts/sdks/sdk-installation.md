---
title: Установка пакета Microsoft Graph SDK
description: Инструкции по установке .NET, Go, Java, JavaScript, PHP, PowerShell и Python microsoft Graph SDK.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 659730d111e3d23f0ef7a9d9352a5dc6730e37c3
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628707"
---
# <a name="install-a-microsoft-graph-sdk"></a>Установка пакета Microsoft Graph SDK

Пакеты SDK microsoft Graph доступны для нескольких языков, которые будут включены в проекты через GitHub и популярных диспетчеров пакетов платформы. В этой статье описывается, как установить пакет Microsoft Graph SDK в проект.

Пакеты SDK доступны на следующих языках.

- [.NET](#install-the-microsoft-graph-net-sdk)
- [Go (предварительная версия)](#install-the-microsoft-graph-go-sdk-preview)
- [Java](#install-the-microsoft-graph-java-sdk)
- [JavaScript](#install-the-microsoft-graph-javascript-sdk)
- [PHP](#install-the-microsoft-graph-php-sdk)
- [PowerShell](#install-the-microsoft-graph-powershell-sdk)
- [Python (предварительная версия)](#install-the-microsoft-graph-python-sdk-preview)

## <a name="install-the-microsoft-graph-net-sdk"></a>Установка пакета Microsoft Graph .NET SDK

Пакет SDK microsoft Graph .NET включен в следующие пакеты NuGet пакетов:

- [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — содержит модели и конструкторы запросов для доступа к `v1.0` конечной точке с помощью текучих API. Microsoft. Graph зависит от корпорации Майкрософт. Graph. Основные.
- [Microsoft. Graph. Бета-версия](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) — содержит модели и конструкторы запросов для доступа к `beta` конечной точке с помощью текучих API. Microsoft. Graph. Бета-версия зависит от корпорации Майкрософт. Graph. Основные.
- [Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — основная библиотека для выполнения вызовов к microsoft Graph.

Для установки пакетов Microsoft.Graph в проект можно использовать пользовательский диспетчер пакетов в Visual Studio или консоль [диспетчер пакетов](/nuget/quickstart/install-and-use-a-package-in-visual-studio). Следующие команды диспетчер пакетов консоли установит Microsoft.Graph и Microsoft.Graph. Основные библиотеки. Microsoft. Graph. Ядро устанавливается как зависимость корпорации Майкрософт. Graph.

```PowerShell
Install-Package Microsoft.Graph
```

## <a name="install-the-microsoft-graph-go-sdk-preview"></a>Установка пакета SDK Microsoft Graph Go (предварительная версия)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Пакет SDK Microsoft Graph Go входит в следующие пакеты:

- [Microsoft Graph SDK для Go](https://github.com/microsoftgraph/msgraph-sdk-go) `v1.0` — содержит модели и конструкторы запросов для доступа к конечной точке с помощью текучих API.
- [Microsoft Graph бета-версии пакета SDK для Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go) `beta` — содержит модели и построицы запросов для доступа к конечной точке с помощью текучих API.
- [Microsoft Graph Core SDK для Go](https://github.com/microsoftgraph/msgraph-sdk-go-core) — основная библиотека для вызовов к Microsoft Graph.

```Shell
go get github.com/microsoftgraph/msgraph-sdk-go
go get github.com/Azure/azure-sdk-for-go/sdk/azidentity
go get github.com/microsoft/kiota-authentication-azure-go
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Установка пакета SDK microsoft Graph Java

Пакет SDK Graph Майкрософт для Java входит в следующие пакеты:

- [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) — содержит модели и конструкторы запросов для доступа к `v1.0` конечной точке с помощью текучих API.
- [microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) — содержит модели `beta` и конструкторы запросов для доступа к конечной точке с помощью текучих API.
- [microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) — основная библиотека для выполнения вызовов к Microsoft Graph.
- [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) — предоставляет оболочку на основе сценария проверки подлинности библиотеки проверки подлинности Майкрософт (MSAL) для использования с пакетом Microsoft Graph SDK.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Установите пакет SDK Microsoft Graph Java с помощью Gradle

Добавьте репозиторий и зависимость компиляции для microsoft-graph в файл build.gradle проекта:

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

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Установка пакета SDK Microsoft Graph Java с помощью Maven

Добавьте зависимость в элемент в `dependencies` pom.xml:

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

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Установка пакета SDK Graph JavaScript для Microsoft

Пакет SDK Graph JavaScript корпорации Майкрософт входит в следующие пакеты:

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) — основная библиотека для выполнения вызовов к Microsoft Graph.
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) — типы Typescript для сущностей Microsoft Graph.

Вы можете использовать [npm](https://www.npmjs.com) для установки пакета SDK Microsoft Graph JavaScript:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-php-sdk"></a>Установка пакета SDK GRAPH Майкрософт

Пакет [SDK PHP](https://github.com/microsoftgraph/msgraph-sdk-php) Graph Microsoft доступен из packagist.org и может быть [](https://packagist.org/packages/microsoft/microsoft-graph) установлен следующим образом:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Установка пакета SDK microsoft Graph PHP вручную с помощью composer

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Установка пакета SDK Graph PHP майкрософт с помощью composer.json

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-graph-powershell-sdk"></a>Установка пакета SDK Microsoft Graph PowerShell

Все модули публикуются [на коллекция PowerShell.](https://www.powershellgallery.com/packages/Microsoft.Graph) Чтобы установить:

``` powershell
Install-Module Microsoft.Graph
```

При обновлении модулей `Install-Module` предварительной версии запустите с помощью параметров AllowClobber и Force, чтобы избежать конфликтов имен команд:

``` powershell
 Install-Module Microsoft.Graph -AllowClobber -Force
```

## <a name="install-the-microsoft-graph-python-sdk-preview"></a>Установка пакета Microsoft Graph Python SDK (предварительная версия)

[!INCLUDE [python-sdk-preview](../../includes/python-sdk-preview.md)]

[Клиентская Graph Microsoft Python Core (предварительная версия)](https://github.com/microsoftgraph/msgraph-sdk-python-core) доступна в [PyPI](https://pypi.org/).

```Shell
python -m pip install msgraph-core
python -m pip install azure-identity
```
