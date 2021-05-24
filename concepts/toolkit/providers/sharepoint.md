---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint, чтобы предоставить компонентам доступ к Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: eb5e5c5935e51fe7574c41feb57700f473567707
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629128"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="08014-103">Поставщик SharePoint</span><span class="sxs-lookup"><span data-stu-id="08014-103">SharePoint provider</span></span>

<span data-ttu-id="08014-104">Используйте поставщика SharePoint в веб-частях SharePoint, чтобы предоставить компонентам доступ к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="08014-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="08014-105">Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="08014-105">To learn more about authentication providers, see [Providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="08014-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="08014-106">Get started</span></span>

<span data-ttu-id="08014-107">Инициализируйте поставщика в методе `onInit()` веб-части.</span><span class="sxs-lookup"><span data-stu-id="08014-107">Initialize the provider inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="08014-108">В этом примере используется [ `@microsoft/mgt-spfx` пакет](../get-started/mgt-spfx.md).</span><span class="sxs-lookup"><span data-stu-id="08014-108">This example uses the [`@microsoft/mgt-spfx` package](../get-started/mgt-spfx.md).</span></span>

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt-spfx';

// add the onInit() method if not already there in your web part class
protected async onInit() {
  Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="08014-109">Теперь вы можете добавить любой компонент в метод `render()` и использовать контекст SharePoint для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="08014-109">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts
public render(): void {
  this.domElement.innerHTML = `
    <mgt-agenda></mgt-agenda>
    `;
}
```

><span data-ttu-id="08014-110">**Примечание:** Microsoft Graph набор средств typescript 3.7 или более новый.</span><span class="sxs-lookup"><span data-stu-id="08014-110">**Note:** The Microsoft Graph Toolkit requires Typescript 3.7 or newer.</span></span> <span data-ttu-id="08014-111">Убедитесь, что вы используете поддерживаемую версию TypeScript, [установив соответствующий компилятор](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="08014-111">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="08014-112">Пример</span><span class="sxs-lookup"><span data-stu-id="08014-112">Sample</span></span>

<span data-ttu-id="08014-113">Сведения о том, как инициализировать SharePoint поставщика, см. в руководстве [Сборка](../get-started/build-a-sharepoint-web-part.md) SharePoint веб-части.</span><span class="sxs-lookup"><span data-stu-id="08014-113">For details about how to initialize the SharePoint provider, see the [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md) getting started guide.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="08014-114">Тестирование на рабочем месте</span><span class="sxs-lookup"><span data-stu-id="08014-114">Test in the workbench</span></span>

<span data-ttu-id="08014-115">Если вы только начинаете работать с веб-частями SharePoint, следуйте руководству в статье [Создайте свою первую веб-часть](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span><span class="sxs-lookup"><span data-stu-id="08014-115">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="08014-116">Когда вы создадите веб-часть и будете готовы использовать компоненты, убедитесь, что веб-часть имеет соответствующие разрешения для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="08014-116">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="08014-117">Подробнее см. в статье [Использование Microsoft Graph в SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial)</span><span class="sxs-lookup"><span data-stu-id="08014-117">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="08014-118">Другими словами, к `package-solution.json` важно добавить соответствующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="08014-118">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="08014-119">Вам нужно будет отправить пакет веб-части в SharePoint, чтобы администратор утвердил запрошенные разрешения.</span><span class="sxs-lookup"><span data-stu-id="08014-119">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

>[!TIP]
><span data-ttu-id="08014-120">Руководство по началу работы [Создание веб-части SharePoint](../get-started/build-a-sharepoint-web-part.md#configure-permissions) содержит пошаговые инструкции по настройке и утверждению разрешений.</span><span class="sxs-lookup"><span data-stu-id="08014-120">The [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) getting started guide provides step-by-step instructions for configuring and approving permissions.</span></span>

><span data-ttu-id="08014-121">**Примечание.** Если вы не знаете точно, какие разрешения следует добавить, все разрешения, необходимые для каждого компонента, указаны в документации по нему.</span><span class="sxs-lookup"><span data-stu-id="08014-121">**Note:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>