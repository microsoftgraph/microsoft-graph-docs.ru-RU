---
title: Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств
description: Начало создания вкладки Microsoft Teams с помощью microsoft Graph набор средств.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 915bbe562fec9ef0bcbd5ae6d67d8497ea7e72eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963276"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств

В этом разделе описывается, как начать работу с помощью microsoft Graph набор средств в решении Microsoft Teams. Начало работы включает в себя следующие действия:

1. Создайте новое приложение Teams с помощью настраиваемой вкладки.
2. Добавьте microsoft Graph набор средств.
3. Инициализация поставщика Microsoft Teams.
4. Создание всплываемой страницы auth.
5. Добавление компонентов.
6. Проверьте приложение.

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>Создание нового приложения Teams с помощью настраиваемой вкладки

Самый простой способ создания нового приложения Teams — использовать расширение [Microsoft Teams набор средств](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) для Visual Studio кода. Следуйте инструкциям по [настройкам нового проекта Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project) Когда вы доберелись до экрана **Добавить возможности,** выберите **вкладку**, а затем **личные вкладки**.

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление Microsoft Graph Toolkit

Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm. Чтобы использовать набор средств, вам также потребуется [SDK Microsoft Teams.](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)

### <a name="use-via-mgt-loader"></a>Использование с помощью mgt-loader
Чтобы использовать набор средств и команд SDK через погрузчики, добавьте в файл следующие `<head>` `public/index.html` ссылки:

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

В `public/index.html` , добавьте поставщика Teams в , как `<body>` показано.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/auth.html"
></mgt-teams-provider>
```

Замените `<YOUR_CLIENT_ID>` на идентификатор клиента для своего приложения. 

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

Чтобы получить клиентский ID, необходимо зарегистрировать приложение Azure Active Directory. Выполните действия в статье [Создание приложения Azure Active Directory.](./add-aad-app-registration.md)

Обязательно установите **URI перенаправления** в регистрации приложения, чтобы указать на `auth.html` страницу. Например, если вы работаете с `localhost:3000` приложением, установите URI перенаправления. `https://localhost:3000/auth.html`

>**Примечание**. MSAL поддерживает только неявный поток для OAuth. Включите неявный поток в своем приложении на портале Azure (он не включен по умолчанию). В области **Проверка подлинности** найдите раздел **Неявное предоставление** и установите флажки **Маркеры доступа** и **Маркеры идентификаторов**. 

## <a name="create-the-auth-popup-page"></a>Создание всплываемой страницы auth

Чтобы разрешить пользователям войти, необходимо указать URL-адрес, который приложение Teams откроет в всплывающее приложение, чтобы следовать потоку проверки подлинности. URL-адрес должен быть в домене, и все, что нужно сделать на этой странице, это вызвать `TeamsProvider.handleAuth()` метод.

Это можно сделать, добавив новый файл в папку (который должен быть на том же уровне, что и) и добавив `auth.html` `public` следующий `index.html` код: 

```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsProvider.handleAuth();
    </script>
  </body>
</html>
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

Чтобы протестировать приложение, вы можете установить приложение в Teams с помощью расширения Teams набор средств. Откройте расширение Teams набор средств и нажмите **кнопку Open Microsoft Teams набор средств.** Щелкните **App Studio** в левом меню, прокрутите вниз и выберите Тест **и Распространение**, а затем **Установите**. Команды будут открываться в браузере, и вы будете перенаправлены на созданную вкладку. Вы должны иметь возможность видеть компонент Login и использовать его для входа в приложение.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с этим пошаговом руководстве по [построению вкладки Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
