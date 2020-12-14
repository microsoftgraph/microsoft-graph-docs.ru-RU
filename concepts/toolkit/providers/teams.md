---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams на вкладке Microsoft Teams, чтобы упростить проверку подлинности и доступ Microsoft Graph ко всем компонентам.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 463fa4afdfd4e0dd3e3cb09ad155f0cae08fb347
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664039"
---
# <a name="microsoft-teams-provider"></a>Поставщик Microsoft Teams

Используйте поставщика Teams на вкладке Microsoft Teams, чтобы упростить проверку подлинности и доступ Microsoft Graph ко всем компонентам.

Дополнительные информацию о поставщиках проверки подлинности см. [в этой теме.](./providers.md)

>**Совет:** Дополнительные сведения о том, как начать работу с созданием приложения Microsoft Teams с помощью поставщика Teams, см. в руководстве по началу работы с вкладками ["Создание вКладки Microsoft Teams".](../get-started/build-a-microsoft-teams-tab.md)

## <a name="get-started"></a>Начало работы

Перед использованием поставщика Teams необходимо убедиться, что вы ссылались на [microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) на своей странице.

# <a name="npm"></a>[npm](#tab/ts)

Обязательно установите набор средств и microsoft Teams SDK.

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

Затем импортировать и использовать поставщика.

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

где `config` находится

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

### <a name="mgt-teams-provider-attributes"></a>атрибуты mgt-teams-provider
| Атрибут | Описание |
| --- | --- |
| client-id   | Строка ИД клиента (см. ["Настройка приложения Teams").](#configure-your-teams-app) Обязательный. |
| auth-popup-url  | Абсолютный или относительный путь к странице, которая будет обрабатывать auth во всплывающее окна (см. страницу создания [всплывающее).](#create-the-popup-page) Обязательный. |
| scopes  | Разделенные запятой строки для областей, на которые пользователь должен согласиться при входе. Необязательно. |
| зависит от | Строка селектора элементов другого компонента поставщика с более высоким приоритетом. Необязательно. |
| authority    | Строка authority. По умолчанию используется общий орган. Для приложений с одним клиентом используйте свой ИД клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` . Необязательно. |

---

### <a name="create-the-popup-page"></a>Создание всплываемой страницы

Чтобы войти с помощью своих учетных данных Teams, необходимо указать URL-адрес, который приложение Teams откроет во всплывающее приложение, которое будет следовать потоку проверки подлинности. Этот URL-адрес должен быть в вашем домене и вызывать `TeamsProvider.handleAuth();` метод. Это единственное, что необходимо сделать на этой странице. Примеры:

# <a name="npm"></a>[npm](#tab/ts)

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
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

### <a name="configure-redirect-uris"></a>Настройка URIS перенаправления

После публикации всплываемой страницы на веб-сайте необходимо использовать URL-адрес в `auth-popup-url/authPopupUrl` свойстве. Этот URL-адрес также необходимо настроить в качестве допустимого URI перенаправления в конфигурации приложения на портале Azure AD.

## <a name="configure-your-teams-app"></a>Настройка приложения Teams

Если вы только начинаете работу с приложениями Teams, см. вкладки "Добавление [вкладок в приложения Microsoft Teams".](/microsoftteams/platform/concepts/tabs/tabs-overview) Вы также можете использовать [App Studio для](/microsoftteams/platform/get-started/get-started-app-studio) быстрой разработки манифеста приложения.
### <a name="creating-an-appclient-id"></a>Создание приложения или ИД клиента
Чтобы получить ИД клиента, необходимо зарегистрировать приложение [в](../get-started/add-aad-app-registration.md) Azure AD. 
>**Примечание.** MSAL поддерживает только неявный поток для OAuth. Обязательно включите неявный поток в приложении на портале Azure (по умолчанию он не включен). В **разделе "Проверка подлинности"** найдите раздел неявного предоставления и выберите для маркеров **доступа** и **маркеров ID** свои почтовые ящики.  

## <a name="see-also"></a>См. также
* [Пример вкладки Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [Создание вкладки Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md)