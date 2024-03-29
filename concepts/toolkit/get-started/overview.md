---
title: Начало работы с Microsoft Graph Toolkit
description: Узнайте, как настроить клиент Microsoft 365 и среду разработки для использования Microsoft Graph Toolkit. Установите пакеты NPM для компонентов и поставщиков.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 3e4711003808dfc97536b648fbd02a1ee40b78b2
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577716"
---
# <a name="get-started-with-microsoft-graph-toolkit"></a>Начало работы с Microsoft Graph Toolkit

Компоненты Microsoft Graph Toolkit можно легко добавить в веб-приложение, веб-часть SharePoint или вкладки Microsoft Teams. Компоненты основаны на веб-стандартах и могут использоваться как в обычных проектах JavaScript, так и в популярных веб-платформах, таких как Reach, Angular и Vue.js.

Просмотрите это короткое видео, чтобы приступить к работе с набором средств.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Пошаговое руководство см. в модуле "Начало [работы с Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) ". 

## <a name="set-up-your-microsoft-365-tenant"></a>Настройка клиента Microsoft 365

Чтобы использовать Microsoft Graph Toolkit для разработки приложения, необходим доступ к клиенту Microsoft 365. Если у вас ее нет, вы можете получить бесплатную подписку разработчика Microsoft 365, присоединившись к [программе для разработчиков Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program). Дополнительные сведения о настройке подписки см. в разделе ["Настройка подписки разработчика Microsoft 365"](/office/developer-program/microsoft-365-developer-program-get-started).

## <a name="set-up-your-development-environment"></a>Настройка среды разработки

Для разработки с помощью набора средств вам потребуется следующее:

- Текстовый редактор или интегрированная среда разработки. Вы можете использовать редактор или интегрированную среду разработки по вашему выбору или установить и [использовать](https://code.visualstudio.com/download) Visual Studio Code бесплатно.
- Современный веб-браузер, например Microsoft Edge, Google Chrome или Firefox.
- Версия LTS Node.js, которую можно установить из [nodejs.org](https://nodejs.org).

## <a name="use-microsoft-graph-toolkit"></a>Использование Microsoft Graph Toolkit

Microsoft Graph Toolkit можно использовать в приложении, ссылаясь на загрузчик напрямую (через `unpkg`) или устанавливая `npm` пакет.

# <a name="unpkg"></a>[unpkg](#tab/html)
Чтобы использовать набор средств с помощью `mgt-loader`, добавьте ссылку в скрипте в код:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
Использование набора средств с помощью модулей ES6 дает полный контроль над процессом объединения и позволяет объединить только код, необходимый для приложения. Чтобы использовать модули ES6, добавьте пакет `npm` в проект:

```cmd
npm install @microsoft/mgt
```
Теперь вы можете ссылаться на все компоненты на странице, которую вы используете:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


### <a name="npm-packages"></a>Пакеты NPM

Microsoft Graph Toolkit состоит из нескольких пакетов NPM, что позволяет включать только код, необходимый для приложений.

<b>@microsoft/mgt-element</b>

Это `@microsoft/mgt-element` основной пакет, содержащий только базовые классы, используемые для создания компонентов и поставщиков. Этот пакет предоставляет все необходимые классы и интерфейсы, необходимые для создания собственных компонентов, и экспортирует интерфейс [IProvider и класс SimpleProvider](../providers/custom.md) для создания пользовательских поставщиков.

<b>@microsoft/mgt-components</b>

Пакет `@microsoft/mgt-components` содержит все веб-компоненты, подключенные к Microsoft Graph, `Person`такие как , и `PeoplePicker`т. д. 

**Поставщики**

Поставщики доступны через один пакет и могут быть установлены по мере необходимости. Доступны следующие пакеты поставщиков:

- <b>@microsoft/mgt-msal-provider</b>

    <code>[@microsoft/mgt-msal-provider](../providers/msal.md)</code> содержит компонент `MsalProvider` и компонент `mgt-msal-provider` . Поставщик MSAL использует msal.js для проверки подлинности в веб-приложениях и прогрессивных веб-приложения (PWA).

- <b>@microsoft/mgt-msal2-provider</b>

    <code>[@microsoft/mgt-msal2-provider](../providers/msal2.md)</code> содержит компонент `Msal2Provider` и компонент `mgt-msal2-provider` . Поставщик MSAL2 использует msal-browser для проверки подлинности в веб-приложениях и PWA.

-  <b>@microsoft/mgt-teams-provider</b>

    <code>[@microsoft/mgt-teams-provider](../providers/teams.md)</code> содержит компонент `TeamsProvider` и компонент `mgt-teams-provider` . Поставщик Microsoft Teams включает проверку подлинности в приложении на вкладке Microsoft Teams.

-  <b>@microsoft/mgt-teams-msal2-provider</b>

    <code>[@microsoft/mgt-teams-msal2-provider](../providers/teams.md)</code> содержит компонент `TeamsMsal2Provider` и компонент `mgt-teams-msal2-provider` . Поставщик Microsoft Teams MSAL2 включает проверку подлинности в приложении на вкладке Microsoft Teams.

- <b>@microsoft/mgt-sharepoint-provider</b>

    <code>[@microsoft/mgt-sharepoint-provider](../providers/sharepoint.md)</code> содержит объект `SharePointProvider` для проверки подлинности в среде SharePoint. 

- <b>@microsoft/mgt-proxy-provider</b>

    <code>[@microsoft/mgt-proxy-provider](../providers/proxy.md)</code> содержит приложение `ProxyProvider` , которое прокси-сервер Graph вызывает через серверную службу. 

<b>@microsoft/mgt</b>

Пакет `@microsoft/mgt` является основным пакетом, который включает все предыдущие пакеты и повторно экспортирует их, чтобы они были доступны через один пакет, который можно установить. 

<b>@microsoft/mgt-react</b>

Пакет <code>[@microsoft/mgt-react](./mgt-react.md)</code> содержит все автоматически созданные компоненты React и принимает зависимость от `@microsoft/mgt` пакета.

<b>@microsoft/mgt-spfx</b>

Пакет <code>[@microsoft/mgt-spfx](./mgt-spfx.md)</code> содержит библиотеку SharePoint Framework, которая необходима для использования Microsoft Graph Toolkit в SharePoint Framework решениях.

## <a name="next-steps"></a>Дальнейшие действия

Теперь вы готовы приступить к разработке с помощью Microsoft Graph Toolkit! Ниже приведены руководства, которые помогут вам приступить к работе.

- [Регистрация приложения Azure Active Directory (Azure AD)](./add-aad-app-registration.md)
- [Создание веб-приложения (JavaScript)](./build-a-web-app.md) (javaScript)
- [Создание веб-приложения (React)](./use-toolkit-with-react.md)
- [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md)
- [Создание веб-части SharePoint](./build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Создание вкладки единого входа в Microsoft Teams](./build-a-microsoft-teams-sso-tab.md)
- [Создание приложения Electron](./build-an-electron-app.md)
