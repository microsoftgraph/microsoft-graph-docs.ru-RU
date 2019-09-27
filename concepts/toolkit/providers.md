---
title: Поставщики набора средств Microsoft Graph
description: Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 52b0510fdc79253cb2a448b7a454b1dcfaf01bb9
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275726"
---
# <a name="microsoft-graph-toolkit-providers"></a>Поставщики набора средств Microsoft Graph

Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов. Каждый поставщик предоставляет реализацию для получения необходимого маркера доступа для вызова API Microsoft Graph.

Чтобы компоненты использовали поставщика, необходимо присвоить `Providers.globalProvider` свойству значение для поставщика, который вы хотите использовать.

В приведенном ниже примере показано, как использовать Мсалпровидер.

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

В наборе средств реализованы следующие поставщики:

- [мсалпровидер](./providers/msal.md)
- [шарепоинтпровидер](./providers/sharepoint.md)
- [теамспровидер](./providers/teams.md)
- Поставщик надстроек Office (ожидается в ближайшее время)

## <a name="get-started"></a>Начало работы

Вы можете создать поставщика в любое время. Рекомендуется создать поставщика перед использованием любого из компонентов. В этом разделе описывается, как инициализировать поставщика.

`Providers` Глобальная переменная предоставляет следующие свойства и функции

- `globalProvider : IProvider`

Задайте для этого свойства поставщик, который будет использоваться глобально. Все компоненты используют это свойство для получения ссылки на поставщика. При задании этого свойства `onProvidersChanged` событие будет срабатывать.

- `function onProviderUpdated(callbackFunction)`

`callbackFunction` Функция будет вызываться при изменении поставщика или при изменении состояния поставщика. В `ProvidersChangedState` функцию передается значение перечисления, которое указывает, что было обновлено.

## <a name="implement-your-own-provider"></a>Реализация собственного поставщика

В наборе инструментов предусмотрено два способа создания новых поставщиков:

- Создание нового `SimpleProvider` путем передачи функции для получения маркера доступа
- Расширение `IProvider` абстрактного класса

Дополнительные сведения о каждом из них содержатся в документации по [настраиваемым поставщикам](./providers/custom.md) .

## <a name="using-multiple-providers"></a>Использование нескольких поставщиков

В некоторых сценариях приложение будет запускаться в другой среде и потребует другого поставщика. Например, приложение может работать в качестве веб-приложения и вкладки Microsoft Teams, и вам может потребоваться использовать Мсалпровидер и Теамспровидер. В этом сценарии все компоненты поставщика имеют `depends-on` атрибут для создания резервной цепочки, как показано в следующем примере.

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

В этом сценарии Мсалпровидер будет использоваться только в том случае, если Теамспровидер недоступен в текущей среде.

Чтобы сделать то же самое в коде, можно использовать `isAvailable` свойство поставщика, как показано ниже.

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>Выполнение собственных вызовов в Microsoft Graph

Все компоненты могут получать доступ к Microsoft Graph без какой-либо настройки, если вы инициализируем поставщик (как описано в предыдущем разделе). Чтобы получить ссылку на тот же пакет SDK Microsoft Graph, используемый компонентами, сначала получите ссылку на глобальный Ипровидер, а затем используйте `Graph` объект, как показано ниже.

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

Возможны случаи, когда вам потребуется передать дополнительные разрешения в зависимости от интерфейса API, который вы вызываете.

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

`graph` Объект — это экземпляр [пакета SDK JavaScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) , который можно использовать для совершения вызовов Microsoft Graph.
