---
title: Начало работы с microsoft Graph набор средств
description: Начало работы с помощью microsoft Graph набор средств в приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e84350a7835cac7914f5238110f74b3383047e13
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579594"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="a7419-103">Начало работы с microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="a7419-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a7419-104">Компоненты microsoft Graph набор средств легко можно добавить в ваше веб-приложение, SharePoint веб-часть или Microsoft Teams вкладки.</span><span class="sxs-lookup"><span data-stu-id="a7419-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="a7419-105">Компоненты основаны на веб-стандартах и могут использоваться как в обычных проектах JavaScript, так и в популярных веб-инфраструктурах, таких как Reach, Angular, Vue.js и других.</span><span class="sxs-lookup"><span data-stu-id="a7419-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="a7419-106">Вы можете просмотреть это короткое видео, чтобы узнать, как быстро и легко начать работу с набор средств.</span><span class="sxs-lookup"><span data-stu-id="a7419-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="a7419-107">Пошаговую инструкцию см. в руководстве [Get started with Microsoft Graph набор средств.](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="a7419-107">For a step-by-step tutorial, see the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> 

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="a7419-108">Настройка клиента Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a7419-108">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="a7419-109">Чтобы развиваться с помощью набор средств, вам необходим доступ к Microsoft 365 клиента.</span><span class="sxs-lookup"><span data-stu-id="a7419-109">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="a7419-110">Если у вас его нет, вы можете получить бесплатную подписку Microsoft 365 разработчика, присоединившись [к программе Microsoft 365 разработчика](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="a7419-110">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="a7419-111">Сведения о настройке подписки см. в материале [Настройка подписки Microsoft 365 разработчика.](/office/developer-program/microsoft-365-developer-program-get-started)</span><span class="sxs-lookup"><span data-stu-id="a7419-111">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="a7419-112">Настройка среды разработки</span><span class="sxs-lookup"><span data-stu-id="a7419-112">Set up your development environment</span></span>
<span data-ttu-id="a7419-113">Для разработки набор средств текстового редактора или IDE.</span><span class="sxs-lookup"><span data-stu-id="a7419-113">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="a7419-114">Вы можете использовать редактор или IDE по вашему выбору или установить и [использовать Visual Studio Code](https://code.visualstudio.com/download) бесплатно.</span><span class="sxs-lookup"><span data-stu-id="a7419-114">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="a7419-115">Вам также понадобится современный веб-браузер, Microsoft Edge, Google Chrome или Firefox.</span><span class="sxs-lookup"><span data-stu-id="a7419-115">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="a7419-116">Вам также понадобится версия LTS Node.js, которую можно установить с [nodejs.org](https://nodejs.org).</span><span class="sxs-lookup"><span data-stu-id="a7419-116">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="a7419-117">Использование microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="a7419-117">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="a7419-118">Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.</span><span class="sxs-lookup"><span data-stu-id="a7419-118">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="a7419-119">unpkg</span><span class="sxs-lookup"><span data-stu-id="a7419-119">unpkg</span></span>](#tab/html)
<span data-ttu-id="a7419-120">Чтобы использовать Toolkit в загрузчике Microsoft Graph Toolkit, добавьте ссылку в сценарий кода:</span><span class="sxs-lookup"><span data-stu-id="a7419-120">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="a7419-121">npm</span><span class="sxs-lookup"><span data-stu-id="a7419-121">npm</span></span>](#tab/npm)
<span data-ttu-id="a7419-122">Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения.</span><span class="sxs-lookup"><span data-stu-id="a7419-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="a7419-123">Чтобы использовать модули ES6, добавьте в проект пакет npm:</span><span class="sxs-lookup"><span data-stu-id="a7419-123">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="a7419-124">Теперь вы можете ссылаться на все компоненты страницы, которые вы используете:</span><span class="sxs-lookup"><span data-stu-id="a7419-124">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="a7419-125">Пакеты NPM</span><span class="sxs-lookup"><span data-stu-id="a7419-125">NPM packages</span></span>

<span data-ttu-id="a7419-126">Microsoft Graph набор средств состоит из нескольких пакетов NPM, что позволяет включать только код, необходимый для приложений.</span><span class="sxs-lookup"><span data-stu-id="a7419-126">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="a7419-127"><b>@microsoft/mgt-element</b></span><span class="sxs-lookup"><span data-stu-id="a7419-127"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="a7419-128">Основной пакет содержит только базовые классы, используемые для создания `@microsoft/mgt-element` компонентов и поставщиков.</span><span class="sxs-lookup"><span data-stu-id="a7419-128">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="a7419-129">Этот пакет предоставляет все необходимые классы и интерфейсы, необходимые для создания собственных компонентов, и экспортирует [интерфейс IProvider и класс SimpleProvider](../providers/custom.md) для создания настраиваемого поставщика.</span><span class="sxs-lookup"><span data-stu-id="a7419-129">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="a7419-130"><b>@microsoft/mgt-components</b></span><span class="sxs-lookup"><span data-stu-id="a7419-130"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="a7419-131">Пакет содержит все подключенные Graph Майкрософт `@microsoft/mgt-components` веб-компоненты, такие как , и `Person` `PeoplePicker` более.</span><span class="sxs-lookup"><span data-stu-id="a7419-131">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="a7419-132">**Поставщики**</span><span class="sxs-lookup"><span data-stu-id="a7419-132">**Providers**</span></span>

<span data-ttu-id="a7419-133">Поставщики доступны через один пакет и могут быть установлены по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="a7419-133">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="a7419-134">Доступны следующие пакеты поставщиков:</span><span class="sxs-lookup"><span data-stu-id="a7419-134">The following provider packages are available:</span></span>

- <span data-ttu-id="a7419-135"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="a7419-135"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="a7419-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) содержит `MsalProvider` и `mgt-msal-provider` компонент.</span><span class="sxs-lookup"><span data-stu-id="a7419-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="a7419-137">Поставщик MSAL использует msal.js для проверки подлинности в веб-приложениях и прогрессивных веб-приложениях (PWAs).</span><span class="sxs-lookup"><span data-stu-id="a7419-137">The MSAL provider uses msal.js for authenticating in web apps and Progressive Web Apps (PWAs).</span></span>

- <span data-ttu-id="a7419-138"><b>@micosoft/mgt-msal2-provider</b></span><span class="sxs-lookup"><span data-stu-id="a7419-138"><b>@micosoft/mgt-msal2-provider</b></span></span>

    <span data-ttu-id="a7419-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) содержит `Msal2Provider` и `mgt-msal2-provider` компонент.</span><span class="sxs-lookup"><span data-stu-id="a7419-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contains the `Msal2Provider` and `mgt-msal2-provider` component.</span></span> <span data-ttu-id="a7419-140">Поставщик MSAL использует msal-browser для проверки подлинности в веб-приложениях и PWAs.</span><span class="sxs-lookup"><span data-stu-id="a7419-140">The MSAL provider uses msal-browser for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="a7419-141"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="a7419-141"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="a7419-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) содержит `TeamsProvider` и `mgt-teams-provider` компонент.</span><span class="sxs-lookup"><span data-stu-id="a7419-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="a7419-143">Поставщик Microsoft Teams включает проверку подлинности в Microsoft Teams вкладке.</span><span class="sxs-lookup"><span data-stu-id="a7419-143">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="a7419-144"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="a7419-144"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="a7419-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)содержит `SharePointProvider` для проверки подлинности в SharePoint среде.</span><span class="sxs-lookup"><span data-stu-id="a7419-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="a7419-146"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="a7419-146"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="a7419-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md)содержит `ProxyProvider` приложение, которое Graph через службу backend.</span><span class="sxs-lookup"><span data-stu-id="a7419-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="a7419-148"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="a7419-148"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="a7419-149">Это основной пакет, который включает все вышеперечисленные пакеты и повторно экспортирует их, чтобы они были доступны с помощью одного `@microsoft/mgt` пакета, который можно установить.</span><span class="sxs-lookup"><span data-stu-id="a7419-149">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="a7419-150"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="a7419-150"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="a7419-151">Пакет содержит все автоматически созданные [`@microsoft/mgt-react`](./mgt-react.md) React и принимает зависимость от `@microsoft/mgt` пакета.</span><span class="sxs-lookup"><span data-stu-id="a7419-151">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

<span data-ttu-id="a7419-152"><b>@microsoft/mgt-spfx</b></span><span class="sxs-lookup"><span data-stu-id="a7419-152"><b>@microsoft/mgt-spfx</b></span></span>

<span data-ttu-id="a7419-153">Пакет содержит библиотеку SharePoint Framework, которая необходима для использования [`@microsoft/mgt-spfx`](./mgt-spfx.md) Microsoft Graph набор средств в SharePoint Framework решениях.</span><span class="sxs-lookup"><span data-stu-id="a7419-153">The [`@microsoft/mgt-spfx`](./mgt-spfx.md) package contains a SharePoint Framework library that's required to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

## <a name="polyfills"></a><span data-ttu-id="a7419-154">Полизаполнение</span><span class="sxs-lookup"><span data-stu-id="a7419-154">Polyfills</span></span>

<span data-ttu-id="a7419-155">Если вы используете модули ES6 из пакета npm и нацеливались на такой браузер, как [IE11,](https://caniuse.com/#search=components) который не поддерживает веб-компоненты, необходимо включить полифилы в проект, так как они не включаются автоматически.</span><span class="sxs-lookup"><span data-stu-id="a7419-155">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="a7419-156">Полифильмы помогают заполнить недостающие возможности браузера в браузерах, которые еще находятся в процессе обновления для поддержки стандартов веб-компонентов.</span><span class="sxs-lookup"><span data-stu-id="a7419-156">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support Web Component standards.</span></span> <span data-ttu-id="a7419-157">Дополнительные инструкции см. в документации [по полифилям.](https://www.webcomponents.org/polyfills)</span><span class="sxs-lookup"><span data-stu-id="a7419-157">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="a7419-158">Полифильмы уже включены, если вы используете набор средств с помощью скрипта mgt-loader.</span><span class="sxs-lookup"><span data-stu-id="a7419-158">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a7419-159">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="a7419-159">Next Steps</span></span>
<span data-ttu-id="a7419-160">Теперь вы готовы начать разработку с помощью microsoft Graph набор средств!</span><span class="sxs-lookup"><span data-stu-id="a7419-160">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="a7419-161">Для начала работы доступны следующие руководства:</span><span class="sxs-lookup"><span data-stu-id="a7419-161">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="a7419-162">Регистрация приложения Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a7419-162">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="a7419-163">[Создание веб-приложения (JavaScript)](./build-a-web-app.md) (ванильный JavaScript)</span><span class="sxs-lookup"><span data-stu-id="a7419-163">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="a7419-164">Создание веб-приложения (React)</span><span class="sxs-lookup"><span data-stu-id="a7419-164">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="a7419-165">Создание веб-приложения (Angular)</span><span class="sxs-lookup"><span data-stu-id="a7419-165">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="a7419-166">Создание веб-части SharePoint</span><span class="sxs-lookup"><span data-stu-id="a7419-166">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="a7419-167">Создание вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a7419-167">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
