---
title: Поставщик прокси
description: Поставщик прокси-сервера позволяет использовать собственную проверку подлинности на стороне сервера с помощью набора средств Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 130811ded21013614c85cc90eea6f22c74e7cc73
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955773"
---
# <a name="proxy-provider"></a><span data-ttu-id="75ae7-103">Поставщик прокси</span><span class="sxs-lookup"><span data-stu-id="75ae7-103">Proxy provider</span></span>

<span data-ttu-id="75ae7-104">При использовании поставщика прокси-сервера вы можете использовать внутреннюю проверку подлинности (например, auth 2.0 on-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of</span><span class="sxs-lookup"><span data-stu-id="75ae7-104">When you use the proxy provider, you can use your backend authentication (such as Auth2.0 On-Behalf-Of flow) to power the Microsoft Graph Toolkit by routing all calls to Microsoft Graph through your own backend.</span></span>

<span data-ttu-id="75ae7-105">Внутренняя служба должна предоставлять API, который будет вызываться для каждого вызова в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="75ae7-105">Your backend service must expose an API that will be called for every call to Microsoft Graph.</span></span> <span data-ttu-id="75ae7-106">Например, когда компонент пытается получить ресурс, Проксипровидер будет вызывать базовый API и добавлять этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="75ae7-106">For example, when a component attempts to get a resource, the ProxyProvider will instead call your base API and append that resource.</span></span>

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

<span data-ttu-id="75ae7-107">Реализация API должна затем вызывать Microsoft Graph от имени пользователя и возвращать результаты в компонент.</span><span class="sxs-lookup"><span data-stu-id="75ae7-107">Your API implementation should then call Microsoft Graph on behalf of the user and return the results to the component.</span></span>

<span data-ttu-id="75ae7-108">Пример реализации представлен в статье [пример ASP.NET MVC](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc).</span><span class="sxs-lookup"><span data-stu-id="75ae7-108">For an implementation example, see the [ASP.NET MVC sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc).</span></span> 

<span data-ttu-id="75ae7-109">Чтобы узнать больше о поставщиках проверки подлинности, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="75ae7-109">To learn more about authentication providers, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="75ae7-110">Начало работы</span><span class="sxs-lookup"><span data-stu-id="75ae7-110">Get started</span></span>

<span data-ttu-id="75ae7-111">Вы можете инициализировать поставщика прокси-сервера в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="75ae7-111">You can initialize the proxy provider in HTML or JavaScript.</span></span> <span data-ttu-id="75ae7-112">Эту операцию следует выполнять только один раз для каждой страницы.</span><span class="sxs-lookup"><span data-stu-id="75ae7-112">You should do this only once per page.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="75ae7-113">Инициализация на HTML-странице</span><span class="sxs-lookup"><span data-stu-id="75ae7-113">Initialize in your HTML page</span></span>

<span data-ttu-id="75ae7-114">Инициализация поставщика прокси-сервера в HTML является самым простым способом определения собственного маршрута для пользовательской проверки подлинности на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="75ae7-114">Initializing the proxy provider in HTML is the simplest way to define your own route for custom server-side authentication.</span></span> <span data-ttu-id="75ae7-115">Используйте `mgt-proxy-provider` компонент, чтобы задать **Graph-proxy-URL**.</span><span class="sxs-lookup"><span data-stu-id="75ae7-115">Use the `mgt-proxy-provider` component to set the **graph-proxy-url**.</span></span> <span data-ttu-id="75ae7-116">В этом случае задается указанный поставщик прокси в качестве глобального поставщика.</span><span class="sxs-lookup"><span data-stu-id="75ae7-116">This will set the defined proxy provider as the global provider.</span></span>

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| <span data-ttu-id="75ae7-117">Атрибут</span><span class="sxs-lookup"><span data-stu-id="75ae7-117">Attribute</span></span> | <span data-ttu-id="75ae7-118">Описание</span><span class="sxs-lookup"><span data-stu-id="75ae7-118">Description</span></span> |
| --- | --- |
| <span data-ttu-id="75ae7-119">Graph-proxy-URL</span><span class="sxs-lookup"><span data-stu-id="75ae7-119">graph-proxy-url</span></span>  | <span data-ttu-id="75ae7-120">Базовый URL-адрес прокси-API.</span><span class="sxs-lookup"><span data-stu-id="75ae7-120">Base URL for the proxy API.</span></span> |


### <a name="initialize-in-javascript"></a><span data-ttu-id="75ae7-121">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="75ae7-121">Initialize in JavaScript</span></span>

<span data-ttu-id="75ae7-122">Вы можете предоставить дополнительные параметры, инициализируя поставщик в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="75ae7-122">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

<span data-ttu-id="75ae7-123">При необходимости можно отправить дополнительные заголовки с каждым запросом на прокси-API, используя необязательную функцию в качестве второго параметра в конструкторе.</span><span class="sxs-lookup"><span data-stu-id="75ae7-123">Optionally, you can send additional headers with each request to your proxy api by using an optional function as the second parameter in the constructor.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

<span data-ttu-id="75ae7-124">Это полезно, когда необходимо передать маркеры или другие заголовки в серверную базу данных.</span><span class="sxs-lookup"><span data-stu-id="75ae7-124">This is useful when you need to pass tokens or other headers to your backend</span></span>

<span data-ttu-id="75ae7-125">Если вы будете использовать `mgt-login` компонент, необходимо также указать функции `login` и `logout` функции для поставщика:</span><span class="sxs-lookup"><span data-stu-id="75ae7-125">If you will be using the `mgt-login` component, you should also specify the `login` and `logout` functions for the provider:</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

