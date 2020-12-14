---
title: Поставщики набор средств Microsoft Graph
description: Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: a4cd1b58bb29e42ecb0283709e71a3ce3a7e86d7
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658261"
---
# <a name="microsoft-graph-toolkit-providers"></a>Поставщики набор средств Microsoft Graph

Поставщики набор средств Microsoft Graph позволяют приложению проверить подлинность с помощью microsoft Identity и получить доступ к Microsoft Graph всего за несколько строк кода. Каждый поставщик обрабатывает проверку подлинности пользователей и получает маркеры доступа для вызова API Microsoft Graph, чтобы вам не нужно было писать этот код самостоятельно. 

Вы можете использовать поставщики самостоятельно без компонентов, чтобы быстро реализовать проверку подлинности для вашего приложения и выполнить вызовы Microsoft Graph через клиентский SDK JavaScript.

Поставщики необходимы при использовании microsoft Graph набор средств компонентов, которые используют их для доступа к Microsoft Graph. Если у вас уже есть собственная проверка подлинности и вы хотите использовать компоненты, можно использовать [настраиваемую службу.](./custom.md)

В набор средств входят следующие поставщики.

|Поставщики|Описание|
|---------|-----------|
|[Msal](./msal.md)|Использует MSAL.js для входов пользователей и получения маркеров для использования с Microsoft Graph в веб-приложении.|
|[SharePoint](./sharepoint.md)|Проверка подлинности и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.|
|[Teams](./teams.md)|Проверка подлинности и предоставляет Microsoft Graph доступ к компонентам на вкладке Microsoft Teams.|
|[Прокси-сервер](./proxy.md)|Позволяет использовать проверку подлинности на тыловом компьютере путем маршрутизации всех вызовов в Microsoft Graph через ваш тыл.|
|[Custom](./custom.md)|Создайте настраиваемого поставщика, чтобы включить проверку подлинности и доступ к Microsoft Graph с помощью существующего кода проверки подлинности приложения.|

## <a name="initializing-a-provider"></a>Инициализация поставщика

Чтобы использовать поставщика в приложении, необходимо инициализировать нового поставщика, а затем установить его в качестве глобального поставщика в пространстве имен поставщиков. Рекомендуем сделать это перед началом использования какого-либо из компонентов. Это можно сделать одним из двух способов:

**Вариант 1. Использование компонента поставщика**

Версию компонента поставщика можно использовать непосредственно в HTML-коде. За кадром новый поставщик инициализируются и устанавливается в качестве глобального поставщика. В следующем примере показано, как использовать MsalProvider.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

**Вариант 2. Инициализация в коде**

Инициализация поставщика в коде JavaScript позволяет предоставить дополнительные параметры. Для этого создайте новый экземпляр поставщика и установите значение свойства для поставщика, который вы `Providers.globalProvider` хотите использовать. В следующем примере показано, как использовать MsalProvider.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **Примечание.** Дополнительные сведения о том, как зарегистрировать приложение и получить ИД клиента, см. в примере создания приложения [Azure Active Directory.](../get-started/add-aad-app-registration.md)

## <a name="permission-scopes"></a>Области разрешений

Мы рекомендуем добавить все области разрешений, необходимые приложению, к атрибуту или свойству при инициализации поставщика (это не относится к поставщику `scopes` [SharePoint).](../providers/sharepoint.md) Это необязательный вариант, но позволит улучшить пользовательский интерфейс, выведя пользователю единый экран согласия со сводным списком разрешений, запрашиваемого всеми компонентами приложения, вместо того чтобы представлять отдельные экраны для каждого компонента. В следующих примерах покажите, как это сделать с помощью MsalProvider.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

Если вы инициализируете поставщика в коде, в свойстве предозначим области разрешений в `scopes` массиве.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

Список областей разрешений, необходимых каждому компоненту, можно найти в разделе разрешений **Microsoft Graph** на странице документации каждого компонента.

## <a name="provider-state"></a>Состояние поставщика

Поставщик отслеживает состояние проверки подлинности пользователя и передает его компонентам. Например, когда пользователь успешно войдет, он обновляется до , сообщает компонентам, что теперь он может звонить `ProviderState` `SignedIn` в Microsoft Graph. В `ProviderState` этом коде определяются три состояния, как показано ниже.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

В некоторых сценариях необходимо показать определенные функции или выполнить действие только после успешного выполнения пользователем. Вы можете получить доступ к поставщику и проверить его состояние, как показано в следующем примере.

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
Этот метод также можно использовать для получения уведомлений при изменениях состояния `Providers.onProviderUpdated` поставщика.

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
  const token = Provider.globalProvider.getAccessToken({scopes: 'User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>Самостоятельное вызовы Microsoft Graph

Все компоненты могут получить доступ к Microsoft Graph без какой-либо настройки, необходимой при инициализации поставщика (как описано в предыдущих разделах). Если вы хотите самостоятельно звонить в Microsoft Graph, вы можете получить ссылку на тот же SDK Microsoft Graph, который используется компонентами. Сначала получите ссылку на глобальный объект, а `IProvider` затем `graph` используйте объект, как показано ниже.

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
В некоторых случаях может потребоваться передать дополнительные разрешения в зависимости от вызываемой API. В следующем примере показывается, как это можно сделать.

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a>Использование нескольких поставщиков

В некоторых сценариях приложение будет работать в разных средах и для каждого из них потребуется другой поставщик. Например, приложение может работать как веб-приложение и как вкладка Microsoft Teams, что означает, что вам может потребоваться использовать msalProvider и TeamsProvider. В этом сценарии все компоненты поставщика имеют атрибут для создания цепочки отката, как показано `depends-on` в следующем примере.

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

В этом сценарии MsalProvider будет использоваться, только если ваше приложение работает как веб-приложение и TeamsProvider не доступен в текущей среде.

Чтобы выполнить то же самое в коде, можно использовать свойство `isAvailable` поставщика, как показано ниже.

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a>Вход и вход пользователя

При инициализации нужных поставщиков для приложения можно добавить [](../components/login.md) компонент входа набор средств, чтобы легко и быстро реализовать вход и вход пользователя. Компонент работает с поставщиком для обработки всей логики проверки подлинности и функций входа и входа в систему. В следующем примере используются MsalProvider и компонент Login.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

В сценариях, где вы хотите реализовать это самостоятельно, а не использовать компонент входа набор средств входа в систему, это можно сделать с помощью и методов `login` `logout` поставщика.

## <a name="implement-your-own-provider"></a>Реализация собственного поставщика

В сценариях, где вы хотите добавить набор средств в приложение с уже существующим кодом проверки подлинности, можно создать настраиваемого поставщика, который подключается к вашему механизму проверки подлинности вместо использования наших предопределенных поставщиков. Набор средств предоставляет два способа создания новых поставщиков:

- Создайте новый маркер доступа из кода проверки подлинности, передав `SimpleProvider` функцию.
- Расширение `IProvider` абстрактного класса.

Дополнительные сведения о каждом из них см. [в настраиваемом поставщике.](../providers/custom.md)
