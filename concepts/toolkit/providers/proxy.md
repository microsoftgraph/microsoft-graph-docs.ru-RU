---
title: Поставщик прокси
description: Поставщик прокси-сервера позволяет использовать собственную проверку подлинности на стороне сервера с microsoft Graph набор средств.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c62718471c361cd9537bc8ee098c33e7b65830ec
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092255"
---
# <a name="proxy-provider"></a>Поставщик прокси

При использовании поставщика прокси-сервера можно использовать серверную проверку подлинности (например, поток "От имени" Auth2.0) для работы microsoft Graph набор средств путем маршрутизации всех вызовов в Microsoft Graph через собственный сервер.

Во второй службе должен быть доступ к API, который будет вызываться для каждого вызова Microsoft Graph. Например, когда компонент пытается получить ресурс, ProxyProvider будет вызывать базовый API и прибавлять этот ресурс.

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

После этого реализация API должна вызывать Microsoft Graph от имени пользователя и возвращать результаты компоненту.

Пример реализации см. в примере [ASP.NET MVC.](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc) 

Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).

## <a name="get-started"></a>Начало работы

Поставщик прокси-сервера можно инициализировать в HTML или JavaScript. Это следует сделать только один раз для каждой страницы.

### <a name="initialize-in-your-html-page"></a>Инициализация на HTML-странице

Инициализация поставщика прокси-сервера в HTML является простейшим способом определения собственного маршрута для пользовательской проверки подлинности на стороне сервера. С помощью `mgt-proxy-provider` компонента можно настроить **url-адрес graph-proxy-url.** При этом определенный поставщик прокси-сервера будет установлен в качестве глобального поставщика.

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| Атрибут | Описание |
| --- | --- |
| graph-proxy-url  | Базовый URL-адрес прокси-API. |


### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить дополнительные параметры, инициализируя поставщика в JavaScript.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

При желании можно отправлять дополнительные заголовки с каждым запросом в прокси-API, используя дополнительную функцию в качестве второго параметра в конструкторе.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

Это полезно, если вам нужно передать маркеры или другие заглавные символы на ваш тыл.

Если вы будете использовать компонент, необходимо также указать и функции `mgt-login` `login` для `logout` поставщика:

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

