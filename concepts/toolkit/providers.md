---
title: Поставщики набора средств Microsoft Graph
description: Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e89247daf92471b4a7c6aa16f34396eaedaaa37a
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243087"
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

- [Мсалпровидер](./providers/msal.md)
- [Шарепоинтпровидер](./providers/sharepoint.md)
- [Теамспровидер](./providers/teams.md)
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

Дополнительные сведения о каждом из них содержатся [](./providers/custom.md) в документации по настраиваемым поставщикам.

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
