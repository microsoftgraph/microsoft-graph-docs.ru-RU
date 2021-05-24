---
title: SharePoint Framework для Microsoft Graph набор средств
description: Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 5868f9fd523055d50f985f2fc8c8840563d56b28
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629492"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a><span data-ttu-id="ed7d0-103">SharePoint Framework для Microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="ed7d0-103">SharePoint Framework library for Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ed7d0-104">Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-104">Use the SharePoint Framework library for Microsoft Graph Toolkit to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

<span data-ttu-id="ed7d0-105">Чтобы запретить нескольким компонентам регистрировать собственный набор компонентов Microsoft Graph набор средств на странице, следует развернуть эту библиотеку для клиента и ссылаться на компоненты Microsoft Graph набор средств, которые вы используете в решении из этой библиотеки.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-105">To prevent multiple components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy this library to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this library.</span></span>

## <a name="installation"></a><span data-ttu-id="ed7d0-106">Установка</span><span class="sxs-lookup"><span data-stu-id="ed7d0-106">Installation</span></span>

<span data-ttu-id="ed7d0-107">Чтобы загрузить компоненты microsoft Graph набор средств из библиотеки, добавьте пакет в качестве зависимости от времени работы в `@microsoft/mgt-spfx` SharePoint Framework проект:</span><span class="sxs-lookup"><span data-stu-id="ed7d0-107">To load Microsoft Graph Toolkit components from the library, add the `@microsoft/mgt-spfx` package as a runtime dependency to your SharePoint Framework project:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

<span data-ttu-id="ed7d0-108">или</span><span class="sxs-lookup"><span data-stu-id="ed7d0-108">or</span></span>

```bash
yarn add @microsoft/mgt-spfx
```

<span data-ttu-id="ed7d0-109">Перед развертывание SharePoint Framework пакета для клиента необходимо развернуть SharePoint Framework `@microsoft/mgt-spfx` для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-109">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the `@microsoft/mgt-spfx` SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="ed7d0-110">Вы можете скачать пакет, соответствующий версии, используемой в проекте, из раздела `@microsoft/mgt-spfx` [Выпуски](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) на GitHub.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-110">You can download the package corresponding to the version of `@microsoft/mgt-spfx` that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="ed7d0-111">Поскольку в клиенте SharePoint Framework может быть установлена только одна версия библиотеки Graph набор средств Microsoft, прежде чем использовать microsoft Graph набор средств в решении, определите, имеет ли ваша организация или клиент уже развернута версия библиотеки SharePoint Framework и использовать ту же версию.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-111">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

## <a name="usage"></a><span data-ttu-id="ed7d0-112">Usage</span><span class="sxs-lookup"><span data-stu-id="ed7d0-112">Usage</span></span>

<span data-ttu-id="ed7d0-113">При создании SharePoint Framework веб-частей и расширений ссылайся на microsoft Graph набор средств `Provider` и `SharePointProvider` из `@microsoft/mgt-spfx` пакета.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-113">When building SharePoint Framework web parts and extensions, reference the Microsoft Graph Toolkit `Provider` and `SharePointProvider` from the `@microsoft/mgt-spfx` package.</span></span> <span data-ttu-id="ed7d0-114">Это позволит вашему решению использовать компоненты Microsoft Graph набор средств, которые уже зарегистрированы на странице, а не мгновенное их использование.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-114">This will ensure that your solution will use Microsoft Graph Toolkit components that are already registered on the page, rather than instantiating its own.</span></span> <span data-ttu-id="ed7d0-115">Процесс мгновенной обработки является одинаковым для всех веб-частей независимо от используемой ими платформы JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-115">The instantiation process is the same for all web parts no matter which JavaScript framework they use.</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';

// [...] trimmed for brevity

export default class MgtWebPart extends BaseClientSideWebPart<IMgtWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  // [...] trimmed for brevity
}
```

<span data-ttu-id="ed7d0-116">При создании веб-частей с помощью фреймворка, кроме React, можно загружать компоненты непосредственно в веб-части:</span><span class="sxs-lookup"><span data-stu-id="ed7d0-116">When building web parts using a framework other than React, you can load components directly in your web part:</span></span>

```ts
export default class MgtNoFrameworkWebPart extends BaseClientSideWebPart<IMgtNoFrameworkWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  public render(): void {
    this.domElement.innerHTML = `
      <div>
        <mgt-person person-query="me"></mgt-person>
      </div>`;
  }

  // [...] trimmed for brevity
}
```

### <a name="react"></a><span data-ttu-id="ed7d0-117">React</span><span class="sxs-lookup"><span data-stu-id="ed7d0-117">React</span></span>

<span data-ttu-id="ed7d0-118">Если вы строите веб-часть с React, вы можете использовать `@microsoft/mgt-react` пакет.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-118">If you're building a web part using React, you can use the `@microsoft/mgt-react` package.</span></span> <span data-ttu-id="ed7d0-119">Однако не забудьте импортировать React компонентов с `@microsoft/mgt-react/dist/es6/spfx` пути.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-119">However, make sure to import all React components from the `@microsoft/mgt-react/dist/es6/spfx` path.</span></span> <span data-ttu-id="ed7d0-120">Это гарантирует, что ваше решение будет использовать только компоненты Microsoft Graph набор средств, которые уже зарегистрированы на странице, а не мгновенное ее собственное.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-120">This will ensure that your solution will only use Microsoft Graph Toolkit components that are already registered on the page, rather than instantiating its own.</span></span>

```tsx
import { Person } from '@microsoft/mgt-react/dist/es6/spfx';
import { ViewType } from '@microsoft/mgt-spfx';

// [...] trimmed for brevity

export default class MgtReact extends React.Component<IMgtReactProps, {}> {
  public render(): React.ReactElement<IMgtReactProps> {
    return (
      <div className={ styles.mgtReact }>
        <Person personQuery="me" view={ViewType.image}></Person>
      </div>
    );
  }
}
```

>[!IMPORTANT]
> <span data-ttu-id="ed7d0-121">Убедитесь, что все Graph набор средств Майкрософт в вашем решении являются либо из:</span><span class="sxs-lookup"><span data-stu-id="ed7d0-121">Make sure all Microsoft Graph Toolkit imports in your solution are from either:</span></span>
> * <span data-ttu-id="ed7d0-122">`@microsoft/mgt-spfx` или </span><span class="sxs-lookup"><span data-stu-id="ed7d0-122">`@microsoft/mgt-spfx` or</span></span>
> * `@microsoft/mgt-react/dist/es6/spfx`
> 
> <span data-ttu-id="ed7d0-123">Не импортируйте из других пакетов Microsoft Graph набор средств (), чтобы избежать упаковки собственной копии инструментария и столкновения с `@microsoft/mgt-*` общей библиотекой.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-123">Do not import from any other Microsoft Graph Toolkit packages (`@microsoft/mgt-*`) to avoid packaging your own copy of the toolkit and colliding with the shared library.</span></span>

## <a name="see-also"></a><span data-ttu-id="ed7d0-124">См. также</span><span class="sxs-lookup"><span data-stu-id="ed7d0-124">See also</span></span>

* [<span data-ttu-id="ed7d0-125">Создайте SharePoint веб-часть с помощью microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="ed7d0-125">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>](./build-a-sharepoint-web-part.md)
* [<span data-ttu-id="ed7d0-126">Сведения о поставщиках проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ed7d0-126">Learn about authentication providers</span></span>](../providers/providers.md)
