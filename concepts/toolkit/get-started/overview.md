---
title: Начало работы с microsoft Graph набор средств
description: Начало работы с microsoft Graph набор средств в приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: f1451213822e2489f04bb454c355125ed95b1aed
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664130"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Начало работы с microsoft Graph набор средств

Компоненты набор средств Microsoft Graph можно легко добавить в веб-приложение, веб-часть SharePoint или на вкладки Microsoft Teams. Эти компоненты основаны на веб-стандартах и могут использоваться как в обычных проектах JavaScript, так и в популярных веб-платформах, таких как Reach, Angular, Vue.js и других.

Вы можете посмотреть это короткое видео, чтобы узнать, как быстро и просто начать работу с набор средств.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a>Настройка клиента Microsoft 365
Для разработки с помощью набор средств вам нужен доступ к клиенту Microsoft 365. Если у вас ее нет, вы можете получить бесплатную подписку разработчика Microsoft 365, присоединившись к программе для [разработчиков Microsoft 365.](https://developer.microsoft.com/microsoft-365/dev-program) Подробные сведения о настройке подписки см. в сведениях о настройке подписки разработчика [Microsoft 365.](/office/developer-program/microsoft-365-developer-program-get-started)

## <a name="set-up-your-development-environment"></a>Настройка среды разработки
Для разработки с набор средств потребуется текстовый редактор или IDE. Вы можете использовать редактор или IDE по вашему выбору или установить и [использовать Visual Studio Code](https://code.visualstudio.com/download) бесплатно. Вам также потребуется современный веб-браузер, например Microsoft Edge, Google Chrome или Firefox. Вам также потребуется версия LTS Node.js, которую можно установить из [nodejs.org.](https://nodejs.org)

## <a name="using-the-microsoft-graph-toolkit"></a>Использование microsoft Graph набор средств
Вы можете использовать microsoft Graph набор средств в приложении, ссылаясь на загрузчик напрямую (с помощью unpkg) или установив пакет npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Чтобы использовать набор средств mgt-loader, добавьте ссылку в сценарии в код:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
Использование набор средств с помощью модулей ES6 дает полный контроль над процессом пакетизации и позволяет объединить только код, необходимый для вашего приложения. Чтобы использовать модули ES6, добавьте пакет npm в проект:

```cmd
npm install @microsoft/mgt
```
Теперь вы можете ссылаться на все компоненты страницы, которые вы используете:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a>Пакеты NPM

Microsoft Graph набор средств состоит из нескольких пакетов NPM, что позволяет включать только код, необходимый для ваших приложений.

<b>@microsoft/mgt-element</b>

Основной пакет содержит только базовые классы, используемые для создания `@microsoft/mgt-element` компонентов и поставщиков. Этот пакет предоставляет все необходимые классы и интерфейсы, необходимые для создания собственных компонентов, и экспортирует [интерфейс IProvider](../providers/custom.md) и класс SimpleProvider для создания пользовательских поставщиков.

<b>@microsoft/mgt-components</b>

Пакет `@microsoft/mgt-components` содержит все веб-компоненты, подключенные к Microsoft Graph, такие как `Person` , и `PeoplePicker` другие. 

**Поставщики**

Поставщики доступны через один пакет и могут быть установлены по мере необходимости. Доступны следующие пакеты поставщиков:

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) содержит и `MsalProvider` `mgt-msal-provider` компонент. Поставщик msal использует msal.js проверки подлинности в веб-приложениях и PWAS.

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) содержит и `TeamsProvider` `mgt-teams-provider` компонент. Поставщик Microsoft Teams включает проверку подлинности в приложении вкладок Microsoft Teams.

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) содержит данные `SharePointProvider` для проверки подлинности в среде SharePoint. 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md) содержит `ProxyProvider` приложение, которое прокси-сервер Graph вызывает через серверную службу. 

<b>@microsoft/mgt</b>

Это основной пакет, который включает все вышеперечисленные пакеты и повторно экспортирует их, чтобы они были доступны через один `@microsoft/mgt` пакет, который можно установить. 

<b>@microsoft/mgt-react</b>

Пакет содержит все автоматически созданные компоненты React и принимает [`@microsoft/mgt-react`](./mgt-react.md) зависимость от `@microsoft/mgt` пакета.

## <a name="polyfills"></a>Polyfills

Если вы используете модули ES6 из пакета npm и используете браузер, такой как [IE11,](https://caniuse.com/#search=components) который не поддерживает веб-компоненты по умолчанию, вам потребуется включить в проект полифайли, так как они не включаются автоматически. Polyfills помогают заполнить отсутствующие возможности браузера в браузерах, которые все еще находятся в процессе обновления для поддержки стандартов веб-компонентов. Инструкции и дополнительные инструкции см. в документации [по полифайлам.](https://www.webcomponents.org/polyfills) 

Полизаполнели уже включены, если вы используете набор средств с помощью скрипта mgt-loader.

## <a name="next-steps"></a>Дальнейшие действия
Теперь вы готовы приступить к разработке с помощью microsoft Graph набор средств! Для начала работы доступны следующие руководства:

- [Регистрация приложения Azure Active Directory](./add-aad-app-registration.md)
- [Создание веб-приложения (JavaScript)](./build-a-web-app.md) (javaScript)
- [Создание веб-приложения (React)](./use-toolkit-with-react.md)
- [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md)
- [Создание веб-части SharePoint](./build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
