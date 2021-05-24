---
title: Начало работы с microsoft Graph набор средств
description: Начало работы с помощью microsoft Graph набор средств в приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 68260cf83f0e9bec34d2c3b23911d04c53143e76
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629156"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Начало работы с microsoft Graph набор средств

Компоненты microsoft Graph набор средств легко можно добавить в ваше веб-приложение, SharePoint веб-часть или Microsoft Teams вкладки. Компоненты основаны на веб-стандартах и могут использоваться как в обычных проектах JavaScript, так и в популярных веб-инфраструктурах, таких как Reach, Angular, Vue.js и других.

Вы можете просмотреть это короткое видео, чтобы узнать, как быстро и легко начать работу с набор средств.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Пошаговую инструкцию см. в руководстве [Get started with Microsoft Graph набор средств.](/learn/modules/msgraph-toolkit-intro/) 

## <a name="set-up-your-microsoft-365-tenant"></a>Настройка клиента Microsoft 365
Чтобы развиваться с помощью набор средств, вам необходим доступ к Microsoft 365 клиента. Если у вас его нет, вы можете получить бесплатную подписку Microsoft 365 разработчика, присоединившись [к программе Microsoft 365 разработчика](https://developer.microsoft.com/microsoft-365/dev-program). Сведения о настройке подписки см. в материале [Настройка подписки Microsoft 365 разработчика.](/office/developer-program/microsoft-365-developer-program-get-started)

## <a name="set-up-your-development-environment"></a>Настройка среды разработки
Для разработки набор средств текстового редактора или IDE. Вы можете использовать редактор или IDE по вашему выбору или установить и [использовать Visual Studio Code](https://code.visualstudio.com/download) бесплатно. Вам также понадобится современный веб-браузер, Microsoft Edge, Google Chrome или Firefox. Вам также понадобится версия LTS Node.js, которую можно установить с [nodejs.org](https://nodejs.org).

## <a name="using-the-microsoft-graph-toolkit"></a>Использование microsoft Graph набор средств
Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Чтобы использовать Toolkit в загрузчике Microsoft Graph Toolkit, добавьте ссылку в сценарий кода:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения. Чтобы использовать модули ES6, добавьте в проект пакет npm:

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

Microsoft Graph набор средств состоит из нескольких пакетов NPM, что позволяет включать только код, необходимый для приложений.

<b>@microsoft/mgt-element</b>

Основной пакет содержит только базовые классы, используемые для создания `@microsoft/mgt-element` компонентов и поставщиков. Этот пакет предоставляет все необходимые классы и интерфейсы, необходимые для создания собственных компонентов, и экспортирует [интерфейс IProvider и класс SimpleProvider](../providers/custom.md) для создания настраиваемого поставщика.

<b>@microsoft/mgt-components</b>

Пакет содержит все подключенные Graph Майкрософт `@microsoft/mgt-components` веб-компоненты, такие как , и `Person` `PeoplePicker` более. 

**Поставщики**

Поставщики доступны через один пакет и могут быть установлены по мере необходимости. Доступны следующие пакеты поставщиков:

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) содержит `MsalProvider` и `mgt-msal-provider` компонент. Поставщик MSAL использует msal.js для проверки подлинности в веб-приложениях и прогрессивных веб-приложениях (PWAs).

- <b>@micosoft/mgt-msal2-provider</b>

    [`@micosoft/mgt-msal2-provider`](../providers/msal2.md) содержит `Msal2Provider` и `mgt-msal2-provider` компонент. Поставщик MSAL использует msal-browser для проверки подлинности в веб-приложениях и PWAs.

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) содержит `TeamsProvider` и `mgt-teams-provider` компонент. Поставщик Microsoft Teams включает проверку подлинности в Microsoft Teams вкладке.

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)содержит `SharePointProvider` для проверки подлинности в SharePoint среде. 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md)содержит `ProxyProvider` приложение, которое Graph через службу backend. 

<b>@microsoft/mgt</b>

Это основной пакет, который включает все вышеперечисленные пакеты и повторно экспортирует их, чтобы они были доступны с помощью одного `@microsoft/mgt` пакета, который можно установить. 

<b>@microsoft/mgt-react</b>

Пакет содержит все автоматически созданные [`@microsoft/mgt-react`](./mgt-react.md) React и принимает зависимость от `@microsoft/mgt` пакета.

<b>@microsoft/mgt-spfx</b>

Пакет содержит библиотеку SharePoint Framework, которая необходима для использования [`@microsoft/mgt-spfx`](./mgt-spfx.md) Microsoft Graph набор средств в SharePoint Framework решениях.

## <a name="next-steps"></a>Дальнейшие действия
Теперь вы готовы начать разработку с помощью microsoft Graph набор средств! Для начала работы доступны следующие руководства:

- [Регистрация приложения Azure Active Directory](./add-aad-app-registration.md)
- [Создание веб-приложения (JavaScript)](./build-a-web-app.md) (ванильный JavaScript)
- [Создание веб-приложения (React)](./use-toolkit-with-react.md)
- [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md)
- [Создание веб-части SharePoint](./build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
