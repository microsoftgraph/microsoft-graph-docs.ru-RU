---
title: Поставщики набора средств Microsoft Graph
description: Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4b51fdf91fd37c0c3dc5ea0ec49571a8ed4e5d47
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086649"
---
# <a name="microsoft-graph-toolkit-providers"></a>Поставщики набора средств Microsoft Graph

Поставщики набора средств Microsoft Graph позволяют приложению выполнять проверку подлинности с помощью Microsoft Identity и получать доступ к Microsoft Graph только в нескольких строках кода. Каждый поставщик управляет проверкой подлинности пользователя и получением маркеров доступа для вызова API Microsoft Graph, поэтому вам не нужно самостоятельно писать этот код. 

Вы можете использовать поставщиков самостоятельно, без компонентов, чтобы быстро реализовать проверку подлинности для приложения и совершать вызовы Microsoft Graph через клиентский пакет SDK для JavaScript.

Поставщики необходимы при использовании компонентов набора инструментов Microsoft Graph, так как компоненты используют их для доступа к Microsoft Graph. Если вы уже обладаете собственной проверкой подлинности и хотите использовать компоненты, вы можете использовать вместо него [настраиваемый поставщик](./providers/custom.md) .

В набор входят следующие поставщики.

|Поставщики|Описание|
|---------|-----------|
|[Msal](./providers/msal.md)|Использует MSAL.js для входа пользователей и получения маркеров для использования с Microsoft Graph в веб-приложении.|
|[SharePoint](./providers/sharepoint.md)|Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.|
|[Teams](./providers/teams.md)|Проверка подлинности и предоставление доступа Microsoft Graph к компонентам в пределах вкладок Microsoft Teams.|
|[Сервера](./providers/proxy.md)|Позволяет использовать внутреннюю проверку подлинности путем маршрутизации всех вызовов Microsoft Graph через серверный сервер.|
|[Custom](./providers/custom.md)|Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph с помощью существующего кода проверки подлинности приложения.|

## <a name="initializing-a-provider"></a>Инициализация поставщика

Чтобы использовать поставщик в своем приложении, необходимо инициализировать новый поставщик, а затем назначить его глобальным поставщиком в пространстве имен providers. Мы рекомендуем сделать это, прежде чем приступать к использованию любого из этих компонентов. Вы можете сделать это одним из двух способов:

**Вариант 1: использование компонента поставщика**

Версию компонента поставщика можно использовать непосредственно в HTML-коде. В фоновом режиме инициализируется новый поставщик, который устанавливается в качестве глобального поставщика. В приведенном ниже примере показано, как использовать Мсалпровидер.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

**Вариант 2: инициализировать в коде**

Инициализация поставщика в коде JavaScript позволяет предоставить дополнительные параметры. Для этого создайте новый экземпляр поставщика и задайте для него значение, которое будет `Providers.globalProvider` использоваться поставщиком. В приведенном ниже примере показано, как использовать Мсалпровидер.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **Примечание:** Сведения о том, как зарегистрировать свое приложение и получить идентификатор клиента, можно найти в статье [Создание приложения Azure Active Directory](./get-started/add-aad-app-registration.md).

## <a name="permission-scopes"></a>Области разрешений

Мы рекомендуем добавить все области разрешений, необходимые приложению для `scopes` атрибута или свойства при инициализации поставщика (это не относится к [поставщику SharePoint](./providers/sharepoint.md)). Это необязательный параметр, но он будет повышать уровень взаимодействия с пользователем, предоставляя пользователю сводный список разрешений, запрошенных всеми компонентами приложения, а не отдельные экраны для каждого компонента. В следующих примерах показано, как это сделать с помощью Мсалпровидер.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

Если вы инициализируем поставщик в коде, предоставьте области разрешений в массиве в `scopes` свойстве.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

Список областей разрешений, необходимых для каждого компонента, можно найти в разделе " **разрешения Microsoft Graph** " на странице документации каждого компонента.

## <a name="provider-state"></a>Состояние поставщика

Поставщик отслеживает состояние проверки подлинности пользователя и передает его компонентам. Например, когда пользователь успешно выполняет вход, он `ProviderState` обновляется `SignedIn` , чтобы сообщить компонентам, которые теперь могут совершать звонки в Microsoft Graph. `ProviderState`Перечисление определяет три состояния, как показано ниже.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

В некоторых случаях потребуется показать некоторые функции или выполнить действие только после успешного входа пользователя. Вы можете получить доступ к состоянию поставщика и проверить его, как показано в следующем примере.

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
Вы также можете использовать этот `Providers.onProviderUpdated` метод для получения уведомлений при изменении состояния поставщика.

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

const providerStateChanged = () => {
  if (Providers.globalProvider.state === ProviderState.SignedIn) {
    // user is now signed in
  }
}

// register a callback for when the state changes
Providers.onProviderUpdated(providerStateChanged);

// remove callback if necessary
Providers.removeProviderUpdatedListener(providerStateChanged);
```

## <a name="getting-an-access-token"></a>Получение маркера доступа

Каждый поставщик предоставляет вызываемую функцию `getAccessToken` , которая может получить текущий маркер доступа или получить новый маркер доступа для предоставленных областей. В приведенном ниже примере показано, как получить новый маркер доступа с `User.Read` областью разрешений.

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Provider.globalProvider.getAccessToken({scopes: 'User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>Выполнение собственных вызовов в Microsoft Graph

Все компоненты могут получать доступ к Microsoft Graph без какой-либо настройки, если вы инициализируем поставщик (как описано в предыдущих разделах). Если вы хотите выполнить собственные вызовы Microsoft Graph, вы можете получить ссылку на тот же пакет SDK Microsoft Graph, который используется компонентами. Сначала получите ссылку на глобальную, `IProvider` а затем используйте объект, `graph` как показано ниже:

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
Возможны случаи, когда необходимо передать дополнительные разрешения в зависимости от вызываемого API. В следующем примере показывается, как это можно сделать.

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a>Использование нескольких поставщиков

В некоторых сценариях приложение будет работать в разных средах и для каждого из них требуется отдельный поставщик. Например, приложение может работать в качестве веб-приложения и вкладки Microsoft Teams, что означает, что вам может потребоваться использовать как Мсалпровидер, так и Теамспровидер. В этом сценарии все компоненты поставщика имеют `depends-on` атрибут для создания резервной цепочки, как показано в следующем примере.

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

В этом сценарии Мсалпровидер будет использоваться только в том случае, если приложение работает в качестве веб-приложения, а Теамспровидер недоступен в текущей среде.

Чтобы сделать то же самое в коде, можно использовать `isAvailable` свойство поставщика, как показано ниже.

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a>Вход и выход пользователя

Если для вашего приложения инициализированы нужные поставщики, можно добавить [компонент входа](./components/login.md) в набор, чтобы быстро и быстро реализовать вход пользователя и выход. Компонент работает с поставщиком, чтобы обрабатывать всю логику проверки подлинности и функции входа и выхода. В следующем примере используется Мсалпровидер и компонент Login.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

В сценариях, где вы хотите реализовать его самостоятельно, а не с помощью компонента входа в набор, вы можете сделать это, используя `login` `logout` методы поставщика.

## <a name="implement-your-own-provider"></a>Реализация собственного поставщика

В сценариях, в которых вы хотите добавить компоненты набора инструментов в приложение с уже существующим кодом проверки подлинности, можно создать настраиваемый поставщик, который будет подключаться к механизму проверки подлинности, а не по предопределенным поставщикам. В наборе инструментов предусмотрено два способа создания новых поставщиков:

- Создайте новый `SimpleProvider` , который возвращает маркер доступа из кода проверки подлинности, передав функцию.
- Расширьте `IProvider` абстрактный класс.

Дополнительные сведения о каждом из них можно найти в разделе [Настраиваемые поставщики](./providers/custom.md).
