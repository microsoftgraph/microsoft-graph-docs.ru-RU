---
title: Установка пакета Microsoft Graph SDK
description: Содержит инструкции по установке пакетов SDK microsoft Graph C#, Java, JavaScript, Objective-C, PHP и Ruby.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 770b1e72d418a3f0308651b8fdd93a5e2fb7e834
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848771"
---
# <a name="install-the-microsoft-graph-sdks"></a>Установка пакетов SDK Graph Майкрософт

Пакеты SDK Graph Майкрософт можно включить в проекты с помощью GitHub и популярных диспетчеров пакетов платформы. В этом разделе описывается, как установить пакет Microsoft Graph SDK в проект.

## <a name="install-the-microsoft-graph-net-sdk"></a>Установка пакета SDK microsoft Graph .NET

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

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Установка пакета SDK Для Java Graph Майкрософт с помощью Gradle

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

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Установка пакета SDK javascript Graph Майкрософт

Пакет SDK Graph JavaScript корпорации Майкрософт входит в следующие пакеты:

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) — основная библиотека для выполнения вызовов к Microsoft Graph.
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) — типы Typescript для сущностей Microsoft Graph.

Для установки [пакета SDK Microsoft](https://www.npmjs.com) Graph Javascript можно использовать npm:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Установка пакета SDK Graph Microsoft Objective-C

Пакет SDK Graph Objective-C корпорации Майкрософт поддерживает платформы iOS и macOS и может быть установлен в проект с помощью CocoaPods или Carthage.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Установка пакета SDK Graph Microsoft Objective-C с помощью Cocoapods

Добавьте следующую строку в файл podfile, чтобы включить пакет SDK для Objective-C microsoft Graph и microsoft Graph Objective-C Auth SDK в проект xcode:

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Установка пакета SDK Graph Microsoft Objective-C с помощью Carthage

Выполните следующие действия, чтобы установить microsoft Graph Objective-C SDK и microsoft Graph Objective-C Auth SDK с помощью [диспетчера пакетов Carthage](https://github.com/Carthage/Carthage).

1. Создайте **Cartfile**, который указывает целевой репозиторий GitHub и [тег выпуска](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) Objective-C.

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. Запустите `carthage update`. Это приведет к извлечению зависимостей в папку Carthage/Checkouts, а затем создаст библиотеку MSGraphClientSDK.

1. С помощью Xcode на вкладке "Общие параметры" целевого приложения в разделе  "Связанные платформы и библиотеки" перетащите **msGraphClientSDK.framework** и **MSGraphMSALAuthProvider.framework** из папки Carthage/Build на диске.

1. На вкладке " **+** Этапы сборки" целевого приложения щелкните значок и выберите "**Новый этап запуска скрипта"**. Создайте скрипт запуска, в котором указывается оболочка (например, /bin/sh), и добавьте в скрипт следующее содержимое:

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. Добавьте пути к платформам, которые вы хотите использовать в разделе " **Входные файлы"**.

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
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

## <a name="install-the-microsoft-powershell-sdk"></a>Установка пакета SDK для Microsoft PowerShell

См[. статью "Установка пакета SDK Microsoft Graph PowerShell"](/powershell/microsoftgraph/installation.md).

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Установка microsoft Graph Ruby SDK

Пакет [SDK Microsoft Graph Ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) доступен из rubygems.org и может [](https://rubygems.org/) быть установлен с помощью следующей команды:

```ruby
gem install microsoft_graph
```
