---
title: Microsoft Teams поставщика MSAL2
description: Используйте поставщик Teams MSAL2 в вкладке Microsoft Teams для облегчения проверки подлинности и доступа microsoft Graph ко всем компонентам. Поставщик может использоваться для одно-входного (SSO) или интерактивного входного знака.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: f4c05862b1a7ad0ffce33b6fa152d47e8e111a63
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588724"
---
# <a name="microsoft-teams-msal2-provider"></a>Microsoft Teams поставщика MSAL2

Используйте поставщика Microsoft Teams MSAL2 в вкладке Microsoft Teams для облегчения проверки подлинности и доступа microsoft Graph ко всем компонентам. Поставщик может использоваться для единого входного (SSO) или интерактивного входного знака.

Дополнительные дополнительные новости см. [в дополнительных данных.](./providers.md)

>**Совет:** Дополнительные сведения о создании приложения Microsoft Teams с поставщиком Teams MSAL2 см. в материале Сборка вкладки [Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md) и создание вкладки Microsoft Teams с [помощью SSO](../get-started/build-a-microsoft-teams-sso-tab.md).


### <a name="difference-between-teams-provider-and-teams-msal2-provider"></a>Разница между Teams и Teams msAL2 Provider
В отличие от Teams поставщика, поставщик Teams MSAL2 поддерживает один вход (SSO) и построен на [msal-браузере](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) для проверки подлинности на стороне клиента. [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) реализует код авторизации OAuth [2.0 Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow) PKCE. Поскольку код авторизации Flow считается более безопасным, чем неявный грант Flow для веб-приложений, мы рекомендуем использовать Teams поставщика MSAL2 через Teams поставщика. Сведения о проблемах безопасности, связанных с неявным потоком грантов, см. в материале [Недостатки неявного потока](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).

Все новые приложения должны по возможности использовать Teams поставщика MSAL2. 

## <a name="get-started"></a>Начало работы

Поставщик может использоваться в интерактивном режиме стороне клиента или режиме SSO. 

### <a name="client-side-authentication"></a>Проверка подлинности на стороне клиента
В клиентской проверке подлинности (или интерактивной проверке подлинности) пользователю будет предложено проверить подлинность при первом запуске приложения. Чтобы инициировать поток проверки подлинности, пользователю потребуется использовать кнопку вход в кнопку. Это можно сделать на клиенте и не требует службы backend. 

### <a name="sso-authentication"></a>Проверка подлинности SSO
Чтобы не запрашивать у пользователя проверку подлинности в приложении, Microsoft Teams вкладки также могут использовать [SSO](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) для автоматической проверки подлинности пользователей. Однако для этого процесса требуется резервная служба, которая используется для обмена Microsoft Teams с маркером доступа, который можно использовать для доступа к Microsoft Graph.

Teams MSAL2 поддерживает режим SSO, который включен при `ssoUrl` \ `sso-url` настроены на службу backend, способную обмениваться маркерами. Резервная служба обязана выставить API (`api/token`например), который получит маркер проверки подлинности из Microsoft Teams `on-behalf-of` и использовать поток для обмена маркера на маркер доступа, который может получить доступ к Microsoft Graph. Для эталонной реализации службы backend узла см. пример [Microsoft Teams узла SSO](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).

### <a name="initialize-the-provider"></a>Инициализация поставщика
Перед использованием поставщика Teams MSAL2 убедитесь, что на странице [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk).

Инициализация поставщика Teams MSAL2 в основном коде.

# <a name="npm"></a>[npm](#tab/ts)
При инициализации Teams msAL2 в JavaScript установите как набор инструментов, так и Microsoft Teams SDK.

```cmd
npm install @microsoft/teams-js @microsoft/mgt-element @microsoft/mgt-teams-msal2-provider
```

Затем импортируйте и используйте поставщика.

```ts
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider(config);
```

где `config`:

```ts
export interface TeamsMsal2Config {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
  ssoUrl?: string; // ex: '/api/token',
  autoConsent?: boolean,
  httpMethod: HttpMethod; //ex HttpMethod.POST
}
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="user.read,people.read..." 
  authority=""
  sso-url="/api/token" 
  http-method="POST">
></mgt-teams-msal2-provider>
```

| Атрибут | Описание |
| --- | --- |
| client-id   | Строковый идентификатор клиента (см. раздел [Настройка приложения Teams](#configure-your-teams-app)). Обязательный. |
| auth-popup-url  | Абсолютный или относительный путь к странице, обрабатывающей проверку подлинности во всплывающем окне (см. раздел [Создание всплывающей страницы](#create-the-popup-page)). Обязательный. |
| scopes  | Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе. Необязательный. |
| authority    | Строка центра. По умолчанию используется общий центр. Для однотенантного приложения используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`. Необязательный. |
| sso-url  | Абсолютный или относительный путь к API-резерву, который обрабатывает обмен маркерами OBO. Необязательно. |
| http-method  | Тип метода HTTP, который используется для вызова API backend. `POST` или `GET`. Значение по умолчанию: `GET`. Необязательный |

---
### <a name="create-the-popup-page"></a>Создание всплывающей страницы

Чтобы войти в Teams учетных данных и обрабатывать согласие, необходимо предоставить URL-адрес, который приложение Teams откроется в всплывающее приложение, которое будет следовать потоку проверки подлинности. Создайте новую страницу в приложении (например, https://mydomain.com/auth) которая будет обрабатывать перенаправление auth и вызывать `TeamsMsal2Provider.handleAuth` метод. Это единственное действие, которое должно выполняться этой страницей. Например:

# <a name="npm"></a>[npm](#tab/ts)

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;
TeamsMsal2Provider.handleAuth();
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsMsal2Provider.handleAuth();
</script>
```
---

## <a name="configure-your-teams-app"></a>Настройка приложения Teams

Если вы только приступаете к работе с приложениями Teams, см. раздел [Добавление вкладок в приложения Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview). Вы также можете использовать [App Studio для](/microsoftteams/platform/get-started/get-started-app-studio) разработки манифеста приложения.

### <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения

Дополнительные сведения о том, как зарегистрировать приложение и получить идентификацию клиента для интерактивной проверки подлинности, см. в Azure Active Directory [приложения](../get-started/add-aad-app-registration.md).


Дополнительные сведения о том, как зарегистрировать приложение и получить ID клиента и секрет для SSO, см. в Microsoft Teams вкладке Build a Microsoft Teams с [одним входом](../get-started/build-a-microsoft-teams-sso-tab.md).

## <a name="migrating-from-teams-provider-to-teams-msal2-provider"></a>Перенос из Teams поставщика в Teams msAL2 Provider
Чтобы перенести приложение, использующее Teams поставщика, к поставщику Teams MSAL2:
1. Перейдите на портал Azure по адресу https://portal.azure.com.
1. В меню выберите **Azure Active Directory**.
1. В меню Azure Active Directory выберите **Регистрация приложений**.
1. Выберите регистрацию приложения, используемого в настоящее время. 
1. В левом меню перейдите к **проверке подлинности**.
1. В **конфигурациях платформы** выберите **Добавить платформу** и выберите **одно-страницное приложение**.
1. Удалите все URL-адреса перенаправления, зарегистрированные в **Интернете**, и добавьте их в **одностражном приложении**.
1. В коде замените TeamsProvider на Teams msAL2 Provider.

    Если вы инициализируете поставщика в коде JS/TS, выполните следующие действия:
    
    Замените заявление на импорт ```mgt-teams-provider``` 
    ```ts 
    import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
    ```
    Замените инициализацию MsalProvider
    ```ts
    Providers.globalProvider = new TeamsMsal2Provider(config);
    ```
    Если вы инициализируете поставщика в HTML, замените 
    ```html
    <mgt-teams-provider client-id="<YOUR_CLIENT_ID>" auth-popup-url="/AUTH-PATH" ... ></mgt-teams-provider>
    ``` 
     с  
    ```html
    <mgt-teams-msal2-provider client-id="<YOUR_CLIENT_ID>" auth-popup-url="/AUTH-PATH" ... ></mgt-teams-msal2-provider>
    ```

## <a name="see-also"></a>См. также
* [Microsoft Teams пример SSO узла](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [Создание вкладки Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md)
* [Создание вкладки Microsoft Teams с помощью SSO](../get-started/build-a-microsoft-teams-sso-tab.md)
