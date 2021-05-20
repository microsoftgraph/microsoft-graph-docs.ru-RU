---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint, чтобы предоставить компонентам доступ к Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c052c3a5bc790b7e9e4316c4a8a8aac4d2d3d7dd
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579692"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="e5ef1-103">Поставщик SharePoint</span><span class="sxs-lookup"><span data-stu-id="e5ef1-103">SharePoint provider</span></span>

<span data-ttu-id="e5ef1-104">Используйте поставщика SharePoint в веб-частях SharePoint, чтобы предоставить компонентам доступ к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="e5ef1-105">Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="e5ef1-105">To learn more about authentication providers, see [Providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="e5ef1-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="e5ef1-106">Get started</span></span>

<span data-ttu-id="e5ef1-107">Инициализируйте поставщика в методе `onInit()` веб-части.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt-spfx';

// add the onInit() method if not already there in your web part class
protected async onInit() {
  Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="e5ef1-108">Теперь вы можете добавить любой компонент в метод `render()` и использовать контекст SharePoint для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts
public render(): void {
  this.domElement.innerHTML = `
    <mgt-agenda></mgt-agenda>
    `;
}
```

><span data-ttu-id="e5ef1-109">**Примечание:** Microsoft Graph набор средств typescript 3.7 или более новый.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.7 or newer.</span></span> <span data-ttu-id="e5ef1-110">Убедитесь, что вы используете поддерживаемую версию TypeScript, [установив соответствующий компилятор](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="e5ef1-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="e5ef1-111">Пример</span><span class="sxs-lookup"><span data-stu-id="e5ef1-111">Sample</span></span>

<span data-ttu-id="e5ef1-112">Сведения о том, как инициализировать SharePoint поставщика, см. в руководстве [Сборка](../get-started/build-a-sharepoint-web-part.md) SharePoint веб-части.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-112">For details about how to initialize the SharePoint provider, see the [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md) getting started guide.</span></span>

<span data-ttu-id="e5ef1-113">Пример готовой веб-части, в котором показано, как использовать различные компоненты в веб-частях SharePoint, см. в статье [Пример веб-части SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) в репозитории Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-113">For a pre-built example that shows you how to use the various components in your SharePoint web parts, see the [SharePoint web part sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) in the Microsoft Graph Toolkit repository.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="e5ef1-114">Тестирование на рабочем месте</span><span class="sxs-lookup"><span data-stu-id="e5ef1-114">Test in the workbench</span></span>

<span data-ttu-id="e5ef1-115">Если вы только начинаете работать с веб-частями SharePoint, следуйте руководству в статье [Создайте свою первую веб-часть](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span><span class="sxs-lookup"><span data-stu-id="e5ef1-115">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="e5ef1-116">Когда вы создадите веб-часть и будете готовы использовать компоненты, убедитесь, что веб-часть имеет соответствующие разрешения для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-116">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="e5ef1-117">Подробнее см. в статье [Использование Microsoft Graph в SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial)</span><span class="sxs-lookup"><span data-stu-id="e5ef1-117">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="e5ef1-118">Другими словами, к `package-solution.json` важно добавить соответствующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-118">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="e5ef1-119">Вам нужно будет отправить пакет веб-части в SharePoint, чтобы администратор утвердил запрошенные разрешения.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-119">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

>[!TIP]
><span data-ttu-id="e5ef1-120">Руководство по началу работы [Создание веб-части SharePoint](../get-started/build-a-sharepoint-web-part.md#configure-permissions) содержит пошаговые инструкции по настройке и утверждению разрешений.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-120">The [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) getting started guide provides step-by-step instructions for configuring and approving permissions.</span></span>

><span data-ttu-id="e5ef1-121">**Примечание.** Если вы не знаете точно, какие разрешения следует добавить, все разрешения, необходимые для каждого компонента, указаны в документации по нему.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-121">**Note:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>

## <a name="polyfills"></a><span data-ttu-id="e5ef1-122">Полизаполнение</span><span class="sxs-lookup"><span data-stu-id="e5ef1-122">Polyfills</span></span>

<span data-ttu-id="e5ef1-123">Если вы планируете поддерживать IE11 в веб-частях SPFx, необходимо использовать полизаполнение.</span><span class="sxs-lookup"><span data-stu-id="e5ef1-123">If you plan to support IE11 in your SPFx webparts, you must use polyfills.</span></span>

<span data-ttu-id="e5ef1-124">Дополнительные сведения см. в статье [Начало работы с Microsoft Graph Toolkit](../get-started/overview.md#polyfills).</span><span class="sxs-lookup"><span data-stu-id="e5ef1-124">To learn more, see [Getting started with Microsoft Graph Toolkit](../get-started/overview.md#polyfills).</span></span>
