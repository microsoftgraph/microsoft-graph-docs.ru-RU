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
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="10b8a-103">Начало работы с microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="10b8a-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="10b8a-104">Компоненты набор средств Microsoft Graph можно легко добавить в веб-приложение, веб-часть SharePoint или на вкладки Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="10b8a-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="10b8a-105">Эти компоненты основаны на веб-стандартах и могут использоваться как в обычных проектах JavaScript, так и в популярных веб-платформах, таких как Reach, Angular, Vue.js и других.</span><span class="sxs-lookup"><span data-stu-id="10b8a-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="10b8a-106">Вы можете посмотреть это короткое видео, чтобы узнать, как быстро и просто начать работу с набор средств.</span><span class="sxs-lookup"><span data-stu-id="10b8a-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="10b8a-107">Настройка клиента Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="10b8a-107">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="10b8a-108">Для разработки с помощью набор средств вам нужен доступ к клиенту Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="10b8a-108">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="10b8a-109">Если у вас ее нет, вы можете получить бесплатную подписку разработчика Microsoft 365, присоединившись к программе для [разработчиков Microsoft 365.](https://developer.microsoft.com/microsoft-365/dev-program)</span><span class="sxs-lookup"><span data-stu-id="10b8a-109">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="10b8a-110">Подробные сведения о настройке подписки см. в сведениях о настройке подписки разработчика [Microsoft 365.](/office/developer-program/microsoft-365-developer-program-get-started)</span><span class="sxs-lookup"><span data-stu-id="10b8a-110">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="10b8a-111">Настройка среды разработки</span><span class="sxs-lookup"><span data-stu-id="10b8a-111">Set up your development environment</span></span>
<span data-ttu-id="10b8a-112">Для разработки с набор средств потребуется текстовый редактор или IDE.</span><span class="sxs-lookup"><span data-stu-id="10b8a-112">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="10b8a-113">Вы можете использовать редактор или IDE по вашему выбору или установить и [использовать Visual Studio Code](https://code.visualstudio.com/download) бесплатно.</span><span class="sxs-lookup"><span data-stu-id="10b8a-113">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="10b8a-114">Вам также потребуется современный веб-браузер, например Microsoft Edge, Google Chrome или Firefox.</span><span class="sxs-lookup"><span data-stu-id="10b8a-114">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="10b8a-115">Вам также потребуется версия LTS Node.js, которую можно установить из [nodejs.org.](https://nodejs.org)</span><span class="sxs-lookup"><span data-stu-id="10b8a-115">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="10b8a-116">Использование microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="10b8a-116">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="10b8a-117">Вы можете использовать microsoft Graph набор средств в приложении, ссылаясь на загрузчик напрямую (с помощью unpkg) или установив пакет npm.</span><span class="sxs-lookup"><span data-stu-id="10b8a-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="10b8a-118">unpkg</span><span class="sxs-lookup"><span data-stu-id="10b8a-118">unpkg</span></span>](#tab/html)
<span data-ttu-id="10b8a-119">Чтобы использовать набор средств mgt-loader, добавьте ссылку в сценарии в код:</span><span class="sxs-lookup"><span data-stu-id="10b8a-119">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="10b8a-120">npm</span><span class="sxs-lookup"><span data-stu-id="10b8a-120">npm</span></span>](#tab/npm)
<span data-ttu-id="10b8a-121">Использование набор средств с помощью модулей ES6 дает полный контроль над процессом пакетизации и позволяет объединить только код, необходимый для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="10b8a-121">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="10b8a-122">Чтобы использовать модули ES6, добавьте пакет npm в проект:</span><span class="sxs-lookup"><span data-stu-id="10b8a-122">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="10b8a-123">Теперь вы можете ссылаться на все компоненты страницы, которые вы используете:</span><span class="sxs-lookup"><span data-stu-id="10b8a-123">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="10b8a-124">Пакеты NPM</span><span class="sxs-lookup"><span data-stu-id="10b8a-124">NPM packages</span></span>

<span data-ttu-id="10b8a-125">Microsoft Graph набор средств состоит из нескольких пакетов NPM, что позволяет включать только код, необходимый для ваших приложений.</span><span class="sxs-lookup"><span data-stu-id="10b8a-125">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="10b8a-126"><b>@microsoft/mgt-element</b></span><span class="sxs-lookup"><span data-stu-id="10b8a-126"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="10b8a-127">Основной пакет содержит только базовые классы, используемые для создания `@microsoft/mgt-element` компонентов и поставщиков.</span><span class="sxs-lookup"><span data-stu-id="10b8a-127">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="10b8a-128">Этот пакет предоставляет все необходимые классы и интерфейсы, необходимые для создания собственных компонентов, и экспортирует [интерфейс IProvider](../providers/custom.md) и класс SimpleProvider для создания пользовательских поставщиков.</span><span class="sxs-lookup"><span data-stu-id="10b8a-128">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="10b8a-129"><b>@microsoft/mgt-components</b></span><span class="sxs-lookup"><span data-stu-id="10b8a-129"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="10b8a-130">Пакет `@microsoft/mgt-components` содержит все веб-компоненты, подключенные к Microsoft Graph, такие как `Person` , и `PeoplePicker` другие.</span><span class="sxs-lookup"><span data-stu-id="10b8a-130">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="10b8a-131">**Поставщики**</span><span class="sxs-lookup"><span data-stu-id="10b8a-131">**Providers**</span></span>

<span data-ttu-id="10b8a-132">Поставщики доступны через один пакет и могут быть установлены по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="10b8a-132">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="10b8a-133">Доступны следующие пакеты поставщиков:</span><span class="sxs-lookup"><span data-stu-id="10b8a-133">The following provider packages are available:</span></span>

- <span data-ttu-id="10b8a-134"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="10b8a-134"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="10b8a-135">[`@micosoft/mgt-msal-provider`](../providers/msal.md) содержит и `MsalProvider` `mgt-msal-provider` компонент.</span><span class="sxs-lookup"><span data-stu-id="10b8a-135">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="10b8a-136">Поставщик msal использует msal.js проверки подлинности в веб-приложениях и PWAS.</span><span class="sxs-lookup"><span data-stu-id="10b8a-136">The msal provider leverages msal.js for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="10b8a-137"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="10b8a-137"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="10b8a-138">[`@microsoft/mgt-teams-provider`](../providers/teams.md) содержит и `TeamsProvider` `mgt-teams-provider` компонент.</span><span class="sxs-lookup"><span data-stu-id="10b8a-138">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="10b8a-139">Поставщик Microsoft Teams включает проверку подлинности в приложении вкладок Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="10b8a-139">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="10b8a-140"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="10b8a-140"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="10b8a-141">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) содержит данные `SharePointProvider` для проверки подлинности в среде SharePoint.</span><span class="sxs-lookup"><span data-stu-id="10b8a-141">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="10b8a-142"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="10b8a-142"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="10b8a-143">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) содержит `ProxyProvider` приложение, которое прокси-сервер Graph вызывает через серверную службу.</span><span class="sxs-lookup"><span data-stu-id="10b8a-143">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="10b8a-144"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="10b8a-144"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="10b8a-145">Это основной пакет, который включает все вышеперечисленные пакеты и повторно экспортирует их, чтобы они были доступны через один `@microsoft/mgt` пакет, который можно установить.</span><span class="sxs-lookup"><span data-stu-id="10b8a-145">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="10b8a-146"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="10b8a-146"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="10b8a-147">Пакет содержит все автоматически созданные компоненты React и принимает [`@microsoft/mgt-react`](./mgt-react.md) зависимость от `@microsoft/mgt` пакета.</span><span class="sxs-lookup"><span data-stu-id="10b8a-147">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

## <a name="polyfills"></a><span data-ttu-id="10b8a-148">Polyfills</span><span class="sxs-lookup"><span data-stu-id="10b8a-148">Polyfills</span></span>

<span data-ttu-id="10b8a-149">Если вы используете модули ES6 из пакета npm и используете браузер, такой как [IE11,](https://caniuse.com/#search=components) который не поддерживает веб-компоненты по умолчанию, вам потребуется включить в проект полифайли, так как они не включаются автоматически.</span><span class="sxs-lookup"><span data-stu-id="10b8a-149">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="10b8a-150">Polyfills помогают заполнить отсутствующие возможности браузера в браузерах, которые все еще находятся в процессе обновления для поддержки стандартов веб-компонентов.</span><span class="sxs-lookup"><span data-stu-id="10b8a-150">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support Web Component standards.</span></span> <span data-ttu-id="10b8a-151">Инструкции и дополнительные инструкции см. в документации [по полифайлам.](https://www.webcomponents.org/polyfills)</span><span class="sxs-lookup"><span data-stu-id="10b8a-151">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="10b8a-152">Полизаполнели уже включены, если вы используете набор средств с помощью скрипта mgt-loader.</span><span class="sxs-lookup"><span data-stu-id="10b8a-152">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="10b8a-153">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="10b8a-153">Next Steps</span></span>
<span data-ttu-id="10b8a-154">Теперь вы готовы приступить к разработке с помощью microsoft Graph набор средств!</span><span class="sxs-lookup"><span data-stu-id="10b8a-154">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="10b8a-155">Для начала работы доступны следующие руководства:</span><span class="sxs-lookup"><span data-stu-id="10b8a-155">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="10b8a-156">Регистрация приложения Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="10b8a-156">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="10b8a-157">[Создание веб-приложения (JavaScript)](./build-a-web-app.md) (javaScript)</span><span class="sxs-lookup"><span data-stu-id="10b8a-157">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="10b8a-158">Создание веб-приложения (React)</span><span class="sxs-lookup"><span data-stu-id="10b8a-158">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="10b8a-159">Создание веб-приложения (Angular)</span><span class="sxs-lookup"><span data-stu-id="10b8a-159">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="10b8a-160">Создание веб-части SharePoint</span><span class="sxs-lookup"><span data-stu-id="10b8a-160">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="10b8a-161">Создание вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="10b8a-161">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
