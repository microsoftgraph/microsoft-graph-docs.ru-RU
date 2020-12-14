---
title: 'Microsoft Graph набор средств: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph'
description: Microsoft Graph набор средств — это коллекция поставщиков проверки подлинности и веб-компонентов, которые могут повторно работать, не зависит от структуры, для доступа к Microsoft Graph и работы с ним.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: d2ed14c5862cbd081b7592a180cd15e2bfdb2548
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659277"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a><span data-ttu-id="b0bf1-103">Microsoft Graph набор средств: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b0bf1-103">Microsoft Graph Toolkit: UI Components and Authentication Providers for Microsoft Graph</span></span> 

<span data-ttu-id="b0bf1-104">Microsoft Graph набор средств — это коллекция повторно работающих, не зависит от структуры компонентов и поставщиков проверки подлинности для доступа к Microsoft Graph и работы с ним.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic components and authentication providers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="b0bf1-105">Компоненты полностью готовы к функциональности со встроенными поставщиками, которые аутентификация и извлечение данных из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="b0bf1-106">Microsoft Graph набор средств упрощает использование Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="b0bf1-107">В следующем примере во время входа пользователя и его событий календаря отображаются только [](./components/agenda.md) две строки кода с помощью компонентов [входа](./components/login.md) и повестки дня.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-107">In the following example, a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="b0bf1-108">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="b0bf1-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="b0bf1-109">Что в microsoft Graph набор средств?</span><span class="sxs-lookup"><span data-stu-id="b0bf1-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="b0bf1-110">Компоненты</span><span class="sxs-lookup"><span data-stu-id="b0bf1-110">Components</span></span>

<span data-ttu-id="b0bf1-111">Microsoft Graph набор средств содержит коллекцию веб-компонентов для наиболее распространенных встроенных API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span> 

<span data-ttu-id="b0bf1-112">Эти компоненты также доступны в качестве [компонентов React.](./get-started/mgt-react.md)</span><span class="sxs-lookup"><span data-stu-id="b0bf1-112">The components are also available as [React components](./get-started/mgt-react.md).</span></span>

|<span data-ttu-id="b0bf1-113">Компонент</span><span class="sxs-lookup"><span data-stu-id="b0bf1-113">Component</span></span>|<span data-ttu-id="b0bf1-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b0bf1-114">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="b0bf1-115">Вход</span><span class="sxs-lookup"><span data-stu-id="b0bf1-115">Login</span></span>](./components/login.md)|<span data-ttu-id="b0bf1-116">Кнопка и flyout для проверки подлинности пользователя с помощью платформы удостоверений Майкрософт и отображения сведений профиля пользователя при входе.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-116">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="b0bf1-117">Пользователь</span><span class="sxs-lookup"><span data-stu-id="b0bf1-117">Person</span></span>](./components/person.md)|<span data-ttu-id="b0bf1-118">Отображает человека или контакт по его фотографии, имени и/или адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-118">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="b0bf1-119">Люди</span><span class="sxs-lookup"><span data-stu-id="b0bf1-119">People</span></span>](./components/people.md)|<span data-ttu-id="b0bf1-120">Отображает группу людей или контактов по их фотографиям или инициалам.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-120">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="b0bf1-121">Повестка</span><span class="sxs-lookup"><span data-stu-id="b0bf1-121">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="b0bf1-122">Отображает события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-122">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="b0bf1-123">Задачи</span><span class="sxs-lookup"><span data-stu-id="b0bf1-123">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="b0bf1-124">Отображает и позволяет добавлять, удалять, завершать или редактировать задачи из Планировщика (Майкрософт) или Microsoft To Do (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="b0bf1-124">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To Do.</span></span>|
|[<span data-ttu-id="b0bf1-125">Выбор людей</span><span class="sxs-lookup"><span data-stu-id="b0bf1-125">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="b0bf1-126">Предоставляет возможность поиска людей и отображения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-126">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="b0bf1-127">Карточка человека</span><span class="sxs-lookup"><span data-stu-id="b0bf1-127">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="b0bf1-128">Flyout used on the person component to display more profile information about a user.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-128">A flyout used on the person component to display more profile information about a user.</span></span>|
|<span data-ttu-id="b0bf1-129">[получение](./components/get.md);</span><span class="sxs-lookup"><span data-stu-id="b0bf1-129">[Get](./components/get.md)</span></span>|<span data-ttu-id="b0bf1-130">Сделайте запрос GET к любому API Microsoft Graph непосредственно в HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-130">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="b0bf1-131">Выбор канала</span><span class="sxs-lookup"><span data-stu-id="b0bf1-131">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="b0bf1-132">Предоставляет возможность поиска каналов Microsoft Teams для выбора канала из отрисовки списка результатов.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-132">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|
|[<span data-ttu-id="b0bf1-133">To Do</span><span class="sxs-lookup"><span data-stu-id="b0bf1-133">To Do</span></span>](./components/todo.md)|<span data-ttu-id="b0bf1-134">Отображает и позволяет добавлять, удалять, завершать или редактировать задачи из Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-134">Displays and enables adding, removing, completing, or editing of tasks from Microsoft To Do.</span></span>|

### <a name="providers"></a><span data-ttu-id="b0bf1-135">Поставщики</span><span class="sxs-lookup"><span data-stu-id="b0bf1-135">Providers</span></span>

<span data-ttu-id="b0bf1-136">[Поставщики](/providers/providers.md) обеспечивают проверку подлинности и обеспечивают реализацию для получения маркеров доступа на различных платформах и предоставления клиента Microsoft Graph для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-136">[Providers](/providers/providers.md) enable authentication and provide the implementation for acquiring access tokens on various platforms and expose a Microsoft Graph client for calling the Microsoft Graph APIs.</span></span> <span data-ttu-id="b0bf1-137">Компоненты лучше всего работают при работе с поставщиком, но их можно использовать самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-137">The components work best when used with a provider, but the providers can be used on their own.</span></span>

|<span data-ttu-id="b0bf1-138">Поставщики</span><span class="sxs-lookup"><span data-stu-id="b0bf1-138">Providers</span></span>|<span data-ttu-id="b0bf1-139">Описание</span><span class="sxs-lookup"><span data-stu-id="b0bf1-139">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="b0bf1-140">Msal</span><span class="sxs-lookup"><span data-stu-id="b0bf1-140">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="b0bf1-141">Использует MSAL.js для входов пользователей и получения маркеров для использования с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-141">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="b0bf1-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="b0bf1-142">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="b0bf1-143">Проверка подлинности и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-143">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="b0bf1-144">Teams</span><span class="sxs-lookup"><span data-stu-id="b0bf1-144">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="b0bf1-145">Проверка подлинности и предоставляет Microsoft Graph доступ к компонентам на вкладке Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-145">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="b0bf1-146">Прокси-сервер</span><span class="sxs-lookup"><span data-stu-id="b0bf1-146">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="b0bf1-147">Позволяет использовать проверку подлинности на тыловом компьютере путем маршрутизации всех вызовов в Microsoft Graph через ваш тыл.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-147">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="b0bf1-148">Custom</span><span class="sxs-lookup"><span data-stu-id="b0bf1-148">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="b0bf1-149">Создайте настраиваемого поставщика, чтобы включить проверку подлинности и доступ к Microsoft Graph с помощью существующего кода проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-149">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="b0bf1-150">Зачем использовать microsoft Graph набор средств?</span><span class="sxs-lookup"><span data-stu-id="b0bf1-150">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="b0bf1-151">Microsoft Graph набор средств позволяет быстро и просто интегрировать распространенные опытом, встроенные в Microsoft Graph, в собственное приложение.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-151">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="b0bf1-152">**Сокращение времени разработки**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-152">**Cut Development Time**</span></span>

    <span data-ttu-id="b0bf1-153">Работа по подключению к API Microsoft Graph и отрисовка данных в пользовательском интерфейсе, который выглядит как Microsoft365, сделана для вас без необходимости настройки.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-153">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="b0bf1-154">**Работает везде**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-154">**Works Everywhere**</span></span>

    <span data-ttu-id="b0bf1-155">Все компоненты основаны на веб-стандартах и легко работают с любым современным браузером и веб-структурой (React, Angular, Vue и т. д.).</span><span class="sxs-lookup"><span data-stu-id="b0bf1-155">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="b0bf1-156">**Красивый, но гибкий**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-156">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="b0bf1-157">Эти компоненты предназначены для работы с Microsoft 365, но также настраиваются с помощью настраиваемых свойств [CSS](./customize-components/style.md) и [шаблонов.](./customize-components/templates.md)</span><span class="sxs-lookup"><span data-stu-id="b0bf1-157">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./customize-components/style.md) and [templating](./customize-components/templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="b0bf1-158">Кто должен использовать его?</span><span class="sxs-lookup"><span data-stu-id="b0bf1-158">Who should use it?</span></span>

<span data-ttu-id="b0bf1-159">Microsoft Graph набор средств отлично подходит для разработчиков всех уровней работы, которые ищут разработку веб-приложения, вкладки Microsoft Teams или веб-части SharePoint, которая подключается к данным из Microsoft Graph и имеет к ним доступ.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-159">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop a web application, Microsoft Teams tab, or SharePoint web part that connects to and accesses data from Microsoft Graph.</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="b0bf1-160">Где его можно использовать?</span><span class="sxs-lookup"><span data-stu-id="b0bf1-160">Where can I use it?</span></span>

<span data-ttu-id="b0bf1-161">Microsoft Graph набор средств в следующих браузерах.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-161">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Интернет-подключение к Интернету](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="b0bf1-168">**Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-168">**Edge**</span></span>|<span data-ttu-id="b0bf1-169">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-169">**Firefox**</span></span>|<span data-ttu-id="b0bf1-170">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-170">**Chrome**</span></span>|<span data-ttu-id="b0bf1-171">**Safari**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-171">**Safari**</span></span>|<span data-ttu-id="b0bf1-172">**Opera**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-172">**Opera**</span></span>|<span data-ttu-id="b0bf1-173">**Сума**</span><span class="sxs-lookup"><span data-stu-id="b0bf1-173">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="b0bf1-174">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b0bf1-174">Next steps</span></span>

- <span data-ttu-id="b0bf1-175">Попробуйте компоненты в игровой [области.](https://mgt.dev)</span><span class="sxs-lookup"><span data-stu-id="b0bf1-175">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="b0bf1-176">[Начало работы](./get-started/overview.md) с microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="b0bf1-176">[Get started](./get-started/overview.md) with the Microsoft Graph Toolkit.</span></span>
- <span data-ttu-id="b0bf1-177">Ознакомьтесь с набор средств Microsoft Graph на [сайте GitHub.](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="b0bf1-177">Check out the Microsoft Graph Toolkit on [GitHub](https://aka.ms/mgt).</span></span>
