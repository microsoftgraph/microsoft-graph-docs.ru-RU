---
title: Поставщик прокси-сервера
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
# <a name="proxy-provider"></a>Поставщик прокси-сервера

При использовании поставщика прокси-сервера вы можете использовать внутреннюю проверку подлинности (например, auth 2.0 on-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of-of

Внутренняя служба должна предоставлять API, который будет вызываться для каждого вызова в Microsoft Graph. Например, когда компонент пытается получить ресурс, Проксипровидер будет вызывать базовый API и добавлять этот ресурс.

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

Реализация API должна затем вызывать Microsoft Graph от имени пользователя и возвращать результаты в компонент.

Пример реализации представлен в статье [пример ASP.NET MVC](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc). 

Чтобы узнать больше о поставщиках проверки подлинности, ознакомьтесь со статьей [поставщики](../providers.md).

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщика прокси-сервера в HTML или JavaScript. Эту операцию следует выполнять только один раз для каждой страницы.

### <a name="initialize-in-your-html-page"></a>Инициализация на HTML-странице

Инициализация поставщика прокси-сервера в HTML является самым простым способом определения собственного маршрута для пользовательской проверки подлинности на стороне сервера. Используйте `mgt-proxy-provider` компонент, чтобы задать **Graph-proxy-URL**. В этом случае задается указанный поставщик прокси в качестве глобального поставщика.

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| Атрибут | Описание |
| --- | --- |
| Graph-proxy-URL  | Базовый URL-адрес прокси-API. |


### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить дополнительные параметры, инициализируя поставщик в JavaScript.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

При необходимости можно отправить дополнительные заголовки с каждым запросом на прокси-API, используя необязательную функцию в качестве второго параметра в конструкторе.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

Это полезно, когда необходимо передать маркеры или другие заголовки в серверную базу данных.

Если вы будете использовать `mgt-login` компонент, необходимо также указать функции `login` и `logout` функции для поставщика:

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

