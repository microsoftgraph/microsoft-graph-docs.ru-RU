---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint, чтобы включить в себя доступ к компонентам Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e9cf69d26f68da0393f1ef1ecd92683cb9efdd39
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955766"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="4208a-103">Поставщик SharePoint</span><span class="sxs-lookup"><span data-stu-id="4208a-103">SharePoint provider</span></span>

<span data-ttu-id="4208a-104">Используйте поставщика SharePoint в веб-частях SharePoint, чтобы включить в себя доступ к компонентам Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4208a-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="4208a-105">Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="4208a-105">To learn more, see [Providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="4208a-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="4208a-106">Get started</span></span>

<span data-ttu-id="4208a-107">Инициализируйте поставщик в `onInit()` методе веб-части.</span><span class="sxs-lookup"><span data-stu-id="4208a-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt/dist/commonjs';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="4208a-108">Теперь вы можете добавить любой компонент в `render()` метод, который будет использовать контекст SharePoint для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4208a-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

><span data-ttu-id="4208a-109">**Примечание:** Набор средств Microsoft Graph требует typescript 3. x.</span><span class="sxs-lookup"><span data-stu-id="4208a-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="4208a-110">Чтобы убедиться, что вы используете поддерживаемую версию typescript, [установите правильный компилятор](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="4208a-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="4208a-111">Пример</span><span class="sxs-lookup"><span data-stu-id="4208a-111">Sample</span></span>

<span data-ttu-id="4208a-112">Пример использования различных компонентов в веб-частях SharePoint представлен в [примере веб-части SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) в репозитории набора средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4208a-112">For an example that shows you how to use the various components in your SharePoint web parts, see the [SharePoint webpart sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) in the Microsoft Graph Toolkit repository.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="4208a-113">Тестирование в Workbench</span><span class="sxs-lookup"><span data-stu-id="4208a-113">Test in the workbench</span></span>

<span data-ttu-id="4208a-114">Если вы только начинаете работать с веб-частями SharePoint, вы можете воспользоваться инструкциями по [созданию первой веб-части](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) .</span><span class="sxs-lookup"><span data-stu-id="4208a-114">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="4208a-115">После создания веб-части и готовности к использованию компонентов необходимо убедиться, что веб-часть имеет необходимые разрешения для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4208a-115">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="4208a-116">Дополнительные сведения см. [в статье Использование Microsoft Graph в SharePoint Framework](https://docs.microsoft.com/sharepoint/dev/spfx/use-aad-tutorial).</span><span class="sxs-lookup"><span data-stu-id="4208a-116">For details, see [Consume Microsoft Graph in the SharePoint Framework](https://docs.microsoft.com/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="4208a-117">Коротко говоря, важно добавить правое разрешение для `package-solution.json`.</span><span class="sxs-lookup"><span data-stu-id="4208a-117">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="4208a-118">Вам потребуется отправить пакет веб-части в SharePoint и разрешить администратору утверждать запрошенные разрешения.</span><span class="sxs-lookup"><span data-stu-id="4208a-118">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

><span data-ttu-id="4208a-119">**Совет.** если вы не знаете, какие разрешения следует добавить, документация для каждого компонента включает все необходимые разрешения.</span><span class="sxs-lookup"><span data-stu-id="4208a-119">**Tip:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>
