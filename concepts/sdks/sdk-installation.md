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
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="b729d-103">Установка SDKs Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b729d-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="b729d-104">SDKs Microsoft Graph доступны для включаемого в проекты с помощью GitHub и популярных менеджеров пакетов платформы.</span><span class="sxs-lookup"><span data-stu-id="b729d-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="b729d-105">В этом разделе описывается, как можно установить SDK Microsoft Graph в проект.</span><span class="sxs-lookup"><span data-stu-id="b729d-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="b729d-106">Установка SDK Microsoft Graph .NET</span><span class="sxs-lookup"><span data-stu-id="b729d-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="b729d-107">SDK Microsoft Graph .NET включен в следующие пакеты NuGet:</span><span class="sxs-lookup"><span data-stu-id="b729d-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="b729d-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `v1.0` свободного API.</span><span class="sxs-lookup"><span data-stu-id="b729d-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="b729d-109">Microsoft.Graph имеет зависимость от Microsoft.Graph.Core.</span><span class="sxs-lookup"><span data-stu-id="b729d-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="b729d-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `beta` свободного API.</span><span class="sxs-lookup"><span data-stu-id="b729d-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="b729d-111">Microsoft.Graph.Beta имеет зависимость от Microsoft.Graph.Core.</span><span class="sxs-lookup"><span data-stu-id="b729d-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="b729d-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — основная библиотека для звонков в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b729d-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="b729d-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) — предоставляет обертку сценариев проверки подлинности в Библиотеке проверки подлинности Майкрософт (MSAL) для использования в SDK Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b729d-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="b729d-114">Microsoft.Graph.Auth имеет зависимость от Microsoft.Graph.Core.</span><span class="sxs-lookup"><span data-stu-id="b729d-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="b729d-115">Для установки пакетов Microsoft.Graph [в проект](/nuget/quickstart/install-and-use-a-package-in-visual-studio) можно диспетчер пакетов пользовательского интерфейса Visual Studio или консоли диспетчер пакетов консоли.</span><span class="sxs-lookup"><span data-stu-id="b729d-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="b729d-116">Следующие команды диспетчер пакетов консоли установят библиотеки Microsoft.Graph, Microsoft.Graph.Core и Microsoft.Graph.Auth.</span><span class="sxs-lookup"><span data-stu-id="b729d-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="b729d-117">Microsoft.Graph.Core устанавливается в зависимости от Microsoft.Graph.</span><span class="sxs-lookup"><span data-stu-id="b729d-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="b729d-118">Установка SDK Microsoft Graph Java</span><span class="sxs-lookup"><span data-stu-id="b729d-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="b729d-119">SDK Microsoft Graph Java включен в следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="b729d-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="b729d-120">[Microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `v1.0` свободного API.</span><span class="sxs-lookup"><span data-stu-id="b729d-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="b729d-121">[Microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) — содержит модели и запрашивает у строителей доступ к конечной точке с `beta` помощью свободного API.</span><span class="sxs-lookup"><span data-stu-id="b729d-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span>
- <span data-ttu-id="b729d-122">[Microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) — основная библиотека для звонков в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b729d-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="b729d-123">[Microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) — предоставляет оболочку для проверки подлинности на основе сценария Microsoft Authentication Library (MSAL) для использования с помощью SDK Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b729d-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="b729d-124">Установка SDK Microsoft Graph Java с помощью Gradle</span><span class="sxs-lookup"><span data-stu-id="b729d-124">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="b729d-125">Добавьте репозиторий и зависимость компиляции для microsoft-graph в сборку проекта.gradle:</span><span class="sxs-lookup"><span data-stu-id="b729d-125">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```Gradle
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:3.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="b729d-126">Установка SDK Microsoft Graph Java через Maven</span><span class="sxs-lookup"><span data-stu-id="b729d-126">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="b729d-127">Добавление репозиториев в `profiles` элементе pom.xml:</span><span class="sxs-lookup"><span data-stu-id="b729d-127">Add the repositories in the `profiles` element in pom.xml:</span></span>

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

<span data-ttu-id="b729d-128">Добавьте зависимость в `dependencies` элементе pom.xml:</span><span class="sxs-lookup"><span data-stu-id="b729d-128">Add the dependency in the `dependencies` element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[3.0,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="b729d-129">Установка SDK Javascript Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b729d-129">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="b729d-130">SDK Javascript Microsoft Graph включен в следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="b729d-130">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="b729d-131">@microsoft/microsoft-graph-client[(npm)](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)— основная библиотека для звонков в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b729d-131">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="b729d-132">@microsoft/microsoft-graph-types[(npm)](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)— типы typescript для сущностям Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b729d-132">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="b729d-133">Вы можете использовать [npm](https://www.npmjs.com) для установки SDK Javascript Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="b729d-133">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="b729d-134">Установка SDK Microsoft Graph Objective-C</span><span class="sxs-lookup"><span data-stu-id="b729d-134">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="b729d-135">SDK Microsoft Graph Objective-C поддерживает платформы iOS и macOS и может быть установлен в проект с помощью cocoaPods или Carthage.</span><span class="sxs-lookup"><span data-stu-id="b729d-135">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="b729d-136">Установка SDK Microsoft Graph Objective-C с помощью Cocoapods</span><span class="sxs-lookup"><span data-stu-id="b729d-136">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="b729d-137">Добавьте следующую строку в podfile, чтобы включить SDK Microsoft Graph Objective-C и Microsoft Graph Objective-C Auth SDK в проект xcode:</span><span class="sxs-lookup"><span data-stu-id="b729d-137">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="b729d-138">Установка SDK Microsoft Graph Objective-C с помощью carthage</span><span class="sxs-lookup"><span data-stu-id="b729d-138">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="b729d-139">Выполните следующие действия, чтобы установить SDK Microsoft Graph Objective-C и Microsoft Graph Objective-C Auth SDK с помощью диспетчера пакетов [Carthage.](https://github.com/Carthage/Carthage)</span><span class="sxs-lookup"><span data-stu-id="b729d-139">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="b729d-140">Создайте **картфиль,** который указывает репозиторий Objective-C SDK GitHub и тег [выпуска](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) для целевого адреса.</span><span class="sxs-lookup"><span data-stu-id="b729d-140">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="b729d-141">Запуск `carthage update` .</span><span class="sxs-lookup"><span data-stu-id="b729d-141">Run `carthage update`.</span></span> <span data-ttu-id="b729d-142">Это позволит извлечь зависимости в папку Картидж/Проверка, а затем создает библиотеку MSGraphClientSDK.</span><span class="sxs-lookup"><span data-stu-id="b729d-142">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="b729d-143">Используя Xcode, в вкладке  Общие параметры целевого приложения в разделе Linked **Frameworks and Libraries** перетащите и отклоняйте папку **MSGraphClientSDK.framework** и **MSGraphMSALAuthProvider.framework** из папки Carthage/Build на диске.</span><span class="sxs-lookup"><span data-stu-id="b729d-143">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="b729d-144">На вкладке Параметры **этапов** сборки целевого приложения щелкните значок и **+** выберите новую **фазу сценария запуска.**</span><span class="sxs-lookup"><span data-stu-id="b729d-144">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="b729d-145">Создайте сценарий запуска, в котором укажите оболочку (например: /bin/sh), и добавьте в сценарий следующее содержимое:</span><span class="sxs-lookup"><span data-stu-id="b729d-145">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="b729d-146">Добавьте пути к фреймворкам, которые необходимо использовать в **вводимых файлах.**</span><span class="sxs-lookup"><span data-stu-id="b729d-146">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="b729d-147">Установка SDK PHP Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b729d-147">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="b729d-148">[SDK PHP Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-php) [](https://packagist.org/packages/microsoft/microsoft-graph) доступен из packagist.org и может быть установлен следующим образом:</span><span class="sxs-lookup"><span data-stu-id="b729d-148">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="b729d-149">Установка SDK PHP Microsoft Graph вручную с помощью композитора</span><span class="sxs-lookup"><span data-stu-id="b729d-149">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="b729d-150">Установка SDK PHP Microsoft Graph с composer.js</span><span class="sxs-lookup"><span data-stu-id="b729d-150">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="b729d-151">Установка SDK Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="b729d-151">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="b729d-152">См. [установку SDK Microsoft Graph PowerShell.](../powershell/installation.md)</span><span class="sxs-lookup"><span data-stu-id="b729d-152">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="b729d-153">Установка SDK Microsoft Graph Ruby</span><span class="sxs-lookup"><span data-stu-id="b729d-153">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="b729d-154">[SDK Microsoft Graph Ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) [доступен](https://rubygems.org/) из rubygems.org и может быть установлен с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="b729d-154">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
