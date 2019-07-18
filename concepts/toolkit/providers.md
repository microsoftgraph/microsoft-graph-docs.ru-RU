---
title: Поставщики набора средств Microsoft Graph
description: Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3e5d587e8c2690d2b71a2e70e41266519566f91e
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778714"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="6b653-103">Поставщики набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6b653-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="6b653-104">Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="6b653-104">The Microsoft Graph Toolkit providers enable authentication and Microsoft Graph access for all components.</span></span> <span data-ttu-id="6b653-105">Каждый поставщик предоставляет реализацию для получения необходимого маркера доступа для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6b653-105">Each provider provides implementation for acquiring the necessary access token for calling the Microsoft Graph APIs.</span></span>

<span data-ttu-id="6b653-106">Чтобы компоненты использовали поставщика, необходимо присвоить `Providers.globalProvider` свойству значение для поставщика, который вы хотите использовать.</span><span class="sxs-lookup"><span data-stu-id="6b653-106">For the components to use a provider, you must set the `Providers.globalProvider` property to the value for a provider you'd like to use.</span></span>

<span data-ttu-id="6b653-107">В приведенном ниже примере показано, как использовать Мсалпровидер.</span><span class="sxs-lookup"><span data-stu-id="6b653-107">The following example shows how to use the MsalProvider.</span></span>

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

<span data-ttu-id="6b653-108">В наборе средств реализованы следующие поставщики:</span><span class="sxs-lookup"><span data-stu-id="6b653-108">The toolkit implements the following providers:</span></span>

- [<span data-ttu-id="6b653-109">Мсалпровидер</span><span class="sxs-lookup"><span data-stu-id="6b653-109">MsalProvider</span></span>](./providers/msal.md)
- [<span data-ttu-id="6b653-110">Шарепоинтпровидер</span><span class="sxs-lookup"><span data-stu-id="6b653-110">SharePointProvider</span></span>](./providers/sharepoint.md)
- [<span data-ttu-id="6b653-111">Теамспровидер</span><span class="sxs-lookup"><span data-stu-id="6b653-111">TeamsProvider</span></span>](./providers/teams.md)
- <span data-ttu-id="6b653-112">Поставщик надстроек Office (ожидается в ближайшее время)</span><span class="sxs-lookup"><span data-stu-id="6b653-112">Office Add-ins provider (coming soon)</span></span>

## <a name="get-started"></a><span data-ttu-id="6b653-113">Начало работы</span><span class="sxs-lookup"><span data-stu-id="6b653-113">Get started</span></span>

<span data-ttu-id="6b653-114">Вы можете создать поставщика в любое время.</span><span class="sxs-lookup"><span data-stu-id="6b653-114">You can create a provider at any time.</span></span> <span data-ttu-id="6b653-115">Рекомендуется создать поставщика перед использованием любого из компонентов.</span><span class="sxs-lookup"><span data-stu-id="6b653-115">We recommend that you create the provider before you use any of the components.</span></span> <span data-ttu-id="6b653-116">В этом разделе описывается, как инициализировать поставщика.</span><span class="sxs-lookup"><span data-stu-id="6b653-116">This section describes how to initialize a provider.</span></span>

<span data-ttu-id="6b653-117">`Providers` Глобальная переменная предоставляет следующие свойства и функции</span><span class="sxs-lookup"><span data-stu-id="6b653-117">The `Providers` global variable exposes the following properties and functions</span></span>

- `globalProvider : IProvider`

<span data-ttu-id="6b653-118">Задайте для этого свойства поставщик, который будет использоваться глобально.</span><span class="sxs-lookup"><span data-stu-id="6b653-118">Set this property to a provider that you want to use globally.</span></span> <span data-ttu-id="6b653-119">Все компоненты используют это свойство для получения ссылки на поставщика.</span><span class="sxs-lookup"><span data-stu-id="6b653-119">All components use this property to get a reference to the provider.</span></span> <span data-ttu-id="6b653-120">При задании этого свойства `onProvidersChanged` событие будет срабатывать.</span><span class="sxs-lookup"><span data-stu-id="6b653-120">Setting this property will fire the `onProvidersChanged` event.</span></span>

- `function onProviderUpdated(callbackFunction)`

<span data-ttu-id="6b653-121">`callbackFunction` Функция будет вызываться при изменении поставщика или при изменении состояния поставщика.</span><span class="sxs-lookup"><span data-stu-id="6b653-121">The `callbackFunction` function will be called when a provider is changed or when the state of a provider changes.</span></span> <span data-ttu-id="6b653-122">В `ProvidersChangedState` функцию передается значение перечисления, которое указывает, что было обновлено.</span><span class="sxs-lookup"><span data-stu-id="6b653-122">A `ProvidersChangedState` enum value will be passed to the function to indicate what updated.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="6b653-123">Реализация собственного поставщика</span><span class="sxs-lookup"><span data-stu-id="6b653-123">Implement your own provider</span></span>

<span data-ttu-id="6b653-124">В наборе инструментов предусмотрено два способа создания новых поставщиков:</span><span class="sxs-lookup"><span data-stu-id="6b653-124">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="6b653-125">Создание нового `SimpleProvider` путем передачи функции для получения маркера доступа</span><span class="sxs-lookup"><span data-stu-id="6b653-125">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="6b653-126">Расширение `IProvider` абстрактного класса</span><span class="sxs-lookup"><span data-stu-id="6b653-126">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="6b653-127">Дополнительные сведения о каждом из них содержатся [](./providers/custom.md) в документации по настраиваемым поставщикам.</span><span class="sxs-lookup"><span data-stu-id="6b653-127">Read more about each one in the [custom providers](./providers/custom.md) documentation.</span></span>

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="6b653-128">Выполнение собственных вызовов в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6b653-128">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="6b653-129">Все компоненты могут получать доступ к Microsoft Graph без какой-либо настройки, если вы инициализируем поставщик (как описано в предыдущем разделе).</span><span class="sxs-lookup"><span data-stu-id="6b653-129">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous section).</span></span> <span data-ttu-id="6b653-130">Чтобы получить ссылку на тот же пакет SDK Microsoft Graph, используемый компонентами, сначала получите ссылку на глобальный Ипровидер, а затем используйте `Graph` объект, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="6b653-130">To get a reference to the same Microsoft Graph SDK used by the components, first get a reference to the global IProvider and then use the `Graph` object, as shown.</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

<span data-ttu-id="6b653-131">Возможны случаи, когда вам потребуется передать дополнительные разрешения в зависимости от интерфейса API, который вы вызываете.</span><span class="sxs-lookup"><span data-stu-id="6b653-131">There might be cases were you will need to pass additional permissions, depending on the API you're calling.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

<span data-ttu-id="6b653-132">`graph` Объект — это экземпляр [пакета SDK JavaScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) , который можно использовать для совершения вызовов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6b653-132">The `graph` object is an instance of the [Microsoft Graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) and you can use it to make any calls to Microsoft Graph.</span></span>
