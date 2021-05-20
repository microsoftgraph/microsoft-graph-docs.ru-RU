---
title: Начало работы с Microsoft Graph набор средств
description: Начать использовать систему Майкрософт Graph набор средств приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e84350a7835cac7914f5238110f74b3383047e13
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579594"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Начало работы с Microsoft Graph набор средств

Дополнительные компоненты майкрософт Graph набор средств могут быть легко добавлены в веб-приложение, SharePoint веб-часть или Microsoft Teams вкладки. Компоненты основаны на веб-стандартах и могут быть использованы как в простых проектах JavaScript, так и в популярных веб-инфраструктурах, таких как Reach, Angular, Vue.js и многое другое.

Вы можете посмотреть это короткое видео, чтобы увидеть, как быстро и легко начать работу с набор средств.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Для пошагового учебника [](/learn/modules/msgraph-toolkit-intro/)с Graph набор средств м. 

## <a name="set-up-your-microsoft-365-tenant"></a>Настройка клиента Microsoft 365
Для того, чтобы развиваться с набор средств, вам нужен доступ к Microsoft 365 арендатору. Если у вас его нет, вы можете получить бесплатную подписку Microsoft 365 разработчика, [присоединившись к Microsoft 365 developer Program.](https://developer.microsoft.com/microsoft-365/dev-program) Подробную информацию о настройке подписки можно найти в [приложении Microsoft 365 разработчика.](/office/developer-program/microsoft-365-developer-program-get-started)

## <a name="set-up-your-development-environment"></a>Настройка среды разработки
Для разработки с набор средств, вам понадобится текстовый редактор или IDE. Вы можете использовать редактор или IDE по вашему выбору или установить [и Visual Studio Code](https://code.visualstudio.com/download) бесплатно. Вам также понадобится современный веб-браузер, как Microsoft Edge, Google Chrome, или Firefox. Вам также понадобится LTS версия Node.js, которую вы можете установить с [nodejs.org](https://nodejs.org).

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
Теперь вы можете со ссылкой на все компоненты страницы, которую вы используете:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a>Пакеты NPM

Microsoft Graph набор средств состоит из нескольких пакетов NPM, что позволяет включать только код, который вам нужен для ваших приложений.

<b>@microsoft/mgt-элемент</b>

Это `@microsoft/mgt-element` основной пакет, содержащий только базовые классы, используемые для создания компонентов и поставщиков. Этот пакет предоставляет все необходимые классы и интерфейсы, необходимые для создания собственных компонентов и [экспорта интерфейса IProvider и класса SimpleProvider](../providers/custom.md) для создания пользовательских поставщиков.

<b>@microsoft/mgt-компоненты</b>

Пакет `@microsoft/mgt-components` содержит все веб-компоненты microsoft Graph подключенные веб-компоненты, `Person` такие как , и многое `PeoplePicker` другое. 

**Поставщики**

Поставщики доступны через единый пакет и могут быть установлены по мере необходимости. Доступны следующие пакеты поставщиков:

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) содержит компонент `MsalProvider` `mgt-msal-provider` и компонент. Поставщик MSAL использует вебmsal.js для проверки подлинности в веб-приложениях и прогрессивных веб-приложениях (PWAs).

- <b>@micosoft/mgt-msal2-провайдер</b>

    [`@micosoft/mgt-msal2-provider`](../providers/msal2.md) содержит компонент `Msal2Provider` `mgt-msal2-provider` и компонент. Поставщик MSAL использует msal-браузер для аутентификации в веб-приложениях и PWAs.

-  <b>@microsoft/mgt-команд-провайдер</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) содержит компонент `TeamsProvider` `mgt-teams-provider` и компонент. Поставщик Microsoft Teams позволяет аутентификацию в Microsoft Teams вкладке.

- <b>@microsoft/mgt-sharepoint-провайдер</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)содержит `SharePointProvider` аутентификацию в SharePoint среде. 

- <b>@microsoft/mgt-прокси-провайдер</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md)содержит `ProxyProvider` приложение, которое прокси-Graph звонки через службу бэкэнда. 

<b>@microsoft/mgt</b>

Основной `@microsoft/mgt` пакет, который включает в себя все вышеперечисленные пакеты и реапорт их, чтобы они были доступны через один пакет, который вы можете установить. 

<b>@microsoft/mgt-реакция</b>

Пакет [`@microsoft/mgt-react`](./mgt-react.md) содержит все автоматически генерируемые React компоненты и принимает зависимость от `@microsoft/mgt` пакета.

<b>@microsoft/mgt-spfx</b>

Пакет [`@microsoft/mgt-spfx`](./mgt-spfx.md) содержит библиотеку SharePoint Framework, которая требуется для использования майкрософт Graph набор средств в SharePoint Framework решениях.

## <a name="polyfills"></a>Полизаполнение

Если вы используете модули ES6 из пакета npm и ориентируетесь [на браузер, такой как IE11, который](https://caniuse.com/#search=components) не поддерживает веб-компоненты на родном языке, вам нужно будет включить полифилли в свой проект, так как они не включены автоматически. Полифилы помогают заполнить недостающие возможности браузера в браузерах, которые все еще находятся в процессе обновления для поддержки стандартов Web Component. Для получения инструкций и узнать больше, [см поликлифы документации](https://www.webcomponents.org/polyfills). 

Полифилы уже включены, если вы используете набор средств через скрипт mgt-loader.

## <a name="next-steps"></a>Дальнейшие действия
Теперь вы готовы начать разработку с помощью Microsoft Graph набор средств! Доступны следующие руководства, которые помогут вам начать работу:

- [Регистрация приложения Azure Active Directory](./add-aad-app-registration.md)
- [Создайте веб-приложение (JavaScript)](./build-a-web-app.md) (ванильный JavaScript)
- [Создание веб-приложения (React)](./use-toolkit-with-react.md)
- [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md)
- [Создание веб-части SharePoint](./build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
