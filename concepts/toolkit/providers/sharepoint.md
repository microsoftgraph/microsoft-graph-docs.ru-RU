---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint, чтобы включить в себя доступ к компонентам Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c27a24ac1b5f41b97d749620edbae09794072bed
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086755"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="73f97-103">Поставщик SharePoint</span><span class="sxs-lookup"><span data-stu-id="73f97-103">SharePoint provider</span></span>

<span data-ttu-id="73f97-104">Используйте поставщика SharePoint в веб-частях SharePoint, чтобы включить в себя доступ к компонентам Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="73f97-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="73f97-105">Чтобы узнать больше о поставщиках проверки подлинности, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="73f97-105">To learn more about authentication providers, see [Providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="73f97-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="73f97-106">Get started</span></span>

<span data-ttu-id="73f97-107">Инициализируйте поставщик в `onInit()` методе веб-части.</span><span class="sxs-lookup"><span data-stu-id="73f97-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="73f97-108">Теперь вы можете добавить любой компонент в `render()` метод, который будет использовать контекст SharePoint для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="73f97-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

><span data-ttu-id="73f97-109">**Примечание:** Набор средств Microsoft Graph требует typescript 3. x.</span><span class="sxs-lookup"><span data-stu-id="73f97-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="73f97-110">Чтобы убедиться, что вы используете поддерживаемую версию typescript, [установите правильный компилятор](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="73f97-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="73f97-111">Пример</span><span class="sxs-lookup"><span data-stu-id="73f97-111">Sample</span></span>

<span data-ttu-id="73f97-112">Подробнее о том, как инитализе поставщика SharePoint, можно узнать в статье Создание руководства по началу работы с [веб-частью SharePoint](../get-started/build-a-sharepoint-web-part.md) .</span><span class="sxs-lookup"><span data-stu-id="73f97-112">For details about how to initalize the SharePoint provider, see the [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md) getting started guide.</span></span>

<span data-ttu-id="73f97-113">Предварительно созданный пример, в котором показано, как использовать различные компоненты в веб-частях SharePoint, можно найти в [примере веб-части SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) в репозитории набора средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="73f97-113">For a pre-built example that shows you how to use the various components in your SharePoint web parts, see the [SharePoint web part sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) in the Microsoft Graph Toolkit repository.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="73f97-114">Тестирование в Workbench</span><span class="sxs-lookup"><span data-stu-id="73f97-114">Test in the workbench</span></span>

<span data-ttu-id="73f97-115">Если вы только начинаете работать с веб-частями SharePoint, вы можете воспользоваться инструкциями по [созданию первой веб-части](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) .</span><span class="sxs-lookup"><span data-stu-id="73f97-115">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="73f97-116">После создания веб-части и готовности к использованию компонентов необходимо убедиться, что веб-часть имеет необходимые разрешения для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="73f97-116">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="73f97-117">Дополнительные сведения см. [в статье Использование Microsoft Graph в SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span><span class="sxs-lookup"><span data-stu-id="73f97-117">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="73f97-118">Коротко говоря, важно добавить правое разрешение для `package-solution.json` .</span><span class="sxs-lookup"><span data-stu-id="73f97-118">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="73f97-119">Вам потребуется отправить пакет веб-части в SharePoint и разрешить администратору утверждать запрошенные разрешения.</span><span class="sxs-lookup"><span data-stu-id="73f97-119">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

>[!TIP]
><span data-ttu-id="73f97-120">Руководство по началу работы с [веб-частью "Создание веб-части SharePoint](../get-started/build-a-sharepoint-web-part.md#configure-permissions) " содержит пошаговые инструкции по настройке и утверждению разрешений.</span><span class="sxs-lookup"><span data-stu-id="73f97-120">The [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) getting started guide provides step-by-step instructions for configuring and approving permissions.</span></span>

><span data-ttu-id="73f97-121">**Примечание.** если вы не знаете, какие разрешения следует добавить, документация для каждого компонента включает все необходимые разрешения.</span><span class="sxs-lookup"><span data-stu-id="73f97-121">**Note:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>

## <a name="polyfills"></a><span data-ttu-id="73f97-122">Polyfills</span><span class="sxs-lookup"><span data-stu-id="73f97-122">Polyfills</span></span>

<span data-ttu-id="73f97-123">Если вы планируете поддерживать IE11 в веб SPFx, необходимо использовать только.</span><span class="sxs-lookup"><span data-stu-id="73f97-123">If you plan to support IE11 in your SPFx webparts, you must use polyfills.</span></span>

<span data-ttu-id="73f97-124">Чтобы узнать больше, ознакомьтесь [со статьей начало работы с набором средств Microsoft Graph](../get-started/overview.md#polyfills).</span><span class="sxs-lookup"><span data-stu-id="73f97-124">To learn more, see [Getting started with Microsoft Graph Toolkit](../get-started/overview.md#polyfills).</span></span>
