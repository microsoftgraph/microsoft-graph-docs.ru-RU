---
title: Установка пакета SDK Microsoft Graph
description: Содержит инструкции по установке пакетов SDK для C#, Java, JavaScript, задания на языке, PHP и Ruby Microsoft Graph.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 9fdb05c6d6fbe3e35f1ed80ddb8223bc3b3f290b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868578"
---
# <a name="install-the-microsoft-graph-sdks"></a>Установка пакетов SDK Microsoft Graph

Пакеты SDK Microsoft Graph доступны для включения в проекты через GitHub и популярные диспетчеры пакетов платформы. В этом разделе описывается, как можно установить пакет SDK Microsoft Graph в проекте.

## <a name="install-the-microsoft-graph-net-sdk"></a>Установка Microsoft Graph .NET SDK

Microsoft Graph .NET SDK включен в следующие пакеты NuGet:

* [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) содержит модели и построители запросов для доступа к `v1.0` КОНЕЧНОЙ точке с помощью API Fluent. Microsoft. Graph зависит от Microsoft. Graph. Core.
* [Microsoft. Graph. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) — содержит модели и построители запросов для доступа к `beta` КОНЕЧНОЙ точке с помощью API Fluent. Microsoft. Graph. Beta зависит от Microsoft. Graph. Core.
* [Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — основная библиотека для совершения вызовов в Microsoft Graph.
* [Microsoft. Graph. auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) — предоставляет оболочку проверки подлинности на основе сценария для библиотеки проверки подлинности Microsoft (MSAL) для использования с пакетом SDK Microsoft Graph. Microsoft. Graph. auth имеет зависимость от Microsoft. Graph. Core.

Для установки пакетов Microsoft. Graph в проект можно использовать [Пользовательский интерфейс диспетчера пакетов в Visual Studio или консоли диспетчера пакетов](/nuget/quickstart/install-and-use-a-package-in-visual-studio) . Следующие команды консоли диспетчера пакетов будут устанавливать библиотеки Microsoft. Graph, Microsoft. Graph. Core и Microsoft. Graph. auth. Microsoft. Graph. Core устанавливается как зависимость от Microsoft. Graph.

```
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Установка пакета SDK Java Microsoft Graph

Пакет SDK Microsoft Graph Java включен в следующие пакеты:

* [Microsoft-Graph](https://github.com/microsoftgraph/msgraph-sdk-java) — содержит модели и построители запросов для доступа к `v1.0` КОНЕЧНОЙ точке с помощью API Fluent.
* [Microsoft — Graph — Core](https://github.com/microsoftgraph/msgraph-sdk-java-core) — основная библиотека для совершения вызовов в Microsoft Graph.
* [Microsoft-Graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -предоставляет оболочку проверки подлинности (MSAL), основанную на сценариях проверки подлинности (), для использования с пакетом SDK Microsoft Graph.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Установка пакета SDK Java Microsoft Graph с помощью Gradle

Добавьте репозиторий и зависимость компиляции для Microsoft Graph к сборке проекта. gradle:

```
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    compile('com.microsoft.graph:microsoft-graph:1.2.+')
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Установка пакета SDK Java Microsoft Graph с помощью Мавен

Добавьте зависимость в элемент Dependencies в пом. XML:

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>1.2.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Установка пакета SDK JavaScript для Microsoft Graph

Пакет SDK для JavaScript для Microsoft Graph включен в следующие пакеты:

* @microsoft/Микрософт-граф-клиент ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) — основная библиотека для совершения вызовов в Microsoft Graph.
* @microsoft/Микрософт-граф-типес ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) — типы typescript для сущностей Microsoft Graph.

С помощью [NPM](https://www.npmjs.com) можно установить пакет SDK JavaScript для Microsoft Graph:

```
npm install @microsoft/microsoft-graph-client
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Установка пакета SDK Microsoft Graph для цели

Пакет SDK целевого приложения Microsoft Graph поддерживает платформы iOS и macOS и может быть установлен в проекте с помощью CocoaPods или Карсаже.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Установка пакета SDK Microsoft Graph с помощью Cocoapods

Добавьте указанную ниже строку в podfile, чтобы включить пакет SDK целевого уровня и Microsoft Graph для Microsoft Graph в проект Xcode:

```
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Установка пакета SDK Microsoft Graph с помощью Карсаже

Выполните следующие действия, чтобы установить пакет SDK целевого приложения Microsoft Graph и Microsoft Graph с целевой системой проверки подлинности с помощью диспетчера пакетов [карсаже](https://github.com/Carthage/Carthage) .

1. Создайте объект **картфиле** , указывающий репозиторий GitHub и [тег выпуска](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) для целевого объекта "целевой объект".

```
github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
```

2. Выполните `carthage update`команду. Это приведет к извлечению зависимостей в папку Карсаже/Checkout и последующее построение библиотеки Мсграфклиентсдк.

3. С помощью Xcode на вкладке **Общие** параметры конечного приложения, в разделе **связанные платформы и библиотеки** , перетащите **мсграфклиентсдк. Framework** и **Мсграфмсалауспровидер. Framework** из папки карсаже/Build на диске.

4. На вкладке Параметры **этапа построения** конечного приложения щелкните **+** значок и выберите **создать этап скрипта запуска**. Создайте скрипт запуска, в котором вы указали командную консоль (ex:/бин/ш), и добавьте в сценарий следующее содержимое:

```
/usr/local/bin/carthage copy-frameworks
```

5. Добавьте пути к платформам, которые вы хотите использовать для **входных файлов**.

```
$(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
$(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
```

## <a name="install-the-microsoft-graph-php-sdk"></a>Установка пакета SDK для Microsoft Graph PHP

[Пакет SDK Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-php) доступен в [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) и может устанавливаться следующими способами:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Установка пакета SDK для Microsoft Graph PHP вручную с помощью Composer

```
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Установка пакета SDK для PHP для Microsoft Graph с помощью Composer. JSON

```
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Установка пакета SDK Microsoft Graph Ruby

[Пакет SDK Microsoft Graph Ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) доступен в [RubyGems.org](https://rubygems.org/) , и его можно установить с помощью следующей команды:

```
gem install microsoft_graph
```
