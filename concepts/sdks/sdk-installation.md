---
title: Установка пакета SDK Microsoft Graph
description: Содержит инструкции по установке пакетов SDK для C#, Java, JavaScript, задания на языке, PHP и Ruby Microsoft Graph.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 7f96266c1ff774f52e559737fe67f032f1e54fdc
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580958"
---
# <a name="install-the-microsoft-graph-sdks"></a>Установка пакетов SDK Microsoft Graph

Пакеты SDK Microsoft Graph доступны для включения в проекты через GitHub и популярные диспетчеры пакетов платформы. В этом разделе описывается, как можно установить пакет SDK Microsoft Graph в проекте.

## <a name="install-the-microsoft-graph-net-sdk"></a>Установка Microsoft Graph .NET SDK

Microsoft Graph .NET SDK включен в следующие пакеты NuGet:

- [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) содержит модели и построители запросов для доступа к `v1.0` конечной точке с помощью API Fluent. Microsoft. Graph зависит от Microsoft. Graph. Core.
- [Microsoft. Graph. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) — содержит модели и построители запросов для доступа к `beta` конечной точке с помощью API Fluent. Microsoft. Graph. Beta зависит от Microsoft. Graph. Core.
- [Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — основная библиотека для совершения вызовов в Microsoft Graph.
- [Microsoft. Graph. auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) — предоставляет оболочку проверки подлинности на основе сценария для библиотеки проверки подлинности Microsoft (MSAL) для использования с пакетом SDK Microsoft Graph. Microsoft. Graph. auth имеет зависимость от Microsoft. Graph. Core.

Для установки пакетов Microsoft. Graph в проект можно использовать [Пользовательский интерфейс диспетчера пакетов в Visual Studio или консоли диспетчера пакетов](/nuget/quickstart/install-and-use-a-package-in-visual-studio) . Следующие команды консоли диспетчера пакетов будут устанавливать библиотеки Microsoft. Graph, Microsoft. Graph. Core и Microsoft. Graph. auth. Microsoft. Graph. Core устанавливается как зависимость от Microsoft. Graph.

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Установка пакета SDK Java Microsoft Graph

Пакет SDK Microsoft Graph Java включен в следующие пакеты:

- [Microsoft-Graph](https://github.com/microsoftgraph/msgraph-sdk-java) — содержит модели и построители запросов для доступа к `v1.0` конечной точке с помощью API Fluent.
- [Microsoft-Graph-бета-версия](https://github.com/microsoftgraph/msgraph-beta-sdk-java) содержит модели и построители запросов для доступа к `beta` конечной точке с помощью API Fluent.
- [Microsoft — Graph — Core](https://github.com/microsoftgraph/msgraph-sdk-java-core) — основная библиотека для совершения вызовов в Microsoft Graph.
- [Microsoft-Graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -предоставляет оболочку проверки подлинности (MSAL), основанную на сценариях проверки подлинности (), для использования с пакетом SDK Microsoft Graph.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Установка пакета SDK Java Microsoft Graph с помощью Gradle

Добавьте репозиторий и зависимость компиляции для Microsoft Graph к сборке проекта. gradle:

```Gradle
repository {
    jcenter()
    jcenter{
        url 'https://oss.jfrog.org/artifactory/oss-snapshot-local'
    }
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:2.+'
    implementation 'com.microsoft.graph:microsoft-graph-auth:0.3.0'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Установка пакета SDK Java Microsoft Graph с помощью Мавен

Добавьте репозитории в `profiles` элемент в pom.xml:

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
    <profile>
       <id>allow-snapshots</id>
          <activation><activeByDefault>true</activeByDefault></activation>
       <repositories>
         <repository>
           <id>snapshots-repo</id>
           <url>https://oss.sonatype.org/content/repositories/snapshots</url>
           <releases><enabled>false</enabled></releases>
           <snapshots><enabled>true</enabled></snapshots>
         </repository>
       </repositories>
     </profile>
</profiles>
```

Добавьте зависимость в `dependencies` элемент в pom.xml:

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[2.0,)</version>
</dependency>
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph-auth</artifactId>
    <version>0.3.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Установка пакета SDK JavaScript для Microsoft Graph

Пакет SDK для JavaScript для Microsoft Graph включен в следующие пакеты:

- @microsoft/Микрософт-граф-клиент ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) — основная библиотека для совершения вызовов в Microsoft Graph.
- @microsoft/Микрософт-граф-типес ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) — типы typescript для сущностей Microsoft Graph.

С помощью [NPM](https://www.npmjs.com) можно установить пакет SDK JavaScript для Microsoft Graph:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Установка пакета SDK Microsoft Graph для цели

Пакет SDK целевого приложения Microsoft Graph поддерживает платформы iOS и macOS и может быть установлен в проекте с помощью CocoaPods или Карсаже.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Установка пакета SDK Microsoft Graph с помощью Cocoapods

Добавьте указанную ниже строку в podfile, чтобы включить пакет SDK целевого уровня и Microsoft Graph для Microsoft Graph в проект Xcode:

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Установка пакета SDK Microsoft Graph с помощью Карсаже

Выполните следующие действия, чтобы установить пакет SDK целевого приложения Microsoft Graph и Microsoft Graph с целевой системой проверки подлинности с помощью диспетчера пакетов [карсаже](https://github.com/Carthage/Carthage) .

1. Создайте объект **картфиле** , указывающий репозиторий GitHub и [тег выпуска](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) для целевого объекта "целевой объект".

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. Выполните команду `carthage update` . Это приведет к извлечению зависимостей в папку Карсаже/Checkout и последующее построение библиотеки Мсграфклиентсдк.

1. С помощью Xcode на вкладке **Общие** параметры конечного приложения, в разделе **связанные платформы и библиотеки** , перетащите **мсграфклиентсдк. Framework** и **Мсграфмсалауспровидер. Framework** из папки карсаже/Build на диске.

1. На вкладке Параметры **этапа построения** конечного приложения щелкните **+** значок и выберите **создать этап скрипта запуска**. Создайте скрипт запуска, в котором вы указали командную консоль (ex:/бин/ш), и добавьте в сценарий следующее содержимое:

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. Добавьте пути к платформам, которые вы хотите использовать для **входных файлов**.

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a>Установка пакета SDK для Microsoft Graph PHP

[Пакет SDK Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-php) доступен в [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) и может устанавливаться следующими способами:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Установка пакета SDK для Microsoft Graph PHP вручную с помощью Composer

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Установите пакет SDK для Microsoft Graph PHP с помощью composer.jsна

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a>Установка пакета SDK для Microsoft PowerShell

Ознакомьтесь [с Разустановочным пакетом SDK PowerShell для Microsoft Graph](../powershell/installation.md).

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Установка пакета SDK Microsoft Graph Ruby

[Пакет SDK Microsoft Graph Ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) доступен в [RubyGems.org](https://rubygems.org/) , и его можно установить с помощью следующей команды:

```ruby
gem install microsoft_graph
```
