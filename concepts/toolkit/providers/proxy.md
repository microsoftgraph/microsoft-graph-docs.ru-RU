---
title: Поставщик прокси
description: Поставщик прокси позволяет использовать собственную проверку подлинности на стороне сервера с помощью microsoft Graph набор средств.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 44f247cb85dbe7444cfd86928387f510369a4193
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64586799"
---
# <a name="proxy-provider"></a>Поставщик прокси

При использовании поставщика прокси-серверов вы можете использовать проверку подлинности backend (например, поток Auth2.0 On-Behalf-Of) для питания microsoft Graph набор средств путем маршрутизации всех вызовов в Microsoft Graph с помощью собственной задней части.

Служба поддержки должна обнаружить API, который будет вызываться для каждого вызова в Корпорацию Майкрософт Graph. Например, когда компонент пытается получить ресурс, proxyProvider вместо этого будет вызывать базовый API и приложение этого ресурса.

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

Затем реализация API должна вызвать microsoft Graph от имени пользователя и вернуть результаты в компонент.

Пример реализации см. в [примере ASP.NET MVC](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc). 

Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщика прокси в HTML или JavaScript. Это следует делать только один раз на страницу.

### <a name="initialize-in-your-html-page"></a>Инициализация на странице HTML

Инициализация поставщика прокси-серверов в HTML — это самый простой способ определения собственного маршрута для проверки подлинности на стороне сервера. Используйте компонент `mgt-proxy-provider` для набора **url-адреса с графом-прокси-адресом**. Это задает определенный поставщик прокси-серверов в качестве глобального поставщика.

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| Атрибут | Описание |
| --- | --- |
| url-адрес graph-proxy  | Базовый URL-адрес API прокси-сервера. |


### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить больше вариантов, инициализируя поставщика в JavaScript.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

Дополнительно можно отправлять дополнительные заголовки с каждым запросом в прокси-api, используя необязательные функции в качестве второго параметра в конструкторе.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
});
```

Это полезно, когда необходимо передать маркеры или другие заготки в спину.

Если вы будете использовать компонент `mgt-login` , необходимо также указать функции `login` `logout` и функции для поставщика:

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

