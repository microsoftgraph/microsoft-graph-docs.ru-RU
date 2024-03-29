---
title: Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств
description: начало работы создание вкладки Microsoft Teams с помощью microsoft Graph набор средств.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 6b33fda93f3383fede93d79362762ea234e7a8be
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589018"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств

В этом разделе описывается, как начать использовать microsoft Graph набор средств в Microsoft Teams решении. Это руководство для приложения на одной странице без единого входного приложения (SSO) и не требует дополнительного приложения. Если вы реализуете SSO с настраиваемой задней Microsoft Teams([SSO)](./build-a-microsoft-teams-sso-tab.md).

Создание вкладки включает в себя следующие действия:

1. Добавьте microsoft Graph набор средств.
1. Создание всплываемой страницы auth.
1. Создание идентификатора клиента/приложения
1. Инициализация поставщика Teams MSAL2.
1. Добавление компонентов.
1. Проверьте приложение.

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление Microsoft Graph Toolkit

Вы можете использовать microsoft Graph набор средств в приложении, ссылаясь на погрузчик напрямую (с помощью unpkg) или установив пакеты npm. Чтобы использовать набор средств, вам также потребуется Microsoft Teams [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk).

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
Чтобы использовать набор средств и Teams SDK через загрузчики, добавьте ссылку в скрипт в код:

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

# <a name="npm"></a>[npm](#tab/npm)
Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения. Чтобы использовать модули ES6, добавьте пакеты npm для набор средств и Microsoft Teams SDK в проект:

```cmd
npm install @microsoft/teams-js @microsoft/mgt-element @microsoft/mgt-teams-msal2-provider @microsoft/mgt-components
```

---

## <a name="create-the-auth-popup-page"></a>Создание всплываемой страницы auth

Чтобы разрешить пользователям войти, вам потребуется страница в вашем приложении, Teams откроется в всплывающее приложение, чтобы следовать потоку проверки подлинности. Путь к странице может быть всем, пока он находится в том же домене, что и ваше приложение (например, https://yourdomain.com/tabauth). Единственное требование для этой страницы `TeamsMsal2Provider.handleAuth()` — вызвать метод, но вы можете добавить любой необходимый контент или ход загрузки.

Ниже приводится пример базовой страницы, которая обрабатывает поток auth в всплывающее всплывающее.

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsMsal2Provider.handleAuth();
    </script>
  </body>
</html>
```
# <a name="npm"></a>[npm](#tab/npm)
```js
import { TeamsMsal2Provider } from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.handleAuth();
```

---

## <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить клиентский ID, необходимо зарегистрировать Azure Active Directory приложение. Выполните действия в статье [Создание Azure Active Directory приложения](./add-aad-app-registration.md).

Убедитесь, что в `redirect URI` регистрации приложения необходимо указать на страницу auth, созданную на предыдущем шаге. Например, https://localhost:3000/tabauth.

> **Примечание:** Убедитесь, что в качестве `redirect URI` .`Single Page Application (SPA)` Teams msAL2 Provider использует поставщика MSAL2 за кулисами.

## <a name="initialize-the-teams-msal2-provider"></a>Инициализация поставщика Teams MSAL2

Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). Поставщик [Teams MSAL2](../providers/teams-msal2.md) обрабатывает все логики и взаимодействия, которые необходимо реализовать с Teams SDK для проверки подлинности пользователя.

Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript. 

# <a name="html"></a>[html](#tab/html)


Добавьте компонент `mgt-teams-msal2-provider` на страницу HTML, как показано.

```html
<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/tabauth"
  scopes="User.Read,Mail.ReadBasic"
  ></mgt-teams-msal2-provider>
```

Замените `<YOUR_CLIENT_ID>` с помощью клиентского ID для приложения и `auth-popup-url` замените полный или относительный путь на страницу auth. 

# <a name="js"></a>[js](#tab/js)


Чтобы инициализировать поставщика в коде JavaScript, добавьте в приложение следующий код:

```ts
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider({
  clientId: `<YOUR_CLIENT_ID>`,
  authPopupUrl: '/tabauth',
  scopes: ['User.Read','Mail.ReadBasic'],
});
```
Замените `<YOUR_CLIENT_ID>` с помощью клиентского ID для приложения и `authPopupUrl` замените полный или относительный путь на страницу auth.

---
## <a name="add-components"></a>Добавление компонентов

Теперь вы готовы добавить любой из компонентов Microsoft Graph набор средств. Первым компонентом, который, скорее всего, потребуется добавить, является компонент Login.

```HTML
<mgt-login></mgt-login>
```

Компонент Login передает кнопку "Вход", которая направляет пользователя по входу в процессе и интегрируется с любым из поставщиков для обработки проверки подлинности. После того, как пользователь включит, все остальные компоненты наборов инструментов смогут автоматически вызывать microsoft Graph. Поставщики также подвергают проверке подлинность клиента Microsoft Graph для звонков API или получения маркеров доступа. Подробные сведения см. [в материале Использование поставщиков](../providers/providers.md).

Если вы используете React, рекомендуется использовать React компоненты `mgt-react` вместо библиотеки. Дополнительные дополнительные ссылки см. в [Graph набор средств Microsoft React](./use-toolkit-with-react.md)

## <a name="next-steps"></a>Дальнейшие действия
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задайте вопрос [в Microsoft Q&A](/answers/topics/microsoft-graph-toolkit.html).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
- Ознакомьтесь с [Microsoft Teams примерами](https://github.com/OfficeDev/Microsoft-Teams-Samples/tree/main/samples/tab-graph-toolkit).
