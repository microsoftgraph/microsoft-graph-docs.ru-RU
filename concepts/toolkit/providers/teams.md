---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams в своей вкладке Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: b83034005a11a7ba1795b3a4e9367b4bb3e94222
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588045"
---
# <a name="microsoft-teams-provider"></a>Поставщик Microsoft Teams

Используйте teamsProvider в вкладке Microsoft Teams для облегчения проверки подлинности и доступа microsoft Graph ко всем компонентам.

Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).

>**Совет**. Сведения о том, как приступить к созданию приложения Microsoft Teams с помощью поставщика Teams, см. в руководстве по началу работы [Создание вкладки Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md).

### <a name="difference-between-teams-provider-and-teams-msal2-provider"></a>Разница между Teams и Teams msAL2 Provider
В отличие от TeamsProvider, Teams msAL2 Provider поддерживает Sign-On (SSO) и построена на вершине [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) для проверки подлинности на стороне клиента. [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) реализует код авторизации OAuth [2.0 Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow) PKCE. Код авторизации Flow считается более безопасным, чем неявный грант Flow для веб-приложений, поэтому мы рекомендуем использовать Teams поставщика MSAL2 через Teams поставщика. Сведения о проблемах безопасности, связанных с неявным потоком грантов, см. в материале [Недостатки неявного потока](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).

Все новые приложения должны использовать поставщик Teams MSAL2 по возможности. См[. Teams msAL2 Provider для](./teams-msal2.md) документации по миграции.

## <a name="get-started"></a>Начало работы

Перед использованием поставщика Teams вам потребуется указать [SDK Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) на своей странице.

# <a name="npm"></a>[npm](#tab/ts)

Установите набор средств и пакет SDK Microsoft Teams.

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

Затем импортируйте и используйте поставщика.

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

где `config`:

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
}
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="User.Read,People.Read..."
  authority=""
></mgt-teams-provider>
```

### <a name="mgt-teams-provider-attributes"></a>Атрибуты mgt-teams-provider
| Атрибут | Описание |
| --- | --- |
| client-id   | Строковый идентификатор клиента (см. раздел [Настройка приложения Teams](#configure-your-teams-app)). Обязательный. |
| auth-popup-url  | Абсолютный или относительный путь к странице, обрабатывающей проверку подлинности во всплывающем окне (см. раздел [Создание всплывающей страницы](#create-the-popup-page)). Обязательный. |
| scopes  | Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе. Необязательный. |
| depends-on | Строка выбора элементов другого компонента поставщика с более высоким приоритетом. Необязательный. |
| authority    | Строка центра. По умолчанию используется общий центр. Для однотенантного приложения используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`. Необязательный. |

---

### <a name="create-the-popup-page"></a>Создание всплывающей страницы

Чтобы войти с использованием своих учетных данных Teams, вам потребуется указать URL-адрес, который будет открываться приложением Teams во всплывающем окне с выполнением потока проверки подлинности. Этот URL-адрес должен находиться в вашем домене и должен вызывать метод `TeamsProvider.handleAuth();`. Это единственное действие, которое должно выполняться этой страницей. Например:

# <a name="npm"></a>[npm](#tab/ts)

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
TeamsProvider.handleAuth();
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```
---

### <a name="configure-redirect-uris"></a>Настройка URI перенаправления

После публикации всплывающей страницы на своем веб-сайте вам требуется использовать URL-адрес в свойстве `auth-popup-url/authPopupUrl`. Этот URL-адрес также нужно настроить в качестве допустимого URI перенаправления в конфигурации приложения на портале Azure AD.

## <a name="configure-your-teams-app"></a>Настройка приложения Teams

Если вы только приступаете к работе с приложениями Teams, см. раздел [Добавление вкладок в приложения Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview). Для быстрой разработки манифеста приложения также можно использовать [App Studio](/microsoftteams/platform/get-started/get-started-app-studio).
### <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](../get-started/add-aad-app-registration.md) в Azure AD. 
>**Примечание**. MSAL поддерживает только неявный поток для OAuth. Включите неявный поток в своем приложении на портале Azure (он не включен по умолчанию). В области **Проверка подлинности** найдите раздел **Неявное предоставление** и установите флажки **Маркеры доступа** и **Маркеры идентификаторов**. 

## <a name="see-also"></a>См. также
* [Пример вкладки Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [Создание вкладки Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md)
