---
title: Установка SDK Graph Microsoft
description: Содержит инструкции по установке C#, Java, Javascript, Objective-C, PHP и Ruby Microsoft Graph SDKs.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 10ad5dfa5059c7504ce9653523a31c5d0c2d17d5
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080514"
---
# <a name="install-the-microsoft-graph-sdks"></a>Установка SDKs Graph Microsoft

SDKs Graph Microsoft доступны для включаемой в проекты с помощью GitHub и популярных менеджеров пакетов платформы. В этом разделе описывается, как можно установить Graph SDK в проект.

## <a name="install-the-microsoft-graph-net-sdk"></a>Установка SDK Graph Microsoft Graph NET

SDK Graph Microsoft NuGet:

- [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Содержит модели и запрашивает у строителей доступ к конечной точке с помощью `v1.0` свободного API. Microsoft. Graph зависит от Microsoft. Graph. Core.
- [Microsoft. Graph. Бета-версия](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `beta` свободного API. Microsoft. Graph. Бета-версия зависит от Microsoft. Graph. Core.
- [Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — основная библиотека для звонков в Microsoft Graph.
- [Microsoft. Graph. Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) — предоставляет обертку на основе сценариев проверки подлинности в Библиотеке проверки подлинности Майкрософт (MSAL) для использования в microsoft Graph SDK. Microsoft. Graph. Auth имеет зависимость от Microsoft. Graph. Core.

Для установки Microsoft можно использовать [диспетчер пакетов пользовательского](/nuget/quickstart/install-and-use-a-package-in-visual-studio) интерфейса Visual Studio или консоли диспетчер пакетов консоли. Graph пакеты в проект. Следующие команды диспетчер пакетов консоли установят Microsoft. Graph, Microsoft. Graph. Core и Microsoft. Graph. Библиотеки Auth. Microsoft. Graph. Core устанавливается в зависимости от Microsoft. Graph.

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Установка microsoft Graph Java SDK

Microsoft Graph Java SDK входит в следующие пакеты:

- [Microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `v1.0` свободного API.
- [Microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) — содержит модели и запрашивает у строителей доступ к конечной точке с `beta` помощью свободного API.
- [Microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) — основная библиотека для звонков в Microsoft Graph.
- [Microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) — предоставляет обертку сценариев проверки подлинности в Microsoft Authentication Library (MSAL) для использования в microsoft Graph SDK.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Установка microsoft Graph Java SDK с помощью Gradle

Добавьте репозиторий и зависимость компиляции для microsoft-graph в сборку проекта.gradle:

```Gradle
repository {
    mavenCentral()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:3.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Установка microsoft Graph Java SDK с помощью Maven

Добавьте зависимость в `dependencies` элементе pom.xml:

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[3.3,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Установка SDK Graph Microsoft Graph Javascript

SDK Graph Microsoft Graph javascript включен в следующие пакеты:

- @microsoft/microsoft-graph-client[(npm)-](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)Основная библиотека для звонков в Microsoft Graph.
- @microsoft/microsoft-graph-types[(npm)](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)— типы typescript для сущно-Graph Microsoft.

Вы можете использовать [npm](https://www.npmjs.com) для установки SDK microsoft Graph Javascript:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Установка SDK Graph Microsoft Graph-C

SDK Graph Microsoft Graph поддерживает платформы iOS и macOS и может быть установлена в проект с помощью cocoaPods или Carthage.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Установка SDK Graph Microsoft Graph-C с помощью Cocoapods

Добавьте следующую строку в podfile, чтобы включить в проект xcode SDK Graph Microsoft Graph Objective-C Auth SDK:

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Установка SDK Graph Microsoft Graph-C с помощью Carthage

Выполните следующие действия по установке SDK Graph Microsoft Graph и Microsoft Graph-C Auth SDK с помощью диспетчера пакетов [Carthage.](https://github.com/Carthage/Carthage)

1. Создайте **картфил,** который указывает целевой тег SDK GitHub и тег [выпуска.](https://github.com/microsoftgraph/msgraph-sdk-objc/releases)

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

## <a name="install-the-microsoft-graph-php-sdk"></a>Установка SDK Graph microsoft Graph PHP

[SDK Graph phP microsoft доступен](https://github.com/microsoftgraph/msgraph-sdk-php) из [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) и может быть установлен следующим образом:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Установка microsoft Graph phP SDK вручную с помощью композитора

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Установка SDK Graph microsoft composer.js

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a>Установка SDK Microsoft PowerShell

См. [в рубрике Установка Graph PowerShell SDK](../powershell/installation.md).

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Установка SDK Graph Microsoft Graph Ruby

[SDK Graph Microsoft rubygems.org](https://github.com/microsoftgraph/msgraph-sdk-ruby) и может [](https://rubygems.org/) быть установлен с помощью следующей команды:

```ruby
gem install microsoft_graph
```
