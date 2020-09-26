---
title: Создание вкладки Microsoft Teams с набором средств Microsoft Graph
description: Приступая к созданию вкладки Microsoft Teams с помощью набора инструментов Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c4ed3396d05c865fd483bc8b007cdc743c0e8419
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288541"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Создание вкладки Microsoft Teams с набором средств Microsoft Graph

В этом разделе описывается, как приступить к использованию набора средств Microsoft Graph в решении Microsoft Teams. Приступая к работе состоит из следующих этапов:

1. Создайте новое приложение Teams с настраиваемой вкладкой.
2. Настройка ngrok и создание туннеля.
3. Добавьте набор инструментов Microsoft Graph.
4. Инициализация поставщика Microsoft Teams.
5. Создайте всплывающую страницу проверки подлинности.
6. Добавление компонентов.
7. Протестируйте приложение.

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>Создание нового приложения Teams с настраиваемой вкладкой

Самый простой способ создать приложение Teams — использовать [расширение набора средств Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) для Visual Studio Code. Следуйте инструкциям по [настройке нового проекта Teams](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project). При **переходе**на экран **добавить возможности** выберите **вкладку**, а затем щелкните Личные.

## <a name="set-up-ngrok-and-create-a-tunnel"></a>Настройка ngrok и создание туннеля

Чтобы протестировать приложение позже, вам потребуется разместить приложение по общедоступному URL-адресу с помощью HTTPS. Установите [ngrok](https://ngrok.com/download) и создайте туннель из Интернета на localhost: 3000 с помощью следующей команды:

```bash
ngrok http 3000
```
В каталоге проекта выберите `.publish\Development.env` файл и замените значение на `baseUrl0` URL-адрес ngrok.

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление набора средств Microsoft Graph

Вы можете использовать набор средств Microsoft Graph в приложении, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM. Чтобы использовать набор средств, вам также понадобится [пакет SDK Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).

### <a name="use-via-mgt-loader"></a>Использование с помощью упр. загрузчиком
Чтобы использовать набор средств и пакет SDK Teams с помощью загрузчиков, добавьте следующие ссылки `public/index.html` :

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Использование через NPM (модули ES6)
Использование набора средств с помощью модулей ES6 даст вам полный контроль над процессом создания пучка и позволяет объединить только код, который требуется для приложения. Чтобы использовать модули ES6, добавьте в проект пакеты NPM для набора средств и пакета SDK Microsoft teams:

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>Инициализация поставщика Teams

Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Чтобы узнать больше, ознакомьтесь со статьей [Использование поставщиков](../providers.md). [Поставщик Teams](../providers/teams.md) обрабатывает всю логику и взаимодействия, которые необходимо реализовать с помощью пакета SDK Teams для проверки подлинности пользователя.

Для инициализации поставщика можно использовать HTML-код или код JavaScript. 

### <a name="initialize-in-html"></a>Инициализация в HTML

`public/index.html`Добавьте поставщика Teams, как показано ниже.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

Замените `<YOUR_CLIENT_ID>` идентификатором клиента для вашего приложения и `<YOUR_NGROK_URL>` созданным URL-адресом ngrok.

### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Чтобы инициализировать поставщик в коде JavaScript, откройте `src/components/App.js` файл в каталоге проекта. Импортируйте поставщика Teams и инициализируйте поставщик.

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
Замените `<YOUR_CLIENT_ID>` идентификатором клиента для вашего приложения.

### <a name="creating-an-appclient-id"></a>Создание идентификатора приложения или клиента
Чтобы получить идентификатор клиента, необходимо [зарегистрировать приложение](../../auth-register-app-v2.md) в Azure AD. Обязательно добавьте URL-адрес ngrok с полным путем к всплывающей странице проверки подлинности в URI перенаправления (например, `https://<YOUR_NGROK_URL>/auth.html` ).
>**Note**: MSAL поддерживает только неявный поток для OAuth. Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен). В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**. 

## <a name="create-the-auth-popup-page"></a>Создание всплывающей страницы проверки подлинности

Чтобы разрешить пользователям входить в систему, необходимо указать URL-адрес, который приложение Teams будет открывать во всплывающем окне, чтобы выполнить этот процесс проверки подлинности. URL-адрес должен находиться в вашем домене, и вся эта страница должна быть вызвана `TeamsProvider.handleAuth()` методом.

Это можно сделать в HTML-коде, добавив новый `auth.html` файл в `public` папку (который должен находиться на том же уровне, что `index.html` и), и добавьте следующий код: 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>Добавление компонентов

Теперь вы готовы добавить на вкладку любой из компонентов набора средств Microsoft Graph. 

Вы можете добавлять компоненты в HTML-код обычным образом. Например, чтобы добавить компонент входа, добавьте приведенный ниже код в текст `index.html` :

```html
<mgt-login></mgt-login>
```

Кроме того, вы можете добавить компоненты в ЖСКС в компонент табуляции. Мы рекомендуем использовать `mgt-react` библиотеку, если вы создали приложение Teams с помощью расширения набора средств Microsoft Teams. Дополнительные сведения см. [Использование набора инструментов Microsoft Graph с откликом](./use-toolkit-with-react.md#using-mgt-react)

Сначала установите `mgt-react` :

```bash
npm install @microsoft/mgt-react
```

Выберите `src/components/Tab.js` файл и импортируйте компоненты, которые вы хотите использовать, из `mgt-react` библиотеки. Например, чтобы добавить компонент, выполните `Login` следующие действия:

```js
import { Login } from "@microsoft/mgt-react"
```

Затем добавьте компонент в `return()` оператор `render()` метода метода `Tab` :

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a>Тестирование приложения

Постройте и запустите приложение с помощью следующих команд:
```bash
npm install
npm start
```

Чтобы протестировать приложение, необходимо загрузить приложение в Teams. Откройте клиент Microsoft Teams, выберите пункт **...** в левом меню и перейдите в **Приложение App Studio**. Перейдите на вкладку **редактор манифестов** и выберите пункт **Импорт существующего приложения**.

Откройте каталог проекта и отправьте файл **Development.zip** в папку **. Publish** .

После загрузки приложения Прокрутите меню слева вниз и выберите команду **проверить и распределить**. Нажмите кнопку **установить** , а затем кнопку **Добавить**. Вы будете перенаправлены на созданную вами вкладку.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с пошаговыми руководствами по [созданию вкладки Teams](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).
- Опробуйте компоненты в [интерактивная среда](https://mgt.dev).
- Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).
- Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).