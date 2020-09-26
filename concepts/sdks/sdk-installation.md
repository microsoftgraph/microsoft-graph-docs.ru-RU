---
title: Установка пакета SDK Microsoft Graph
description: Содержит инструкции по установке пакетов SDK для C#, Java, JavaScript, задания на языке, PHP и Ruby Microsoft Graph.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: d9feb4ebca4cc0558ad981e1598ff6f7d68ac95a
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289472"
---
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="f2a02-103">Установка пакетов SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f2a02-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="f2a02-104">Пакеты SDK Microsoft Graph доступны для включения в проекты через GitHub и популярные диспетчеры пакетов платформы.</span><span class="sxs-lookup"><span data-stu-id="f2a02-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="f2a02-105">В этом разделе описывается, как можно установить пакет SDK Microsoft Graph в проекте.</span><span class="sxs-lookup"><span data-stu-id="f2a02-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="f2a02-106">Установка Microsoft Graph .NET SDK</span><span class="sxs-lookup"><span data-stu-id="f2a02-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="f2a02-107">Microsoft Graph .NET SDK включен в следующие пакеты NuGet:</span><span class="sxs-lookup"><span data-stu-id="f2a02-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="f2a02-108">[Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) содержит модели и построители запросов для доступа к `v1.0` конечной точке с помощью API Fluent.</span><span class="sxs-lookup"><span data-stu-id="f2a02-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="f2a02-109">Microsoft. Graph зависит от Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="f2a02-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="f2a02-110">[Microsoft. Graph. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) — содержит модели и построители запросов для доступа к `beta` конечной точке с помощью API Fluent.</span><span class="sxs-lookup"><span data-stu-id="f2a02-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="f2a02-111">Microsoft. Graph. Beta зависит от Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="f2a02-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="f2a02-112">[Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — основная библиотека для совершения вызовов в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f2a02-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="f2a02-113">[Microsoft. Graph. auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) — предоставляет оболочку проверки подлинности на основе сценария для библиотеки проверки подлинности Microsoft (MSAL) для использования с пакетом SDK Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f2a02-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="f2a02-114">Microsoft. Graph. auth имеет зависимость от Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="f2a02-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="f2a02-115">Для установки пакетов Microsoft. Graph в проект можно использовать [Пользовательский интерфейс диспетчера пакетов в Visual Studio или консоли диспетчера пакетов](/nuget/quickstart/install-and-use-a-package-in-visual-studio) .</span><span class="sxs-lookup"><span data-stu-id="f2a02-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="f2a02-116">Следующие команды консоли диспетчера пакетов будут устанавливать библиотеки Microsoft. Graph, Microsoft. Graph. Core и Microsoft. Graph. auth.</span><span class="sxs-lookup"><span data-stu-id="f2a02-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="f2a02-117">Microsoft. Graph. Core устанавливается как зависимость от Microsoft. Graph.</span><span class="sxs-lookup"><span data-stu-id="f2a02-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="f2a02-118">Установка пакета SDK Java Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f2a02-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="f2a02-119">Пакет SDK Microsoft Graph Java включен в следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="f2a02-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="f2a02-120">[Microsoft-Graph](https://github.com/microsoftgraph/msgraph-sdk-java) — содержит модели и построители запросов для доступа к `v1.0` конечной точке с помощью API Fluent.</span><span class="sxs-lookup"><span data-stu-id="f2a02-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="f2a02-121">[Microsoft-Graph-бета-версия](https://github.com/microsoftgraph/msgraph-beta-sdk-java) содержит модели и построители запросов для доступа к `beta` конечной точке с помощью API Fluent.</span><span class="sxs-lookup"><span data-stu-id="f2a02-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span>
- <span data-ttu-id="f2a02-122">[Microsoft — Graph — Core](https://github.com/microsoftgraph/msgraph-sdk-java-core) — основная библиотека для совершения вызовов в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f2a02-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="f2a02-123">[Microsoft-Graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -предоставляет оболочку проверки подлинности (MSAL), основанную на сценариях проверки подлинности (), для использования с пакетом SDK Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f2a02-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="f2a02-124">Установка пакета SDK Java Microsoft Graph с помощью Gradle</span><span class="sxs-lookup"><span data-stu-id="f2a02-124">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="f2a02-125">Добавьте репозиторий и зависимость компиляции для Microsoft Graph к сборке проекта. gradle:</span><span class="sxs-lookup"><span data-stu-id="f2a02-125">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```Gradle
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:2.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="f2a02-126">Установка пакета SDK Java Microsoft Graph с помощью Мавен</span><span class="sxs-lookup"><span data-stu-id="f2a02-126">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="f2a02-127">Добавьте зависимость в элемент Dependencies в pom.xml:</span><span class="sxs-lookup"><span data-stu-id="f2a02-127">Add the dependency in the dependencies element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[2.0,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="f2a02-128">Установка пакета SDK JavaScript для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f2a02-128">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="f2a02-129">Пакет SDK для JavaScript для Microsoft Graph включен в следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="f2a02-129">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="f2a02-130">@microsoft/Микрософт-граф-клиент ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) — основная библиотека для совершения вызовов в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f2a02-130">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="f2a02-131">@microsoft/Микрософт-граф-типес ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) — типы typescript для сущностей Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f2a02-131">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="f2a02-132">С помощью [NPM](https://www.npmjs.com) можно установить пакет SDK JavaScript для Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="f2a02-132">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="f2a02-133">Установка пакета SDK Microsoft Graph для цели</span><span class="sxs-lookup"><span data-stu-id="f2a02-133">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="f2a02-134">Пакет SDK целевого приложения Microsoft Graph поддерживает платформы iOS и macOS и может быть установлен в проекте с помощью CocoaPods или Карсаже.</span><span class="sxs-lookup"><span data-stu-id="f2a02-134">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="f2a02-135">Установка пакета SDK Microsoft Graph с помощью Cocoapods</span><span class="sxs-lookup"><span data-stu-id="f2a02-135">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="f2a02-136">Добавьте указанную ниже строку в podfile, чтобы включить пакет SDK целевого уровня и Microsoft Graph для Microsoft Graph в проект Xcode:</span><span class="sxs-lookup"><span data-stu-id="f2a02-136">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="f2a02-137">Установка пакета SDK Microsoft Graph с помощью Карсаже</span><span class="sxs-lookup"><span data-stu-id="f2a02-137">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="f2a02-138">Выполните следующие действия, чтобы установить пакет SDK целевого приложения Microsoft Graph и Microsoft Graph с целевой системой проверки подлинности с помощью диспетчера пакетов [карсаже](https://github.com/Carthage/Carthage) .</span><span class="sxs-lookup"><span data-stu-id="f2a02-138">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="f2a02-139">Создайте объект **картфиле** , указывающий репозиторий GitHub и [тег выпуска](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) для целевого объекта "целевой объект".</span><span class="sxs-lookup"><span data-stu-id="f2a02-139">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="f2a02-140">Выполните команду `carthage update` .</span><span class="sxs-lookup"><span data-stu-id="f2a02-140">Run `carthage update`.</span></span> <span data-ttu-id="f2a02-141">Это приведет к извлечению зависимостей в папку Карсаже/Checkout и последующее построение библиотеки Мсграфклиентсдк.</span><span class="sxs-lookup"><span data-stu-id="f2a02-141">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="f2a02-142">С помощью Xcode на вкладке **Общие** параметры конечного приложения, в разделе **связанные платформы и библиотеки** , перетащите **мсграфклиентсдк. Framework** и **Мсграфмсалауспровидер. Framework** из папки карсаже/Build на диске.</span><span class="sxs-lookup"><span data-stu-id="f2a02-142">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="f2a02-143">На вкладке Параметры **этапа построения** конечного приложения щелкните **+** значок и выберите **создать этап скрипта запуска**.</span><span class="sxs-lookup"><span data-stu-id="f2a02-143">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="f2a02-144">Создайте скрипт запуска, в котором вы указали командную консоль (ex:/бин/ш), и добавьте в сценарий следующее содержимое:</span><span class="sxs-lookup"><span data-stu-id="f2a02-144">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="f2a02-145">Добавьте пути к платформам, которые вы хотите использовать для **входных файлов**.</span><span class="sxs-lookup"><span data-stu-id="f2a02-145">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="f2a02-146">Установка пакета SDK для Microsoft Graph PHP</span><span class="sxs-lookup"><span data-stu-id="f2a02-146">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="f2a02-147">[Пакет SDK Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-php) доступен в [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) и может устанавливаться следующими способами:</span><span class="sxs-lookup"><span data-stu-id="f2a02-147">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="f2a02-148">Установка пакета SDK для Microsoft Graph PHP вручную с помощью Composer</span><span class="sxs-lookup"><span data-stu-id="f2a02-148">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="f2a02-149">Установите пакет SDK для Microsoft Graph PHP с помощью composer.jsна</span><span class="sxs-lookup"><span data-stu-id="f2a02-149">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="f2a02-150">Установка пакета SDK для Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="f2a02-150">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="f2a02-151">Ознакомьтесь [с Разустановочным пакетом SDK PowerShell для Microsoft Graph](../powershell/installation.md).</span><span class="sxs-lookup"><span data-stu-id="f2a02-151">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="f2a02-152">Установка пакета SDK Microsoft Graph Ruby</span><span class="sxs-lookup"><span data-stu-id="f2a02-152">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="f2a02-153">[Пакет SDK Microsoft Graph Ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) доступен в [RubyGems.org](https://rubygems.org/) , и его можно установить с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="f2a02-153">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
