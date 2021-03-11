---
title: Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств
description: Начало создания вкладки Microsoft Teams с помощью microsoft Graph набор средств.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 757c7eb8a94b0f6936a21f5ecb6f126cde36b6ad
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721567"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств

В этом разделе описывается, как начать работу с помощью microsoft Graph набор средств в решении Microsoft Teams. Начало работы включает в себя следующие действия:

1. Создайте новое приложение Teams с помощью настраиваемой вкладки.
2. Настройка ngrok и создание туннеля.
3. Добавьте microsoft Graph набор средств.
4. Инициализация поставщика Microsoft Teams.
5. Создание всплываемой страницы auth.
6. Добавление компонентов.
7. Проверьте приложение.

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>Создание нового приложения Teams с помощью настраиваемой вкладки

Самый простой способ создания нового приложения Teams — использовать расширение [Microsoft Teams набор средств](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) для Visual Studio кода. Следуйте инструкциям по [настройкам нового проекта Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project) Когда вы доберелись до экрана **Добавить возможности,** выберите **вкладку**, а затем **личные вкладки**.

## <a name="set-up-ngrok-and-create-a-tunnel"></a>Настройка ngrok и создание туннеля

Чтобы протестировать приложение позже, необходимо будет использовать HTTPS-адрес с общедоступным URL-адресом. Установите [ngrok](https://ngrok.com/download) и создайте туннель из Интернета в localhost:3000 со следующей командой:

```bash
ngrok http 3000
```
В каталоге проектов найдите файл и замените значение `.publish\Development.env` `baseUrl0` url-адресом ngrok.

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление Microsoft Graph Toolkit

Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm. Чтобы использовать набор средств, вам также потребуется [SDK Microsoft Teams.](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)

### <a name="use-via-mgt-loader"></a>Использование с помощью mgt-loader
Чтобы использовать набор средств и команд SDK через погрузчики, добавьте следующие ссылки `public/index.html` на:

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Использование через npm (модули ES6)
Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения. Чтобы использовать модули ES6, добавьте пакеты npm как для набор средств, так и для SDK Microsoft Teams:

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>Инициализация поставщика Teams

Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). Поставщик [Teams обрабатывает](../providers/teams.md) все логики и взаимодействия, которые необходимо реализовать с командой SDK для проверки подлинности пользователя.

Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript. 

### <a name="initialize-in-html"></a>Инициализация в HTML

В `public/index.html` , добавьте поставщика Teams, как показано.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

Замените `<YOUR_CLIENT_ID>` с помощью клиентского ИД для приложения и `<YOUR_NGROK_URL>` созданного URL-адреса ngrok.

### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Чтобы инициализировать поставщика в коде JavaScript, найдите `src/components/App.js` файл в каталоге проекта. Импорт поставщика teams и инициализация поставщика.

```js
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
Замените `<YOUR_CLIENT_ID>` на идентификатор клиента для своего приложения.

### <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](../../auth-register-app-v2.md) в Azure AD. Обязательно добавьте URL-адрес ngrok с полным путем к всплываемой странице auth в URL-адреса перенаправления (например, `https://<YOUR_NGROK_URL>/auth.html` ).
>**Примечание**. MSAL поддерживает только неявный поток для OAuth. Включите неявный поток в своем приложении на портале Azure (он не включен по умолчанию). В области **Проверка подлинности** найдите раздел **Неявное предоставление** и установите флажки **Маркеры доступа** и **Маркеры идентификаторов**. 

## <a name="create-the-auth-popup-page"></a>Создание всплываемой страницы auth

Чтобы разрешить пользователям войти, необходимо указать URL-адрес, который приложение Teams откроет в всплывающее приложение, чтобы следовать потоку проверки подлинности. URL-адрес должен быть в домене, и все, что нужно сделать на этой странице, это вызвать `TeamsProvider.handleAuth()` метод.

Вы можете сделать это в HTML, добавив новый файл в папку (который должен быть на том же уровне, что и) и добавив `auth.html` `public` следующий `index.html` код: 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>Добавление компонентов

Теперь вы готовы добавить в вкладку любой набор средств Microsoft Graph. 

Вы можете добавлять компоненты в HTML, как обычно. Например, чтобы добавить компонент Login, добавьте ниже код в тело `index.html` вашего :

```html
<mgt-login></mgt-login>
```

Или можно добавить компоненты jSX в компонент Tab. Рекомендуется использовать библиотеку, если вы создали приложение Teams с помощью расширения `mgt-react` Microsoft Teams набор средств. Дополнительные данные см. в [набор средств Microsoft Graph с React](./use-toolkit-with-react.md)

Во-первых, `mgt-react` установите:

```bash
npm install @microsoft/mgt-react
```

Найдите `src/components/Tab.js` файл и импортируете компоненты, которые необходимо использовать из `mgt-react` библиотеки. Например, чтобы добавить использование `Login` компонентов:

```js
import { Login } from "@microsoft/mgt-react"
```

Затем добавьте компонент в утверждение `return()` метода `render()` `Tab` :

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

Чтобы протестировать приложение, необходимо загрузить приложение в Teams. Откройте клиент Microsoft Teams, выберите **... в левом** меню и перейдите в **App Studio**. Щелкните **вкладку Редактор Манифеста** и **выберите Импорт существующего приложения.**

Найдите каталог проекта и загрузите **Development.zip** файл внутри **папки .publish.**

После загрузки приложения прокрутите в левом меню и выберите **Test and Distribute**. Нажмите **кнопку Установка** и нажмите кнопку **Добавить**. Вы будете перенаправлены на созданную вкладку.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с этим пошаговом руководстве по [построению вкладки Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
