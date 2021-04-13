---
title: Поставщики набор средств Microsoft Graph
description: Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 1bebdb6bd2445873d8b45412b61f8793673db216
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697181"
---
# <a name="microsoft-graph-toolkit-providers"></a>Поставщики набор средств Microsoft Graph

Поставщики набор средств Microsoft Graph позволяют приложению проверить подлинность с помощью Microsoft Identity и получить доступ к Microsoft Graph только в нескольких строках кода. Каждый поставщик обрабатывает проверку подлинности пользователей и приобретает маркеры доступа для вызова API Microsoft Graph, чтобы вам не нужно было самостоятельно писать этот код. 

Вы можете использовать поставщики самостоятельно, без компонентов, чтобы быстро реализовать проверку подлинности для вашего приложения и сделать вызовы в Microsoft Graph через SDK клиента JavaScript.

Поставщики необходимы при использовании компонентов Microsoft Graph набор средств, так как компоненты используют их для доступа к Microsoft Graph. Если у вас уже есть собственная проверка подлинности и вы хотите использовать компоненты, вместо этого можно использовать [настраиваемый поставщик.](./custom.md)

В набор средств входят следующие поставщики.

|Поставщики|Описание|
|---------|-----------|
|[MSAL](./msal.md)|Использует MSAL.js для регистрации пользователей и приобретения маркеров для использования с Помощью Microsoft Graph в веб-приложении.|
|[Электрон](./electron.md)|Проверка подлинности и обеспечивает доступ Microsoft Graph к компонентам в приложениях Electron.|
|[SharePoint](./sharepoint.md)|Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.|
|[Teams](./teams.md)|Проверка подлинности и доступ Microsoft Graph к компонентам на вкладке Microsoft Teams.|
|[Прокси-сервер](./proxy.md)|Позволяет использовать проверку подлинности на внутреннем сервере с помощью маршрутизации всех вызовов Microsoft Graph через внутренний сервер.|
|[Настраиваемый](./custom.md)|Создание настраиваемого поставщика для включения проверки подлинности и доступа к Microsoft Graph с помощью существующего кода проверки подлинности приложения.|

## <a name="initializing-a-provider"></a>Инициализация поставщика

Чтобы использовать поставщика в приложении, необходимо инициализировать нового поставщика, а затем установить его в качестве глобального поставщика в пространстве имен поставщиков. Мы рекомендуем сделать это, прежде чем приступить к использованию любого из компонентов. Это можно сделать одним из двух способов:

**Вариант 1. Использование компонента поставщика**

Компонентную версию поставщика можно использовать непосредственно в HTML. За кулисами новый поставщик инициализируются и устанавливается как глобальный поставщик. В следующем примере показано, как использовать MsalProvider.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

**Вариант 2. Инициализация кода**

Инициализация поставщика в коде JavaScript позволяет предоставить дополнительные параметры. Для этого создайте новый экземпляр поставщика и установите значение свойства поставщику, который вы `Providers.globalProvider` хотите использовать. В следующем примере показано, как использовать MsalProvider.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **Примечание:** Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в материале [Create an Azure Active Directory app.](../get-started/add-aad-app-registration.md)

## <a name="permission-scopes"></a>Области разрешений

Мы рекомендуем добавить все области разрешений, необходимые вашему приложению, к атрибуту или свойству при инициализации поставщика (это не относится к `scopes` [поставщику SharePoint).](../providers/sharepoint.md) Это необязательный вариант, но улучшит пользовательский интерфейс, презентуя пользователю единый экран согласия со сводным списком разрешений, запрашиваемого всеми компонентами в вашем приложении, вместо того чтобы представлять отдельные экраны для каждого компонента. В следующих примерах покажите, как это сделать с MsalProvider.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

Если вы инициализируете поставщика в коде, указать области разрешений в массиве `scopes` в свойстве.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

Список областей разрешений, необходимых каждому компоненту, можно найти в разделе **Разрешения Microsoft Graph** на странице документации каждого компонента.

## <a name="provider-state"></a>Состояние поставщика

Поставщик отслеживает состояние проверки подлинности пользователя и передает его компонентам. Например, когда пользователь успешно войдет, пользователь обновляется до , сигнализая компонентам, что они теперь могут делать вызовы `ProviderState` `SignedIn` в Microsoft Graph. Как показано, перечисление `ProviderState` определяет три состояния.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

В некоторых сценариях необходимо показать определенные функции или выполнить действие только после успешной записи пользователя. Вы можете получить доступ и проверить состояние поставщика, как показано в следующем примере.

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
Вы также можете использовать метод для получения уведомлений всякий раз, `Providers.onProviderUpdated` когда меняется состояние поставщика.

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

Каждый поставщик предоставляет функцию, которая может получить текущий маркер доступа или получить новый маркер доступа `getAccessToken` для предоставленных областей. В следующем примере показано, как получить новый маркер доступа с `User.Read` областью разрешений.

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = await Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>Создание собственных вызовов в Microsoft Graph

Все компоненты могут получать доступ к Microsoft Graph без каких-либо настроек, необходимых при инициализации поставщика (как описано в предыдущих разделах). Если вы хотите сделать собственные вызовы в Microsoft Graph, вы можете сделать это, получив ссылку на тот же SDK Microsoft Graph, используемый компонентами. Сначала получите ссылку на глобальный, а `IProvider` затем используйте `graph` объект, как показано:

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
Могут быть случаи, когда вам необходимо передать дополнительные разрешения в зависимости от API, который вы вызываете. В следующем примере показывается, как это можно сделать.

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a>Использование нескольких поставщиков

В некоторых сценариях приложение будет работать в разных средах и для каждого из них потребуется другой поставщик. Например, приложение может работать как веб-приложение, так и вкладка Microsoft Teams, что означает, что вам может потребоваться использовать как MsalProvider, так и TeamsProvider. Для этого сценария все компоненты поставщика имеют атрибут для создания цепочки откатов, как показано `depends-on` в следующем примере.

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

В этом сценарии msalProvider будет использоваться только в том случае, если ваше приложение работает в качестве веб-приложения, а TeamsProvider не доступен в текущей среде.

Чтобы выполнить то же самое в коде, можно использовать свойство `isAvailable` на поставщике, как показано.

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a>Вход пользователя/вход в систему

Если у вас есть правильные поставщики, инициализированные для вашего приложения, вы можете добавить компонент [login](../components/login.md) набор средств для легкой и быстрой реализации входа и входа пользователя. Компонент работает с поставщиком для обработки всей логики проверки подлинности и функций входа/входа. В следующем примере используются компонент MsalProvider и компонент Login.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

В сценариях, в которых вы хотите реализовать это самостоятельно, а не использовать компонент login набор средств, вы можете сделать это с помощью и методов `login` `logout` поставщика.

## <a name="implement-your-own-provider"></a>Реализация собственного поставщика

В сценариях, когда необходимо добавить набор средств в приложение с уже существующим кодом проверки подлинности, можно создать настраиваемого поставщика, который подключается к вашему механизму проверки подлинности, а не с помощью наших предопределяющих поставщиков. Набор инструментов предоставляет два способа создания новых поставщиков:

- Создайте новый маркер доступа из кода проверки подлинности, передав `SimpleProvider` функцию.
- Расширение `IProvider` абстрактного класса.

Дополнительные сведения о каждом из них см. в [пользовательских поставщиках.](../providers/custom.md)
