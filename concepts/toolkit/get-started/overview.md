---
title: Начало работы с microsoft Graph набор средств
description: Начало работы с помощью microsoft Graph набор средств в приложении.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 09e69c51e4cbb693f9923b793a80b687c0afbddc
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477680"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Начало работы с microsoft Graph набор средств

Компоненты microsoft Graph набор средств легко можно добавить в ваше веб-приложение, SharePoint веб-часть или Microsoft Teams вкладки. Эти компоненты основаны на веб-стандартах и могут использоваться как в обычных проектах JavaScript, так и в популярных веб-инфраструктурах, таких как Reach, Angular, Vue.js и других.

Вы можете просмотреть это короткое видео, чтобы узнать, как быстро и легко начать работу с набор средств.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Пошаговая инструкция см. в руководстве [Get started with Microsoft Graph набор средств](/learn/modules/msgraph-toolkit-intro/). 

## <a name="set-up-your-microsoft-365-tenant"></a>Настройка клиента Microsoft 365
Чтобы развиваться с помощью набор средств, вам необходим доступ к Microsoft 365 клиента. Если у вас его нет, вы можете получить бесплатную подписку Microsoft 365 разработчика, присоединившись [к программе Microsoft 365 разработчика](https://developer.microsoft.com/microsoft-365/dev-program). Сведения о настройке подписки см. в материале [Настройка подписки Microsoft 365 разработчика](/office/developer-program/microsoft-365-developer-program-get-started).

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

Основной `@microsoft/mgt-element` пакет содержит только базовые классы, используемые для создания компонентов и поставщиков. Этот пакет предоставляет все необходимые классы и интерфейсы, необходимые для создания собственных компонентов, и экспортирует [интерфейс IProvider и класс SimpleProvider](../providers/custom.md) для создания настраиваемого поставщика.

<b>@microsoft/mgt-components</b>

Пакет `@microsoft/mgt-components` содержит все подключенные Graph microsoft, `Person`например , и `PeoplePicker`другие. 

**Поставщики**

Поставщики доступны через один пакет и могут быть установлены по мере необходимости. Доступны следующие пакеты поставщиков:

- <b>@microsoft/mgt-msal-provider</b>

    [`@microsoft/mgt-msal-provider`](../providers/msal.md) содержит и `MsalProvider` компонент `mgt-msal-provider` . Поставщик MSAL использует msal.js для проверки подлинности в веб-приложениях и прогрессивных веб-приложениях (PWAs).

- <b>@microsoft/mgt-msal2-provider</b>

    [`@microsoft/mgt-msal2-provider`](../providers/msal2.md) содержит и `Msal2Provider` компонент `mgt-msal2-provider` . Поставщик MSAL2 использует msal-browser для проверки подлинности в веб-приложениях и PWAs.

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) содержит и `TeamsProvider` компонент `mgt-teams-provider` . Поставщик Microsoft Teams включает проверку подлинности в Microsoft Teams вкладке.

-  <b>@microsoft/mgt-teams-msal2-provider</b>

    [`@microsoft/mgt-teams-msal2-provider`](../providers/teams.md) содержит и `TeamsMsal2Provider` компонент `mgt-teams-msal2-provider` . Поставщик Microsoft Teams MSAL2 включает проверку подлинности в Microsoft Teams вкладке.

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)содержит для `SharePointProvider` проверки подлинности в SharePoint среде. 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md)содержит приложение`ProxyProvider`, которое Graph через службу backend. 

<b>@microsoft/mgt</b>

Это `@microsoft/mgt` основной пакет, который включает все вышеперечисленные пакеты и повторно экспортирует их, чтобы они были доступны с помощью одного пакета, который можно установить. 

<b>@microsoft/mgt-react</b>

Пакет [`@microsoft/mgt-react`](./mgt-react.md) содержит все автоматически созданные React и принимает зависимость от `@microsoft/mgt` пакета.

<b>@microsoft/mgt-spfx</b>

Пакет [`@microsoft/mgt-spfx`](./mgt-spfx.md) содержит библиотеку SharePoint Framework, которая необходима для использования Microsoft Graph набор средств в SharePoint Framework решениях.

## <a name="next-steps"></a>Дальнейшие действия
Теперь вы готовы начать разработку с помощью microsoft Graph набор средств! Для начала работы доступны следующие руководства:

- [Регистрация приложения Azure Active Directory](./add-aad-app-registration.md)
- [Создание веб-приложения (JavaScript)](./build-a-web-app.md) (ванильный JavaScript)
- [Создание веб-приложения (React)](./use-toolkit-with-react.md)
- [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md)
- [Создание веб-части SharePoint](./build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
