---
title: Создайте вкладку Microsoft Teams SSO с помощью microsoft Graph набор средств
description: начало работы создание вкладки Microsoft Teams SSO с помощью microsoft Graph набор средств.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 43a7a7b4b1fee3f33b027f170eb66cd04e49157d
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588815"
---
# <a name="build-a-microsoft-teams-sso-tab-with-the-microsoft-graph-toolkit"></a>Создайте вкладку Microsoft Teams SSO с помощью microsoft Graph набор средств

В этом разделе описывается использование microsoft Graph набор средств в Microsoft Teams решении. Это руководство для одно-страницного приложения с одним входом (SSO) и требует дополнительного приложения. Если вы реализуете вкладку Teams с интерактивным входом, см. в Microsoft Teams [Tab](./build-a-microsoft-teams-tab.md).

Создание вкладки SSO включает в себя следующие действия: 

1. Добавьте microsoft Graph набор средств.
1. Создание всплываемой страницы auth.
1. Создание идентификатора клиента/приложения
6. Создание backend
7. Инициализация Teams MSAL2.
8. Добавление компонентов.
9. Проверьте приложение.

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление Microsoft Graph Toolkit

Вы можете использовать microsoft Graph набор средств в приложении, ссылаясь на погрузчик напрямую (с помощью unpkg) или установив пакеты npm. Чтобы использовать набор средств, вам также потребуется Microsoft Teams [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk).

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
Чтобы использовать набор средств и Teams SDK через загрузчики, добавьте ссылку в скрипт в код:

```HTML
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

Если администратор не согласится на предварительное согласие вашего приложения, пользователям может потребоваться согласие на разрешения. Чтобы включить это, необходимо предоставить страницу, Teams приложение откроется в всплывающее приложение, чтобы следовать потоку проверки подлинности. Путь к странице может иметь все, что угодно, если она находится в том же домене, что и ваше приложение (например, https://yourdomain.com/tabauth). Единственное требование для этой страницы `TeamsMsal2Provider.handleAuth()` — вызвать метод, но вы можете добавить любой необходимый контент или ход загрузки.


Ниже приводится пример базовой страницы, которая обрабатывает поток auth в всплывающее всплывающее.

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
```HTML
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
```JavaScript
import { TeamsMsal2Provider } from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.handleAuth();
```

---

## <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить маркер доступа в Azure AD, вкладка должна работать в качестве зарегистрированного приложения Azure AD. Зарегистрируйте приложение в клиенте и Microsoft Teams получить маркеры доступа от его имени:

1. Откройте браузер и перейдите [в центр Azure Active Directory администрирования](https://aad.portal.azure.com). Во входе с помощью **личной учетной записи** (Учетная запись Майкрософт) **или Учетной записи Work или School**.

1. На левой области **выберите Azure Active Directory,** а **затем выберите Регистрация приложений** в **статье Управление**.

1. Выберите **Новая регистрация**. На странице **Регистрация приложения** задайте необходимые значения следующим образом:

    - Установите **имя** `Node.js Teams SSO` (или имя по вашему выбору).
    - В поле **Поддерживаемые типы учетных записей** выберите **Учетные записи в любом каталоге организаций и личные учетные записи Майкрософт**.
    - В **статье Перенаправление URI**`Single Page Application` установите первое падение и установите значение URL-адреса страницы auth, созданного на предыдущем шаге; например . `https://myapp.ngrok.io/tabauth` 

1. На странице обзор приложения скопируйте значение **ID приложения (клиента)** для более поздней части. Это значение потребуется при создании нового поставщика и в его задней части.

1. В **статье Управление** перейдите к **сертификатам & секретов**. Нажмите кнопку **Новый секрет клиента**. Введите значение в поле **Описание**, выберите один из параметров **Срок действия** и нажмите **Добавить**.

1. Прежде чем покинуть страницу, скопируйте значение секрета клиента. Это необходимо для службы backend.

    >[!IMPORTANT]
    >Система никогда не покажет секрет клиента повторно, поэтому убедитесь, что вы скопировали его.

1. В **статье Управление** перейдите **к разрешениям API**. Выберите **Добавить** **разрешенияMicrosoft** >  Graph  > **Delegated разрешений**, а затем добавить следующие разрешения: `email`, `offline_access`, `openid`, , `profile`. `User.Read` Выберите **Добавить разрешения**.

1. (НЕОБЯЗАТЕЛЬНЫЙ) Если требуется предварительное согласие на любые другие области, можно добавить дополнительные разрешения. Если вы используете различные компоненты или планируете использовать другие API Graph Microsoft, вам могут потребоваться дополнительные разрешения. Дополнительные сведения о необходимых разрешениях см. в [документации по](../overview.md) каждому компоненту.

    - Для предварительного согласия в качестве администратора выберите **согласие администратора Гранта**, а затем выберите **Да**.

1.  В **статье Управление** перейдите к **статье Expose aPI**. В верхней части страницы рядом с выберите `Application ID URI`**Набор**. Это создает API в виде: `api://{AppID}`. Обновите его, чтобы добавить поддомен; например, `api://myapp.ngrok.io/{appID}`.

1. На этой же странице выберите **Добавить область**. Заполните поля следующим образом и выберите **область Добавить**:

    - Имя области: `access_as_user`
    - Кто может согласиться?: **Администраторы и пользователи**
    - Имя отображения согласия администратора: `Teams can access the user’s profile`
    - Описание согласия администратора: `Allows Teams to call the app’s web APIs as the current user`
    - Имя отображения согласия пользователя: `Teams can access the user profile and make requests on the user's behalf`
    - Описание согласия пользователя: `Enable Teams to call this app’s APIs with the same rights as the user.`
    - Состояние: **Включено**
    
    URL-адрес API должен выглядеть так: `api://myapp.ngrok.io/{appID}/access_as_user`. 

1. Далее добавьте два клиентских приложения. Это для Teams/мобильных клиентов и веб-клиента. В разделе **Авторизованные клиентские приложения** выберите **Добавить клиентскую заявку**. Заполните ИД клиента и выберите область, созданную вами. Затем выберите **приложение Добавить**. Сделайте это для следующих IDs:
    
    - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346
    - 1fec8e78-bce4-4aaf-ab1b-5451cc387264

## <a name="create-the-backend"></a>Создание backend

Backend может быть любой задней частью, которая позволяет обмениваться маркером Microsoft Teams проверки подлинности с маркером, который можно использовать для вызова Microsoft Graph через поток от [имени.](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) 

Для справки см. [Teams SSO Node Sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/teams-sso-node).

Ниже приводится эталонная реализация экспресс-сервера узла:

```TypeScript
import dotenv from 'dotenv';
import express from 'express';
import path from 'path';
import * as msal from '@azure/msal-node';
import { NextFunction, Request, Response } from 'express';
import jwt, { JwtHeader, SigningKeyCallback } from 'jsonwebtoken';
import jwksClient from 'jwks-rsa';
import jwt_decode from 'jwt-decode';

// Load .env file
dotenv.config();

/**
 * Validates a JWT
 * @param {Request} req - The incoming request
 * @param {Response} res - The outgoing response
 * @returns {Promise<string | null>} - Returns the token if valid, returns null if invalid
 */
function validateJwt(req: Request, res: Response, next: NextFunction): void {
  const authHeader = req.headers.authorization!;
  const ssoToken = authHeader.split(' ')[1];
  if (ssoToken) {
    const validationOptions = {
      audience: process.env.CLIENT_ID,
    };
    jwt.verify(ssoToken, getSigningKey, validationOptions, (err, payload) => {
      if (err) {
        return res.sendStatus(403);
      }
      next();
    });
  } else {
    res.sendStatus(401);
  }
}

/**
 * Parses the JWT header and retrieves the appropriate public key
 * @param {JwtHeader} header - The JWT header
 * @param {SigningKeyCallback} callback - Callback function
 */
function getSigningKey(header: JwtHeader, callback: SigningKeyCallback): void {
  const client = jwksClient({
    jwksUri: 'https://login.microsoftonline.com/common/discovery/keys'
  });
  client.getSigningKey(header.kid!, (err, key) => {
    if (err) {
      callback(err, undefined);
    } else {
      callback(null, key.getPublicKey());
    }
  });
}

/**
 * Gets an access token for the user using the on-behalf-of flow
 * @param authHeader - The Authorization header value containing a JWT bearer token
 * @returns {Promise<string | null>} - Returns the access token if successful, null if not
 */
async function getAccessTokenOnBehalfOf(req: Request, res: Response): Promise<void> {
  // The token has already been validated, just grab it
  const authHeader = req.headers.authorization!;
  const ssoToken = authHeader.split(' ')[1];

  // Create an MSAL client
  const msalClient = new msal.ConfidentialClientApplication({
    auth: {
      clientId: req.body.clientid,
      clientSecret: process.env.APP_SECRET
    }
  });

  try {
    const result = await msalClient.acquireTokenOnBehalfOf({
      authority: `https://login.microsoftonline.com/${jwt_decode<any>(ssoToken).tid}`,
      oboAssertion: ssoToken,
      scopes: req.body.scopes,
      skipCache: true
    });
    res.json({ access_token: result?.accessToken });
  } catch (error) {
    if (error.errorCode === 'invalid_grant' || error.errorCode === 'interaction_required') {
      // This is expected if it's the user's first time running the app ( user must consent ) or the admin requires MFA
      res.status(403).json({ error: 'consent_required' }); // This error triggers the consent flow in the client.
    } else {
      // Unknown error
      res.status(500).json({ error: error.message });
    }
  }
}

////////////////////////
// create and run server
////////////////////////

const app = express();
const PORT = process.env.port || process.env.PORT || 8000;

// Support JSON payloads
app.use(express.json());
app.use(express.static(path.join(__dirname, 'client')));

// An example for using POST and with token validation using middleware
app.post('/api/token', validateJwt, async (req, res) => {
  await getAccessTokenOnBehalfOf(req, res);
});

app.listen(PORT, () => {
  console.log(`⚡️[server]: Server is running at http://localhost:${PORT}`);
});
```

## <a name="initialize-the-teams-msal2-provider"></a>Инициализация поставщика Teams MSAL2

Поставщики Graph набор средств Майкрософт обеспечивают проверку подлинности и доступ к microsoft Graph. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). Поставщик [Teams MSAL2](../providers/teams-msal2.md) обрабатывает все логики и взаимодействия, которые необходимо реализовать с Teams SDK для проверки подлинности пользователя.

В SSO-режиме убедитесь, что он `sso-url` / `ssoUrl` должен быть указать на API-поддержку.

# <a name="html"></a>[HTML](#tab/HTML)

Добавьте htmL-код `mgt-teams-msal2-provider` .

```HTML
<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/tabauth"
  scopes="User.Read,Mail.ReadBasic"
  sso-url="http://localhost:8000/api/token"
  http-method="POST"
  ></mgt-teams-msal2-provider>
```

Замените `<YOUR_CLIENT_ID>` с помощью клиентского ИД для приложения, `auth-popup-url` замените полный или относительный путь на страницу auth и `sso-url` замените полный или относительный путь к службе backend.

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)

Чтобы инициализировать поставщика в коде JavaScript, импортировать `TeamsMsal2Provider` и устанавливать `globalProvider`.

```TypeScript
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider, HttpMethod} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider({
  clientId: `<YOUR_CLIENT_ID>`,
  authPopupUrl: '/tabauth',
  scopes: ['User.Read','Mail.ReadBasic'],
  ssoUrl: 'http://localhost:8000/api/token',
  httpMethod: HttpMethod.POST
});
```
Замените `<YOUR_CLIENT_ID>` с помощью клиентского ИД для приложения, `authPopupUrl` замените полный или относительный путь на страницу auth и `ssoUrl` замените полный или относительный путь к службе backend.

---

## <a name="add-components"></a>Добавление компонентов

Теперь вы готовы добавить любой из компонентов Microsoft Graph набор средств. 

Вы можете добавлять компоненты в HTML, как обычно. Например, чтобы добавить компонент `Person` , добавьте следующий код в HTML.

```HTML
<mgt-person person-query="me"></mgt-person>
```

Если вы используете React, рекомендуется использовать React компоненты `mgt-react` вместо библиотеки. Дополнительные дополнительные [ссылки см. в Graph набор средств Microsoft React](./use-toolkit-with-react.md).

## <a name="test-the-sample"></a>Тестирование примера
Полный пример реализации см. [в Teams SSO Node Sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/teams-sso-node).

Если все настроено правильно, `Person` будет отрисовка компонента без необходимости входа.
>[!IMPORTANT]
>Если вы еще не дали предварительного согласия, может потребоваться согласие с помощью запроса.

## <a name="next-steps"></a>Дальнейшие действия
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задайте вопрос [в Microsoft Q&A](/answers/topics/microsoft-graph-toolkit.html).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
