---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 62dba210d4fbf7d3540df7fd58d33e275f0065c3
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990257"
---
# <a name="microsoft-teams-provider"></a>Поставщик Microsoft Teams

Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.

Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).

## <a name="get-started"></a>Начало работы

Перед использованием поставщика Teams необходимо убедиться, что на странице есть ссылка на [пакет SDK Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) .

### <a name="via-script-tag"></a>тег сценария Via
В следующем примере используется поставщик в HTML (через CDN).

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
  authority=""
></mgt-teams-provider>
```

| Атрибут | Описание |
| --- | --- |
| Client — ID   | Строковый идентификатор клиента (см. раздел [Настройка приложения Teams](#configure-your-teams-app)). Обязательный. |
| auth-контекстное-URL  | Абсолютный или относительный путь к странице, которая будет обрабатывать проверку подлинности в всплывающем окне (см. раздел [Создание всплывающей страницы](#create-the-popup-page)). Обязательный. |
| scopes  | Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему. Необязательный параметр. |
| зависит от | Строка выбора элемента другого компонента поставщика с более высоким приоритетом. Необязательный параметр. |
| авторитет    | Строка Authority. По умолчанию используется общий центр. Для приложений с одним клиентом используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` . Необязательный параметр. |


### <a name="via-npm"></a>с помощью NPM
В следующем примере используется поставщик в JS-модулях (через NPM).

Обязательно установите набор средств и пакет SDK Microsoft Teams.

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

После этого импортируйте и используйте поставщика.

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt';
Providers.globalProvider = new TeamsProvider(config);
```

где `config` находится

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

Кроме того, может потребоваться задать ссылку на библиотеку Microsoft Teams. Вот пример:

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

Полный пример приведен в [статье пример вкладки Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).

## <a name="configure-your-teams-app"></a>Настройка приложения Teams

Если вы только начинаете работать с приложениями Teams, ознакомьтесь с разделом [Добавление вкладок в приложения Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview). Кроме того, с помощью [app Studio](/microsoftteams/platform/get-started/get-started-app-studio) можно быстро разработать манифест приложения.

После установки приложения на вкладке и готовности к использованию компонентов необходимо убедиться, что у вашего приложения есть необходимые разрешения для доступа к Microsoft Graph. Чтобы настроить приложение с необходимыми разрешениями:

1. [Получение имени домена](/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [Создание регистрации нового приложения](/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [Предоставление разрешения на доступ к приложению](/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

Важно добавить правое разрешение на **странице Добавление доступа к API**. Для добавления и утверждения разрешений необходимо быть администратором в зависимости от того, какой компонент вам необходим.

>**Совет:** Если вы не знаете, какие разрешения следует добавить, ознакомьтесь с документацией по каждому компоненту.

### <a name="enable-implicit-grant-flow"></a>Разрешить неявный поток предоставления

Не забудьте включить неявный поток предоставления; Это требование для веб-приложений, запрашивающих маркеры от клиентской стороны. На портале Azure при управлении регистрацией приложений измените манифест и измените `oauth2AllowImplicitFlow` его на `true` .

### <a name="create-the-popup-page"></a>Создание всплывающей страницы

Чтобы войти в систему с помощью учетных данных Teams, необходимо предоставить URL-адрес, который приложение Teams будет открывать во всплывающем окне, которое будет проходить процесс проверки подлинности. Этот URL-адрес должен находиться в вашем домене и должен вызывать `TeamsProvider.handleAuth();` метод. Это единственный элемент, который требуется для выполнения этой страницы. Например:

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

или через модуль, указанный в всплывающем окне проверки подлинности:

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a>Настройка URI перенаправления

После публикации этой страницы на веб-сайте необходимо использовать URL-адрес в `auth-popup-url/authPopupUrl` свойстве. Этот URL-адрес также необходимо настроить в качестве действительного URI перенаправления в конфигурации приложения на портале Azure AD.
