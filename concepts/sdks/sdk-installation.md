---
title: Установка SDK Graph Microsoft
description: Содержит инструкции по установке C#, Java, Javascript, Objective-C, PHP и Ruby Microsoft Graph SDKs.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 9be84ab8688aa8bc1ad047c2776f30a030611298
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334803"
---
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="77d52-103">Установка SDKs Graph Microsoft</span><span class="sxs-lookup"><span data-stu-id="77d52-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="77d52-104">SDKs Graph Microsoft доступны для включаемой в проекты с помощью GitHub и популярных менеджеров пакетов платформы.</span><span class="sxs-lookup"><span data-stu-id="77d52-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="77d52-105">В этом разделе описывается, как можно установить Graph SDK в проект.</span><span class="sxs-lookup"><span data-stu-id="77d52-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="77d52-106">Установка SDK Graph Microsoft Graph NET</span><span class="sxs-lookup"><span data-stu-id="77d52-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="77d52-107">SDK Graph Microsoft NuGet:</span><span class="sxs-lookup"><span data-stu-id="77d52-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="77d52-108">[Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Содержит модели и запрашивает у строителей доступ к конечной точке с помощью `v1.0` свободного API.</span><span class="sxs-lookup"><span data-stu-id="77d52-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="77d52-109">Microsoft. Graph зависит от Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="77d52-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="77d52-110">[Microsoft. Graph. Бета-версия](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `beta` свободного API.</span><span class="sxs-lookup"><span data-stu-id="77d52-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="77d52-111">Microsoft. Graph. Бета-версия зависит от Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="77d52-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="77d52-112">[Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) — основная библиотека для звонков в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="77d52-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="77d52-113">[Microsoft. Graph. Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) — предоставляет обертку на основе сценариев проверки подлинности в Библиотеке проверки подлинности Майкрософт (MSAL) для использования в microsoft Graph SDK.</span><span class="sxs-lookup"><span data-stu-id="77d52-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="77d52-114">Microsoft. Graph. Auth имеет зависимость от Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="77d52-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="77d52-115">Для установки Microsoft можно использовать [диспетчер пакетов пользовательского](/nuget/quickstart/install-and-use-a-package-in-visual-studio) интерфейса Visual Studio или консоли диспетчер пакетов консоли. Graph пакеты в проект.</span><span class="sxs-lookup"><span data-stu-id="77d52-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="77d52-116">Следующие команды диспетчер пакетов консоли установят Microsoft. Graph, Microsoft. Graph. Core и Microsoft. Graph. Библиотеки Auth.</span><span class="sxs-lookup"><span data-stu-id="77d52-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="77d52-117">Microsoft. Graph. Core устанавливается в зависимости от Microsoft. Graph.</span><span class="sxs-lookup"><span data-stu-id="77d52-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="77d52-118">Установка microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="77d52-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="77d52-119">Microsoft Graph Java SDK входит в следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="77d52-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="77d52-120">[Microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) — содержит модели и запрашивает у строителей доступ к конечной точке с помощью `v1.0` свободного API.</span><span class="sxs-lookup"><span data-stu-id="77d52-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="77d52-121">[Microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) — содержит модели и запрашивает у строителей доступ к конечной точке с `beta` помощью свободного API.</span><span class="sxs-lookup"><span data-stu-id="77d52-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span>
- <span data-ttu-id="77d52-122">[Microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) — основная библиотека для звонков в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="77d52-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="77d52-123">[Microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) — предоставляет обертку сценариев проверки подлинности в Microsoft Authentication Library (MSAL) для использования в microsoft Graph SDK.</span><span class="sxs-lookup"><span data-stu-id="77d52-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="77d52-124">Установка microsoft Graph Java SDK с помощью Gradle</span><span class="sxs-lookup"><span data-stu-id="77d52-124">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="77d52-125">Добавьте репозиторий и зависимость компиляции для microsoft-graph в сборку проекта.gradle:</span><span class="sxs-lookup"><span data-stu-id="77d52-125">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```Gradle
repository {
    mavenCentral()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:4.+'
    // Include Azure identity for authentication
    implementation 'com.azure:azure-identity:1.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="77d52-126">Установка microsoft Graph Java SDK с помощью Maven</span><span class="sxs-lookup"><span data-stu-id="77d52-126">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="77d52-127">Добавьте зависимость в `dependencies` элементе pom.xml:</span><span class="sxs-lookup"><span data-stu-id="77d52-127">Add the dependency in the `dependencies` element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[4.0,)</version>
</dependency>
<dependency>
    <groupId>com.azure</groupId>
    <artifactId>azure-identity</artifactId>
    <version>[1.2,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="77d52-128">Установка SDK Graph Microsoft Graph Javascript</span><span class="sxs-lookup"><span data-stu-id="77d52-128">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="77d52-129">SDK Graph Microsoft Graph javascript включен в следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="77d52-129">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="77d52-130">@microsoft/microsoft-graph-client[(npm)-](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)Основная библиотека для звонков в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="77d52-130">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="77d52-131">@microsoft/microsoft-graph-types[(npm)](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)— типы typescript для сущно-Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="77d52-131">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="77d52-132">Вы можете использовать [npm](https://www.npmjs.com) для установки SDK microsoft Graph Javascript:</span><span class="sxs-lookup"><span data-stu-id="77d52-132">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="77d52-133">Установка SDK Graph Microsoft Graph-C</span><span class="sxs-lookup"><span data-stu-id="77d52-133">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="77d52-134">SDK Graph Microsoft Graph поддерживает платформы iOS и macOS и может быть установлена в проект с помощью cocoaPods или Carthage.</span><span class="sxs-lookup"><span data-stu-id="77d52-134">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="77d52-135">Установка SDK Graph Microsoft Graph-C с помощью Cocoapods</span><span class="sxs-lookup"><span data-stu-id="77d52-135">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="77d52-136">Добавьте следующую строку в podfile, чтобы включить в проект xcode SDK Graph Microsoft Graph Objective-C Auth SDK:</span><span class="sxs-lookup"><span data-stu-id="77d52-136">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="77d52-137">Установка SDK Graph Microsoft Graph-C с помощью Carthage</span><span class="sxs-lookup"><span data-stu-id="77d52-137">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="77d52-138">Выполните следующие действия по установке SDK Graph Microsoft Graph и Microsoft Graph-C Auth SDK с помощью диспетчера пакетов [Carthage.](https://github.com/Carthage/Carthage)</span><span class="sxs-lookup"><span data-stu-id="77d52-138">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="77d52-139">Создайте **картфил,** который указывает целевой тег SDK GitHub и тег [выпуска.](https://github.com/microsoftgraph/msgraph-sdk-objc/releases)</span><span class="sxs-lookup"><span data-stu-id="77d52-139">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="77d52-140">Запустите `carthage update`.</span><span class="sxs-lookup"><span data-stu-id="77d52-140">Run `carthage update`.</span></span> <span data-ttu-id="77d52-141">Это позволит извлечь зависимости в папку Картидж/Проверка, а затем создает библиотеку MSGraphClientSDK.</span><span class="sxs-lookup"><span data-stu-id="77d52-141">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="77d52-142">Используя Xcode, в вкладке  Общие параметры целевого приложения в разделе Linked **Frameworks and Libraries** перетащите и отклоняйте папку **MSGraphClientSDK.framework** и **MSGraphMSALAuthProvider.framework** из папки Carthage/Build на диске.</span><span class="sxs-lookup"><span data-stu-id="77d52-142">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="77d52-143">На вкладке Параметры **этапов** сборки целевого приложения щелкните значок и **+** выберите новую **фазу сценария запуска.**</span><span class="sxs-lookup"><span data-stu-id="77d52-143">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="77d52-144">Создайте сценарий запуска, в котором укажите оболочку (например: /bin/sh), и добавьте в сценарий следующее содержимое:</span><span class="sxs-lookup"><span data-stu-id="77d52-144">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="77d52-145">Добавьте пути к фреймворкам, которые необходимо использовать в **вводимых файлах.**</span><span class="sxs-lookup"><span data-stu-id="77d52-145">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="77d52-146">Установка SDK Graph microsoft Graph PHP</span><span class="sxs-lookup"><span data-stu-id="77d52-146">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="77d52-147">[SDK Graph phP microsoft доступен](https://github.com/microsoftgraph/msgraph-sdk-php) из [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) и может быть установлен следующим образом:</span><span class="sxs-lookup"><span data-stu-id="77d52-147">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="77d52-148">Установка microsoft Graph phP SDK вручную с помощью композитора</span><span class="sxs-lookup"><span data-stu-id="77d52-148">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="77d52-149">Установка SDK Graph microsoft composer.js</span><span class="sxs-lookup"><span data-stu-id="77d52-149">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="77d52-150">Установка SDK Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="77d52-150">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="77d52-151">См. [в рубрике Установка Graph PowerShell SDK](../powershell/installation.md).</span><span class="sxs-lookup"><span data-stu-id="77d52-151">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="77d52-152">Установка SDK Graph Microsoft Graph Ruby</span><span class="sxs-lookup"><span data-stu-id="77d52-152">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="77d52-153">[SDK Graph Microsoft rubygems.org](https://github.com/microsoftgraph/msgraph-sdk-ruby) и может [](https://rubygems.org/) быть установлен с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="77d52-153">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
