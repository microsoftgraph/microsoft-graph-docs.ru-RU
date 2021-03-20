---
title: Установка SDK Microsoft Graph
description: Содержит инструкции по установке SDKs C#, Java, Javascript, Objective-C, PHP и Ruby Microsoft Graph.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: cd019a8f13bd0ffe154a2a998d59815addf664e9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941395"
---
# <a name="install-the-microsoft-graph-sdks"></a>Установка SDKs Microsoft Graph

SDKs Microsoft Graph доступны для включаемого в проекты с помощью GitHub и популярных менеджеров пакетов платформы. В этом разделе описывается, как можно установить SDK Microsoft Graph в проект.

## <a name="install-the-microsoft-graph-net-sdk"></a>Установка SDK Microsoft Graph .NET

SDK Microsoft Graph .NET включен в следующие пакеты NuGet:

- [Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `v1.0` свободного API. Microsoft.Graph имеет зависимость от Microsoft.Graph.Core.
- [Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `beta` свободного API. Microsoft.Graph.Beta имеет зависимость от Microsoft.Graph.Core.
- [Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — основная библиотека для звонков в Microsoft Graph.
- [Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) — предоставляет обертку сценариев проверки подлинности в Библиотеке проверки подлинности Майкрософт (MSAL) для использования в SDK Microsoft Graph. Microsoft.Graph.Auth имеет зависимость от Microsoft.Graph.Core.

Для установки пакетов Microsoft.Graph [в проект](/nuget/quickstart/install-and-use-a-package-in-visual-studio) можно диспетчер пакетов пользовательского интерфейса Visual Studio или консоли диспетчер пакетов консоли. Следующие команды диспетчер пакетов консоли установят библиотеки Microsoft.Graph, Microsoft.Graph.Core и Microsoft.Graph.Auth. Microsoft.Graph.Core устанавливается в зависимости от Microsoft.Graph.

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Установка SDK Microsoft Graph Java

SDK Microsoft Graph Java включен в следующие пакеты:

- [Microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `v1.0` свободного API.
- [Microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) — содержит модели и запрашивает у строителей доступ к конечной точке с `beta` помощью свободного API.
- [Microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) — основная библиотека для звонков в Microsoft Graph.
- [Microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) — предоставляет оболочку для проверки подлинности на основе сценария Microsoft Authentication Library (MSAL) для использования с помощью SDK Microsoft Graph.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Установка SDK Microsoft Graph Java с помощью Gradle

Добавьте репозиторий и зависимость компиляции для microsoft-graph в сборку проекта.gradle:

```Gradle
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:3.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Установка SDK Microsoft Graph Java через Maven

Добавление репозиториев в `profiles` элементе pom.xml:

```xml
<profiles>
    <profile>
        <repositories>
            <repository>
                <snapshots>
                    <enabled>false</enabled>
                </snapshots>
                <id>bintray-microsoftgraph-Maven</id>
                <name>bintray</name>
                <url>https://dl.bintray.com/microsoftgraph/Maven</url>
            </repository>
        </repositories>
    </profile>
</profiles>
```

Добавьте зависимость в `dependencies` элементе pom.xml:

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[3.0,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Установка SDK Javascript Microsoft Graph

SDK Javascript Microsoft Graph включен в следующие пакеты:

- @microsoft/microsoft-graph-client[(npm)](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)— основная библиотека для звонков в Microsoft Graph.
- @microsoft/microsoft-graph-types[(npm)](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)— типы typescript для сущностям Microsoft Graph.

Вы можете использовать [npm](https://www.npmjs.com) для установки SDK Javascript Microsoft Graph:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Установка SDK Microsoft Graph Objective-C

SDK Microsoft Graph Objective-C поддерживает платформы iOS и macOS и может быть установлен в проект с помощью cocoaPods или Carthage.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Установка SDK Microsoft Graph Objective-C с помощью Cocoapods

Добавьте следующую строку в podfile, чтобы включить SDK Microsoft Graph Objective-C и Microsoft Graph Objective-C Auth SDK в проект xcode:

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Установка SDK Microsoft Graph Objective-C с помощью carthage

Выполните следующие действия, чтобы установить SDK Microsoft Graph Objective-C и Microsoft Graph Objective-C Auth SDK с помощью диспетчера пакетов [Carthage.](https://github.com/Carthage/Carthage)

1. Создайте **картфиль,** который указывает репозиторий Objective-C SDK GitHub и тег [выпуска](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) для целевого адреса.

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. Запуск `carthage update` . Это позволит извлечь зависимости в папку Картидж/Проверка, а затем создает библиотеку MSGraphClientSDK.

1. Используя Xcode, в вкладке  Общие параметры целевого приложения в разделе Linked **Frameworks and Libraries** перетащите и отклоняйте папку **MSGraphClientSDK.framework** и **MSGraphMSALAuthProvider.framework** из папки Carthage/Build на диске.

1. На вкладке Параметры **этапов** сборки целевого приложения щелкните значок и **+** выберите новую **фазу сценария запуска.** Создайте сценарий запуска, в котором укажите оболочку (например: /bin/sh), и добавьте в сценарий следующее содержимое:

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. Добавьте пути к фреймворкам, которые необходимо использовать в **вводимых файлах.**

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a>Установка SDK PHP Microsoft Graph

[SDK PHP Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-php) [](https://packagist.org/packages/microsoft/microsoft-graph) доступен из packagist.org и может быть установлен следующим образом:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Установка SDK PHP Microsoft Graph вручную с помощью композитора

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Установка SDK PHP Microsoft Graph с composer.js

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a>Установка SDK Microsoft PowerShell

См. [установку SDK Microsoft Graph PowerShell.](../powershell/installation.md)

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Установка SDK Microsoft Graph Ruby

[SDK Microsoft Graph Ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) [доступен](https://rubygems.org/) из rubygems.org и может быть установлен с помощью следующей команды:

```ruby
gem install microsoft_graph
```
