---
title: 'Microsoft Graph Toolkit: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph'
description: Microsoft Graph Toolkit — это коллекция поставщиков проверки подлинности и многократно используемых, не зависящих от платформы веб-компонентов для доступа и работы в Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: d2ed14c5862cbd081b7592a180cd15e2bfdb2548
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659277"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a><span data-ttu-id="d078a-103">Microsoft Graph Toolkit: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d078a-103">Microsoft Graph Toolkit: UI Components and Authentication Providers for Microsoft Graph</span></span> 

<span data-ttu-id="d078a-104">Microsoft Graph Toolkit — это коллекция многократно используемых, не зависящих от платформы компонентов и поставщиков проверки подлинности для доступа и работы в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d078a-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic components and authentication providers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="d078a-105">Готовые компоненты являются полностью функциональными и включают встроенных поставщиков, которые проверяют подлинность и получают данные из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d078a-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="d078a-106">С помощью Microsoft Graph Toolkit можно легко использовать Microsoft Graph в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="d078a-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="d078a-107">В следующем примере вошедший пользователь и события его календаря отображаются всего лишь в двух строках кода с помощью компонентов [Вход](./components/login.md) и [Повестка дня](./components/agenda.md).</span><span class="sxs-lookup"><span data-stu-id="d078a-107">In the following example, a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="d078a-108">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="d078a-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d078a-109">Что включает Microsoft Graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="d078a-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="d078a-110">Компоненты</span><span class="sxs-lookup"><span data-stu-id="d078a-110">Components</span></span>

<span data-ttu-id="d078a-111">Microsoft Graph Toolkit включает коллекцию веб-компонентов для наиболее распространенных встроенных возможностей на базе API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d078a-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span> 

<span data-ttu-id="d078a-112">Они также доступны как [компоненты React](./get-started/mgt-react.md).</span><span class="sxs-lookup"><span data-stu-id="d078a-112">The components are also available as [React components](./get-started/mgt-react.md).</span></span>

|<span data-ttu-id="d078a-113">Компонент</span><span class="sxs-lookup"><span data-stu-id="d078a-113">Component</span></span>|<span data-ttu-id="d078a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d078a-114">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="d078a-115">Вход</span><span class="sxs-lookup"><span data-stu-id="d078a-115">Login</span></span>](./components/login.md)|<span data-ttu-id="d078a-116">Кнопка и элемент управления "Всплывающий элемент" для проверки подлинности пользователя с помощью платформы удостоверений Майкрософт и отображения сведений из профиля пользователя при входе.</span><span class="sxs-lookup"><span data-stu-id="d078a-116">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="d078a-117">Человек</span><span class="sxs-lookup"><span data-stu-id="d078a-117">Person</span></span>](./components/person.md)|<span data-ttu-id="d078a-118">Отображает пользователя или контакт с помощью его фотографии, имени и/или адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d078a-118">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="d078a-119">Люди</span><span class="sxs-lookup"><span data-stu-id="d078a-119">People</span></span>](./components/people.md)|<span data-ttu-id="d078a-120">Отображает группу людей или контактов с помощью их фотографий или инициалов.</span><span class="sxs-lookup"><span data-stu-id="d078a-120">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="d078a-121">Повестка дня</span><span class="sxs-lookup"><span data-stu-id="d078a-121">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="d078a-122">Отображает события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="d078a-122">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="d078a-123">Задачи</span><span class="sxs-lookup"><span data-stu-id="d078a-123">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="d078a-124">Отображает и включает добавление, удаление, выполнение или редактирование задач из Планировщика (Майкрософт) или Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="d078a-124">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To Do.</span></span>|
|[<span data-ttu-id="d078a-125">Выбор людей</span><span class="sxs-lookup"><span data-stu-id="d078a-125">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="d078a-126">Предоставляет возможность поиска людей и отображает список результатов.</span><span class="sxs-lookup"><span data-stu-id="d078a-126">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="d078a-127">Карточка контакта</span><span class="sxs-lookup"><span data-stu-id="d078a-127">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="d078a-128">Всплывающий элемент, который используется в компоненте "Человек", чтобы отобразить больше сведений профиля о пользователе.</span><span class="sxs-lookup"><span data-stu-id="d078a-128">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="d078a-129">Get</span><span class="sxs-lookup"><span data-stu-id="d078a-129">Get</span></span>](./components/get.md)|<span data-ttu-id="d078a-130">Создание GET-запроса к API Microsoft Graph прямо в HTML.</span><span class="sxs-lookup"><span data-stu-id="d078a-130">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="d078a-131">Средство выбора каналов</span><span class="sxs-lookup"><span data-stu-id="d078a-131">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="d078a-132">Предоставляет возможность поиска каналов Microsoft Teams и выбора канала из отображенного списка результатов.</span><span class="sxs-lookup"><span data-stu-id="d078a-132">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|
|[<span data-ttu-id="d078a-133">To Do</span><span class="sxs-lookup"><span data-stu-id="d078a-133">To Do</span></span>](./components/todo.md)|<span data-ttu-id="d078a-134">Отображает и включает добавление, удаление, выполнение или редактирование задач из Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="d078a-134">Displays and enables adding, removing, completing, or editing of tasks from Microsoft To Do.</span></span>|

### <a name="providers"></a><span data-ttu-id="d078a-135">Поставщики</span><span class="sxs-lookup"><span data-stu-id="d078a-135">Providers</span></span>

<span data-ttu-id="d078a-136">[Поставщики](/providers/providers.md) включают проверку подлинности, предоставляют реализацию для приобретения маркеров доступа на разных платформах и используют клиент Microsoft Graph для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d078a-136">[Providers](/providers/providers.md) enable authentication and provide the implementation for acquiring access tokens on various platforms and expose a Microsoft Graph client for calling the Microsoft Graph APIs.</span></span> <span data-ttu-id="d078a-137">Компоненты работают наилучшим образом, если используются с поставщиком, однако поставщики могут использоваться самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="d078a-137">The components work best when used with a provider, but the providers can be used on their own.</span></span>

|<span data-ttu-id="d078a-138">Поставщики</span><span class="sxs-lookup"><span data-stu-id="d078a-138">Providers</span></span>|<span data-ttu-id="d078a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d078a-139">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="d078a-140">MSAL</span><span class="sxs-lookup"><span data-stu-id="d078a-140">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="d078a-141">Использует MSAL.js для входа в систему и получения маркеров, которые применяются с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d078a-141">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="d078a-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="d078a-142">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="d078a-143">Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d078a-143">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="d078a-144">Teams</span><span class="sxs-lookup"><span data-stu-id="d078a-144">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="d078a-145">Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам во вкладках Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d078a-145">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="d078a-146">Прокси-сервер</span><span class="sxs-lookup"><span data-stu-id="d078a-146">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="d078a-147">Позволяет использовать проверку подлинности на внутреннем сервере с помощью маршрутизации всех вызовов Microsoft Graph через внутренний сервер.</span><span class="sxs-lookup"><span data-stu-id="d078a-147">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="d078a-148">Настраиваемый</span><span class="sxs-lookup"><span data-stu-id="d078a-148">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="d078a-149">Создание настраиваемого поставщика для включения проверки подлинности и доступа к Microsoft Graph с помощью существующего кода проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="d078a-149">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="d078a-150">Зачем использовать Microsoft Graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="d078a-150">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="d078a-151">Microsoft Graph Toolkit позволяет быстро и легко интегрировать общие возможности на платформе Microsoft Graph в собственное приложение.</span><span class="sxs-lookup"><span data-stu-id="d078a-151">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="d078a-152">**Сокращает срок разработки**</span><span class="sxs-lookup"><span data-stu-id="d078a-152">**Cut Development Time**</span></span>

    <span data-ttu-id="d078a-153">Работа по подключению API Microsoft Graph и отображению данных в пользовательском интерфейсе, который выглядит и работает как возможность Microsoft365, выполняется за вас, без обязательной настройки.</span><span class="sxs-lookup"><span data-stu-id="d078a-153">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="d078a-154">**Работает везде**</span><span class="sxs-lookup"><span data-stu-id="d078a-154">**Works Everywhere**</span></span>

    <span data-ttu-id="d078a-155">Все компоненты соответствуют веб-стандартам и работают без проблем с любым современным браузером и веб-платформой (React, Angular, Vue и т. д.).</span><span class="sxs-lookup"><span data-stu-id="d078a-155">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="d078a-156">**Красивый, но гибкий**</span><span class="sxs-lookup"><span data-stu-id="d078a-156">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="d078a-157">Компоненты выглядят и работают как возможности Microsoft365, но также могут быть настроены с помощью [настраиваемых свойств CSS](./customize-components/style.md) и [шаблонов](./customize-components/templates.md).</span><span class="sxs-lookup"><span data-stu-id="d078a-157">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./customize-components/style.md) and [templating](./customize-components/templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="d078a-158">Кто должен его использовать?</span><span class="sxs-lookup"><span data-stu-id="d078a-158">Who should use it?</span></span>

<span data-ttu-id="d078a-159">Microsoft Graph Toolkit — это находка для разработчиков любого уровня, которые хотят разработать веб-приложение, вкладку Microsoft Teams или веб-часть SharePoint, которая подключается и обращается к данным Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d078a-159">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop a web application, Microsoft Teams tab, or SharePoint web part that connects to and accesses data from Microsoft Graph.</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="d078a-160">Где его можно использовать?</span><span class="sxs-lookup"><span data-stu-id="d078a-160">Where can I use it?</span></span>

<span data-ttu-id="d078a-161">Microsoft Graph Toolkit поддерживается в следующих браузерах.</span><span class="sxs-lookup"><span data-stu-id="d078a-161">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="d078a-168">**Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="d078a-168">**Edge**</span></span>|<span data-ttu-id="d078a-169">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="d078a-169">**Firefox**</span></span>|<span data-ttu-id="d078a-170">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="d078a-170">**Chrome**</span></span>|<span data-ttu-id="d078a-171">**Safari**</span><span class="sxs-lookup"><span data-stu-id="d078a-171">**Safari**</span></span>|<span data-ttu-id="d078a-172">**Opera**</span><span class="sxs-lookup"><span data-stu-id="d078a-172">**Opera**</span></span>|<span data-ttu-id="d078a-173">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="d078a-173">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="d078a-174">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d078a-174">Next steps</span></span>

- <span data-ttu-id="d078a-175">Попробуйте компоненты в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="d078a-175">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="d078a-176">[Начало работы](./get-started/overview.md) с Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="d078a-176">[Get started](./get-started/overview.md) with the Microsoft Graph Toolkit.</span></span>
- <span data-ttu-id="d078a-177">Ознакомьтесь с Microsoft Graph Toolkit на [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="d078a-177">Check out the Microsoft Graph Toolkit on [GitHub](https://aka.ms/mgt).</span></span>
