---
title: Создание вкладки Microsoft Teams с помощью microsoft Graph набор средств
description: Начало создания вкладки Microsoft Teams с помощью microsoft Graph набор средств.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 9cd548e78ff21577df852a28be76e45144bfb91d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663920"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Создание вкладки Microsoft Teams с помощью microsoft Graph набор средств

В этом разделе описывается, как начать использовать microsoft Graph набор средств в решении Microsoft Teams. Начало работы состоит из следующих этапов:

1. Создайте новое приложение Teams с помощью настраиваемой вкладки.
2. Настройка ngrok и создание туннеля.
3. Добавьте microsoft Graph набор средств.
4. Инициализация поставщика Microsoft Teams.
5. Создайте всплывающее страницу auth.
6. Добавление компонентов.
7. Протестировать приложение.

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>Создание нового приложения Teams с помощью настраиваемой вкладки

Самый простой способ создать приложение Teams — использовать расширение [Microsoft Teams набор средств](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) для Visual Studio Code. Следуйте инструкциям, чтобы [настроить новый проект Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project) When you get to the **Add capabilities** screen, select **Tab**, and then **Personal tab**.

## <a name="set-up-ngrok-and-create-a-tunnel"></a>Настройка ngrok и создание туннеля

Чтобы протестировать приложение позже, необходимо будет провести его по общедоступным URL-адресам с помощью HTTPS. Установите [ngrok](https://ngrok.com/download) и создайте туннель из Интернета в localhost:3000 с помощью следующей команды:

```bash
ngrok http 3000
```
В каталоге проекта найдите файл и замените значение `.publish\Development.env` `baseUrl0` url-адреса ngrok.

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление учетной записи Microsoft Graph набор средств

Вы можете использовать microsoft Graph набор средств в приложении, ссылаясь на загрузчик напрямую (с помощью unpkg) или установив пакет npm. Чтобы использовать набор средств, вам также потребуется [SDK Microsoft Teams.](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)

### <a name="use-via-mgt-loader"></a>Использование с помощью mgt-loader
Чтобы использовать набор средств и Teams SDK через загрузчики, добавьте следующие ссылки `public/index.html` на:

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Использование через npm (модули ES6)
Использование набор средств с помощью модулей ES6 дает полный контроль над процессом пакетизации и позволяет объединить только код, необходимый для вашего приложения. Чтобы использовать модули ES6, добавьте пакеты npm для набор средств и пакета Microsoft Teams SDK в проект:

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>Инициализация поставщика Teams

Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные см. [в этой теме.](../providers/providers.md) Поставщик [Teams обрабатывает](../providers/teams.md) всю логику и взаимодействия, которые необходимо реализовать с помощью SDK Teams для проверки подлинности пользователя.

Вы можете инициализировать поставщика в коде HTML или JavaScript. 

### <a name="initialize-in-html"></a>Инициализация в HTML

Добавьте `public/index.html` поставщика Teams, как показано ниже.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

Замените на ИД клиента для приложения и `<YOUR_CLIENT_ID>` `<YOUR_NGROK_URL>` созданный URL-адрес ngrok.

### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Чтобы инициализировать поставщика в коде JavaScript, найдите файл `src/components/App.js` в каталоге проекта. Импорт поставщика Teams и инициализация поставщика.

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
Замените `<YOUR_CLIENT_ID>` его на ИД клиента для вашего приложения.

### <a name="creating-an-appclient-id"></a>Создание приложения или ИД клиента
Чтобы получить ИД клиента, необходимо зарегистрировать приложение [в](../../auth-register-app-v2.md) Azure AD. Обязательно добавьте URL-адрес ngrok с полным путем во всплывающее окне auth в URIS перенаправления `https://<YOUR_NGROK_URL>/auth.html` (например).
>**Примечание.** MSAL поддерживает только неявный поток для OAuth. Обязательно включите неявный поток в приложении на портале Azure (по умолчанию он не включен). В **разделе "Проверка подлинности"** найдите раздел неявного предоставления и выберите для маркеров **доступа** и **маркеров ID** свои почтовые ящики.  

## <a name="create-the-auth-popup-page"></a>Создание всплываемой страницы auth

Чтобы разрешить пользователям выполнять вход, необходимо указать URL-адрес, который приложение Teams откроет во всплывающее приложение, чтобы следовать потоку проверки подлинности. URL-адрес должен быть в вашем домене, и все, что нужно сделать, это вызвать `TeamsProvider.handleAuth()` метод.

Это можно сделать в HTML-коде, добавив новый файл в папку (который должен быть на том же уровне, что и) и добавив `auth.html` `public` следующий `index.html` код: 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>Добавление компонентов

Теперь все готово к добавлению на вкладку любых компонентов microsoft Graph набор средств microsoft Graph. 

Вы можете добавлять компоненты в HTML обычным образом. Например, чтобы добавить компонент входа, добавьте в текст кода `index.html` ниже:

```html
<mgt-login></mgt-login>
```

Кроме того, вы можете добавить компоненты jSX в компонент Tab. Рекомендуем использовать библиотеку, если вы создали приложение Teams с помощью набор средств `mgt-react` Microsoft Teams. Дополнительные данные см. [в набор средств Microsoft Graph с React](./use-toolkit-with-react.md)

Сначала `mgt-react` установите:

```bash
npm install @microsoft/mgt-react
```

Найдите файл и импортировать компоненты, которые вы хотите использовать `src/components/Tab.js` из `mgt-react` библиотеки. Например, чтобы добавить `Login` использование компонента:

```js
import { Login } from "@microsoft/mgt-react"
```

Затем добавьте компонент в выписку `return()` метода `render()` `Tab` :

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a>Тестирование приложения

Создайте и запустите приложение с помощью следующих команд:
```bash
npm install
npm start
```

Чтобы протестировать приложение, необходимо отправить приложение в Teams. Откройте клиент Microsoft Teams, выберите **пункт ...в** левом меню и перейдите в **App Studio.** Перейдите **на вкладку "Редактор** манифеста" и выберите **"Импорт существующего приложения".**

Найдите каталог проекта и загрузите **Development.zip** в папку **.publish.**

После загрузки приложения прокрутите меню слева вниз и выберите пункт **"Тестирование и распространение".** Нажмите **кнопку "Установить",** а затем нажмите **кнопку "Добавить".** Вы будете перенаправлены на созданную вкладку.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с этим пошаговом руководстве по [построению вкладки Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)
- Попробуйте компоненты в игровой [области.](https://mgt.dev)
- Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)
- Сообщать об ошибках или оставлять запросы на функции на [GitHub.](https://aka.ms/mgt)