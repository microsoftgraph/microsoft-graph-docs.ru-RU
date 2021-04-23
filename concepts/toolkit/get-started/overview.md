---
title: Начало работы с microsoft Graph набор средств
description: Начало работы с помощью microsoft Graph набор средств в приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 3197542066d92978bf151d61a378e7f392633016
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961424"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Начало работы с microsoft Graph набор средств

Компоненты Microsoft Graph набор средств легко добавляться в веб-приложение, веб-часть SharePoint или вкладки Microsoft Teams. Компоненты основаны на веб-стандартах и могут использоваться как в обычных проектах JavaScript, так и в популярных веб-инфраструктурах, таких как Reach, Angular, Vue.js и других.

Вы можете просмотреть это короткое видео, чтобы узнать, как быстро и легко начать работу с набор средств.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Пошаговая инструкция см. в руководстве Начать работу с [модулем Microsot Graph набор средств.](/learn/modules/msgraph-toolkit-intro/) 

## <a name="set-up-your-microsoft-365-tenant"></a>Настройка клиента Microsoft 365
Для разработки с помощью набор средств необходимо получить доступ к клиенту Microsoft 365. Если у вас его нет, вы можете получить бесплатную подписку на разработчика Microsoft 365, присоединившись к [программе разработчиков Microsoft 365.](https://developer.microsoft.com/microsoft-365/dev-program) Сведения о настройке подписки см. в материале [Настройка подписки на разработчика Microsoft 365.](/office/developer-program/microsoft-365-developer-program-get-started)

## <a name="set-up-your-development-environment"></a>Настройка среды разработки
Для разработки с набор средств потребуется текстовый редактор или IDE. Вы можете использовать редактор или IDE по вашему выбору или установить [и использовать Visual Studio код](https://code.visualstudio.com/download) бесплатно. Вам также понадобится современный веб-браузер, например Microsoft Edge, Google Chrome или Firefox. Вам также понадобится версия LTS Node.js, которую можно установить с [nodejs.org](https://nodejs.org).

## <a name="using-the-microsoft-graph-toolkit"></a>Использование microsoft Graph набор средств
Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Чтобы использовать Toolkit в загрузчике Microsoft Graph Toolkit, добавьте ссылку в сценарий кода:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
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

Программа Microsoft Graph набор средств состоит из нескольких пакетов NPM, что позволяет включать только код, необходимый для приложений.

<b>@microsoft/mgt-element</b>

Основной пакет содержит только базовые классы, используемые для создания `@microsoft/mgt-element` компонентов и поставщиков. Этот пакет предоставляет все необходимые классы и интерфейсы, необходимые для создания собственных компонентов, и экспортирует [интерфейс IProvider и класс SimpleProvider](../providers/custom.md) для создания настраиваемого поставщика.

<b>@microsoft/mgt-components</b>

Пакет `@microsoft/mgt-components` содержит все подключенные веб-компоненты Microsoft Graph, такие как `Person` , и `PeoplePicker` более. 

**Поставщики**

Поставщики доступны через один пакет и могут быть установлены по мере необходимости. Доступны следующие пакеты поставщиков:

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) содержит `MsalProvider` и `mgt-msal-provider` компонент. Поставщик msal использует msal.js для проверки подлинности в веб-приложениях и PWAs.

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) содержит `TeamsProvider` и `mgt-teams-provider` компонент. Поставщик Microsoft Teams включает проверку подлинности в приложении вкладки Microsoft Teams.

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) содержит `SharePointProvider` для проверки подлинности в среде SharePoint. 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md) содержит `ProxyProvider` приложение, которое прокси-граф вызывает через службу backend. 

<b>@microsoft/mgt</b>

Это основной пакет, который включает все вышеперечисленные пакеты и повторно экспортирует их, чтобы они были доступны с помощью одного `@microsoft/mgt` пакета, который можно установить. 

<b>@microsoft/mgt-react</b>

Пакет [`@microsoft/mgt-react`](./mgt-react.md) содержит все автоматически созданные компоненты React и принимает зависимость от `@microsoft/mgt` пакета.

## <a name="polyfills"></a>Полизаполнение

Если вы используете модули ES6 из пакета npm и нацеливались на такой браузер, как [IE11,](https://caniuse.com/#search=components) который не поддерживает веб-компоненты, необходимо включить полифилы в проект, так как они не включаются автоматически. Полифильмы помогают заполнить недостающие возможности браузера в браузерах, которые еще находятся в процессе обновления для поддержки стандартов веб-компонентов. Дополнительные инструкции см. в документации [по полифилям.](https://www.webcomponents.org/polyfills) 

Полифильмы уже включены, если вы используете набор средств с помощью скрипта mgt-loader.

## <a name="next-steps"></a>Дальнейшие действия
Теперь вы готовы начать разработку с помощью microsoft Graph набор средств! Для начала работы доступны следующие руководства:

- [Регистрация приложения Azure Active Directory](./add-aad-app-registration.md)
- [Создание веб-приложения (JavaScript)](./build-a-web-app.md) (ванильный JavaScript)
- [Создание веб-приложения (React)](./use-toolkit-with-react.md)
- [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md)
- [Создание веб-части SharePoint](./build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
