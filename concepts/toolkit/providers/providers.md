---
title: Поставщики Graph набор средств Майкрософт
description: Поставщики Graph набор средств Майкрософт обеспечивают проверку подлинности, а microsoft Graph доступ ко всем компонентам.
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: ec7fd10e37e2382313ae611fee3912110216cfc3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126557"
---
# <a name="microsoft-graph-toolkit-providers"></a>Поставщики Graph набор средств Майкрософт

Поставщики Graph набор средств Майкрософт позволяют приложению проверить подлинность с помощью Microsoft Identity и получить доступ Graph только в нескольких строках кода. Каждый поставщик обрабатывает проверку подлинности пользователей и приобретает маркеры доступа для вызова API Microsoft Graph, чтобы вам не нужно было самостоятельно писать этот код. 

Вы можете использовать поставщики самостоятельно, без компонентов, чтобы быстро реализовать проверку подлинности для вашего приложения и сделать вызовы в Microsoft Graph через SDK клиента JavaScript.

Поставщики требуются при использовании компонентов Microsoft Graph набор средств, так как компоненты используют их для доступа к microsoft Graph. Если у вас уже есть собственная проверка подлинности и вы хотите использовать компоненты, вместо этого можно использовать [настраиваемый поставщик.](./custom.md)

В набор средств содержатся следующие поставщики.

|Поставщики|Описание|
|---------|-----------|
|[MSAL](./msal.md)|Использует msal.js для регистрации пользователей и приобретения маркеров для использования с microsoft Graph в веб-приложении.|
|[MSAL2](./msal2.md)| Использует msal-browser для регистрации пользователей и приобретения маркеров для использования с microsoft Graph в веб-приложении. | 
|[Электрон](./electron.md)|Проверка подлинности и Graph доступ к компонентам в приложениях Electron.|
|[SharePoint](./sharepoint.md)|Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.|
|[Teams](./teams.md)|Использует msal.js для регистрации пользователей и приобретения маркеров на клиенте в Microsoft Teams вкладок.|
|[Teams MSAL2](./teams-msal2.md)|Использует msal-browser для регистрации пользователей и приобретения маркеров в Microsoft Teams вкладками. Поддерживает единую Sign-On с настраиваемой поддержкой. |
|[Прокси-сервер](./proxy.md)|Позволяет использовать проверку подлинности на внутреннем сервере с помощью маршрутизации всех вызовов Microsoft Graph через внутренний сервер.|
|[Настраиваемый](./custom.md)|Создание настраиваемого поставщика для включения проверки подлинности и доступа к Microsoft Graph с помощью существующего кода проверки подлинности приложения.|

## <a name="initializing-a-provider"></a>Инициализация поставщика

Чтобы использовать поставщика в приложении, необходимо инициализировать нового поставщика, а затем установить его в качестве глобального поставщика в пространстве имен поставщиков. Мы рекомендуем сделать это, прежде чем приступить к использованию любого из компонентов. Это можно сделать одним из двух способов:

**Вариант 1. Использование компонента поставщика**

Компонентную версию поставщика можно использовать непосредственно в HTML. За кулисами новый поставщик инициализируются и устанавливается как глобальный поставщик. В следующем примере показано, как использовать поставщика MSAL2.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"></mgt-msal2-provider>
```

**Вариант 2. Инициализация кода**

Инициализация поставщика в коде JavaScript позволяет предоставить дополнительные параметры. Для этого создайте новый экземпляр поставщика и установите значение свойства поставщику, который вы `Providers.globalProvider` хотите использовать. В следующем примере показано, как использовать поставщика MSAL2.

```js
import {Providers, Msal2Provider } from "@microsoft/mgt";
Providers.globalProvider = new Msal2Provider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **Примечание:** Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в материале [Create an Azure Active Directory app.](../get-started/add-aad-app-registration.md)

## <a name="permission-scopes"></a>Области разрешений

Мы рекомендуем добавить все области разрешений, необходимые вашему приложению, к атрибуту или свойству при инициализации поставщика (это не относится к `scopes` [поставщику SharePoint).](../providers/sharepoint.md) Это необязательный вариант, но улучшит пользовательский интерфейс, презентуя пользователю единый экран согласия со сводным списком разрешений, запрашиваемого всеми компонентами в вашем приложении, вместо того чтобы представлять отдельные экраны для каждого компонента. В следующих примерах покажите, как это сделать с поставщиком MSAL2.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal2-provider>
```

Если вы инициализируете поставщика в коде, указать области разрешений в массиве `scopes` в свойстве.

```js
import {Providers, Msal2Provider } from "@microsoft/mgt";
Providers.globalProvider = new Msal2Provider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

Список областей разрешений, необходимых каждому компоненту, можно найти в разделе разрешений **microsoft Graph** на странице документации каждого компонента.

## <a name="provider-state"></a>Состояние поставщика

Поставщик отслеживает состояние проверки подлинности пользователя и передает его компонентам. Например, когда пользователь успешно войдет, пользователь обновляется до , сигнализая компонентам, что они теперь могут звонить в `ProviderState` `SignedIn` Microsoft Graph. Как показано, перечисление `ProviderState` определяет три состояния.

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

## <a name="making-your-own-calls-to-microsoft-graph"></a>Создание собственных звонков в Корпорацию Майкрософт Graph

Все компоненты могут получать доступ к microsoft Graph без каких-либо настроек, необходимых до тех пор, пока вы инициализируете поставщика (как описано в предыдущих разделах). Если вы хотите сделать собственные вызовы в Microsoft Graph, вы можете сделать это, получив ссылку на тот же microsoft Graph SDK, используемый компонентами. Сначала получите ссылку на глобальный, а `IProvider` затем используйте `graph` объект, как показано:

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

В некоторых сценариях приложение будет работать в разных средах и для каждого из них потребуется другой поставщик. Например, приложение может работать в качестве веб-приложения и вкладки Microsoft Teams, что означает, что вам может потребоваться использовать как поставщика MSAL2, так и поставщика Teams MSAL2. Для этого сценария все компоненты поставщика имеют атрибут для создания цепочки откатов, как показано `depends-on` в следующем примере.

```html
<mgt-teams-msal2-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-msal2-provider>

<mgt-msal2-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal2-provider>
```

В этом сценарии поставщик MSAL2 будет использоваться только в том случае, если ваше приложение работает в качестве веб-приложения, а поставщик msAL2 Teams msAL2 в текущей среде.

Чтобы выполнить то же самое в коде, можно использовать свойство `isAvailable` на поставщике, как показано.

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new Msal2Provider(msalConfig)
}
```
## <a name="user-loginlogout"></a>Вход пользователя/вход в систему

Если у вас есть правильные поставщики, инициализированные для вашего приложения, вы можете добавить компонент [login](../components/login.md) набор средств для легкой и быстрой реализации входа и входа пользователя. Компонент работает с поставщиком для обработки всей логики проверки подлинности и функций входа/входа. В следующем примере используется поставщик MSAL2 и компонент Login.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

В сценариях, в которых вы хотите реализовать это самостоятельно, а не использовать компонент login набор средств, вы можете сделать это с помощью и методов `login` `logout` поставщика.

## <a name="implement-your-own-provider"></a>Реализация собственного поставщика

В сценариях, когда необходимо добавить набор средств в приложение с уже существующим кодом проверки подлинности, можно создать настраиваемого поставщика, который подключается к вашему механизму проверки подлинности, а не с помощью наших предопределяющих поставщиков. Набор инструментов предоставляет два способа создания новых поставщиков:

- Создайте новый маркер доступа из кода проверки подлинности, передав `SimpleProvider` функцию.
- Расширение `IProvider` абстрактного класса.

Дополнительные сведения о каждом из них см. в [пользовательских поставщиках.](../providers/custom.md)
