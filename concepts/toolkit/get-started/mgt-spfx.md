---
title: SharePoint Framework для Microsoft Graph набор средств
description: Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 17a6e899003dec34a6dac41daaeba7e2c0e3fba1
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579876"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a><span data-ttu-id="9f58d-103">SharePoint Framework для Microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="9f58d-103">SharePoint Framework library for Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9f58d-104">Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.</span><span class="sxs-lookup"><span data-stu-id="9f58d-104">Use the SharePoint Framework library for Microsoft Graph Toolkit to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

<span data-ttu-id="9f58d-105">Чтобы запретить нескольким компонентам регистрировать собственный набор компонентов Microsoft Graph набор средств на странице, следует развернуть эту библиотеку для клиента и ссылаться на компоненты Microsoft Graph набор средств, которые вы используете в решении из этой библиотеки.</span><span class="sxs-lookup"><span data-stu-id="9f58d-105">To prevent multiple components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy this library to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this library.</span></span>

## <a name="installation"></a><span data-ttu-id="9f58d-106">Установка</span><span class="sxs-lookup"><span data-stu-id="9f58d-106">Installation</span></span>

<span data-ttu-id="9f58d-107">Чтобы загрузить компоненты microsoft Graph набор средств из библиотеки, добавьте пакет в качестве зависимости от времени работы в `@microsoft/mgt-spfx` SharePoint Framework проект:</span><span class="sxs-lookup"><span data-stu-id="9f58d-107">To load Microsoft Graph Toolkit components from the library, add the `@microsoft/mgt-spfx` package as a runtime dependency to your SharePoint Framework project:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

<span data-ttu-id="9f58d-108">или</span><span class="sxs-lookup"><span data-stu-id="9f58d-108">or</span></span>

```bash
yarn add @microsoft/mgt-spfx
```

<span data-ttu-id="9f58d-109">Перед развертывание SharePoint Framework пакета для клиента необходимо развернуть SharePoint Framework `@microsoft/mgt-spfx` для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f58d-109">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the `@microsoft/mgt-spfx` SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="9f58d-110">Вы можете скачать пакет, соответствующий версии, используемой в проекте, из раздела `@microsoft/mgt-spfx` [Выпуски](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) на GitHub.</span><span class="sxs-lookup"><span data-stu-id="9f58d-110">You can download the package corresponding to the version of `@microsoft/mgt-spfx` that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="9f58d-111">Поскольку в клиенте SharePoint Framework может быть установлена только одна версия библиотеки Graph набор средств Microsoft, прежде чем использовать microsoft Graph набор средств в решении, определите, имеет ли ваша организация или клиент уже развернута версия библиотеки SharePoint Framework и использовать ту же версию.</span><span class="sxs-lookup"><span data-stu-id="9f58d-111">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

## <a name="usage"></a><span data-ttu-id="9f58d-112">Usage</span><span class="sxs-lookup"><span data-stu-id="9f58d-112">Usage</span></span>

<span data-ttu-id="9f58d-113">При создании SharePoint Framework веб-частей и расширений ссылайся на microsoft Graph набор средств `Provider` и `SharePointProvider` из `@microsoft/mgt-spfx` пакета.</span><span class="sxs-lookup"><span data-stu-id="9f58d-113">When building SharePoint Framework web parts and extensions, reference the Microsoft Graph Toolkit `Provider` and `SharePointProvider` from the `@microsoft/mgt-spfx` package.</span></span> <span data-ttu-id="9f58d-114">Это позволит вашему решению использовать компоненты Microsoft Graph набор средств, которые уже зарегистрированы на странице, а не мгновенное их использование.</span><span class="sxs-lookup"><span data-stu-id="9f58d-114">This will ensure that your solution will use Microsoft Graph Toolkit components that are already registered on the page, rather than instantiating its own.</span></span> <span data-ttu-id="9f58d-115">Процесс мгновенной обработки является одинаковым для всех веб-частей независимо от используемой ими платформы JavaScript.</span><span class="sxs-lookup"><span data-stu-id="9f58d-115">The instantiation process is the same for all web parts no matter which JavaScript framework they use.</span></span>

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

<span data-ttu-id="9f58d-116">При создании веб-частей с помощью фреймворка, кроме React, можно загружать компоненты непосредственно в веб-части:</span><span class="sxs-lookup"><span data-stu-id="9f58d-116">When building web parts using a framework other than React, you can load components directly in your web part:</span></span>

```ts
export default class MgtNoFrameworkWebPart extends BaseClientSideWebPart<IMgtNoFrameworkWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  public render(): void {
    this.domElement.innerHTML = `
      <div class="${styles.mgtNoFramework}">
        <div class="${styles.container}">
          <div class="${styles.row}">
            <div class="${styles.column}">
              <span class="${styles.title}">No framework webpart</span>
              <mgt-person person-query="me" show-name show-email></mgt-person>
            </div>
          </div>
        </div>
      </div>`;
  }

  // [...] trimmed for brevity
}
```

<span data-ttu-id="9f58d-117">Если вы создаете веб-часть с React, загружайте компоненты из `@microsoft/mgt-react` пакета:</span><span class="sxs-lookup"><span data-stu-id="9f58d-117">If you build a web part using React, load components from the `@microsoft/mgt-react` package:</span></span>

```tsx
import { Person } from '@microsoft/mgt-react';

// [...] trimmed for brevity

export default class MgtReact extends React.Component<IMgtReactProps, {}> {
  public render(): React.ReactElement<IMgtReactProps> {
    return (
      <div className={ styles.mgtReact }>
        <Person personQuery="me" />
      </div>
    );
  }
}
```

## <a name="see-also"></a><span data-ttu-id="9f58d-118">См. также</span><span class="sxs-lookup"><span data-stu-id="9f58d-118">See also</span></span>

* [<span data-ttu-id="9f58d-119">Создайте SharePoint веб-часть с помощью microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="9f58d-119">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>](./build-a-sharepoint-web-part.md)
* [<span data-ttu-id="9f58d-120">Сведения о поставщиках проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9f58d-120">Learn about authentication providers</span></span>](../providers/providers.md)
