---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint для обеспечения доступа к компонентам с помощью Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: bb657e8fb5d6d9a775fb41e5c5c9fa6bf4662926
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657298"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="abe64-103">Поставщик SharePoint</span><span class="sxs-lookup"><span data-stu-id="abe64-103">SharePoint provider</span></span>

<span data-ttu-id="abe64-104">Используйте поставщика SharePoint в веб-частях SharePoint для обеспечения доступа к компонентам с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="abe64-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="abe64-105">Дополнительные информацию о поставщиках проверки подлинности см. [в этой теме.](./providers.md)</span><span class="sxs-lookup"><span data-stu-id="abe64-105">To learn more about authentication providers, see [Providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="abe64-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="abe64-106">Get started</span></span>

<span data-ttu-id="abe64-107">Инициализация поставщика в `onInit()` методе веб-части.</span><span class="sxs-lookup"><span data-stu-id="abe64-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="abe64-108">Теперь вы можете добавить в метод любой компонент, который будет использовать контекст `render()` SharePoint для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="abe64-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

><span data-ttu-id="abe64-109">**Примечание.** Для набор средств Microsoft Graph требуется Typescript 3.x.</span><span class="sxs-lookup"><span data-stu-id="abe64-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="abe64-110">Убедитесь, что вы используете поддерживаемую версию Typescript, [установив правильный компилятор.](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)</span><span class="sxs-lookup"><span data-stu-id="abe64-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="abe64-111">Пример</span><span class="sxs-lookup"><span data-stu-id="abe64-111">Sample</span></span>

<span data-ttu-id="abe64-112">Сведения о том, как инклиализировать поставщика SharePoint, см. в руководстве по началу работы с веб-частью "Создание веб-части [SharePoint".](../get-started/build-a-sharepoint-web-part.md)</span><span class="sxs-lookup"><span data-stu-id="abe64-112">For details about how to initalize the SharePoint provider, see the [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md) getting started guide.</span></span>

<span data-ttu-id="abe64-113">Встроенный пример использования различных компонентов в веб-частях SharePoint см. в примере веб-части [SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) в репозитории Microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="abe64-113">For a pre-built example that shows you how to use the various components in your SharePoint web parts, see the [SharePoint web part sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) in the Microsoft Graph Toolkit repository.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="abe64-114">Тестирование в workbench</span><span class="sxs-lookup"><span data-stu-id="abe64-114">Test in the workbench</span></span>

<span data-ttu-id="abe64-115">Если вы только начинаете работу с веб-частями SharePoint, вы можете следовать указаниям по созданию [первой веб-части.](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)</span><span class="sxs-lookup"><span data-stu-id="abe64-115">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="abe64-116">После создания веб-части и готовности к использованию компонентов необходимо убедиться, что у веб-части есть необходимые разрешения на доступ к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="abe64-116">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="abe64-117">Подробные сведения [см. в записи "Использовать Microsoft Graph" в SharePoint Framework.](/sharepoint/dev/spfx/use-aad-tutorial)</span><span class="sxs-lookup"><span data-stu-id="abe64-117">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="abe64-118">Одним словом, важно добавить в него нужное `package-solution.json` разрешение.</span><span class="sxs-lookup"><span data-stu-id="abe64-118">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="abe64-119">Вам потребуется отправить пакет веб-части в SharePoint и попросить администратора утвердить запрашиваемую разрешения.</span><span class="sxs-lookup"><span data-stu-id="abe64-119">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

>[!TIP]
><span data-ttu-id="abe64-120">Руководство по началу работы с веб-частью "Создание веб-части [SharePoint"](../get-started/build-a-sharepoint-web-part.md#configure-permissions) содержит пошаговую инструкцию по настройке и одобрению разрешений.</span><span class="sxs-lookup"><span data-stu-id="abe64-120">The [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) getting started guide provides step-by-step instructions for configuring and approving permissions.</span></span>

><span data-ttu-id="abe64-121">**Примечание.** Если вы не знаете, какие разрешения нужно добавить, документация для каждого компонента включает все необходимые ему разрешения.</span><span class="sxs-lookup"><span data-stu-id="abe64-121">**Note:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>

## <a name="polyfills"></a><span data-ttu-id="abe64-122">Polyfills</span><span class="sxs-lookup"><span data-stu-id="abe64-122">Polyfills</span></span>

<span data-ttu-id="abe64-123">Если планируется поддержка IE11 в веб-части SPFx, необходимо использовать полизаполнеки.</span><span class="sxs-lookup"><span data-stu-id="abe64-123">If you plan to support IE11 in your SPFx webparts, you must use polyfills.</span></span>

<span data-ttu-id="abe64-124">Дополнительные данные [см. в этой](../get-started/overview.md#polyfills)набор средств.</span><span class="sxs-lookup"><span data-stu-id="abe64-124">To learn more, see [Getting started with Microsoft Graph Toolkit](../get-started/overview.md#polyfills).</span></span>
