---
title: 'Microsoft Graph Toolkit: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph'
description: Microsoft Graph Toolkit — это коллекция поставщиков проверки подлинности и многократно используемых, не зависящих от платформы веб-компонентов для доступа и работы в Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e39eba8c79d2aae3d1ce048a21d2d0a911aed089
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579769"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a><span data-ttu-id="5507f-103">Microsoft Graph Toolkit: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5507f-103">Microsoft Graph Toolkit: UI Components and Authentication Providers for Microsoft Graph</span></span> 

<span data-ttu-id="5507f-104">Microsoft Graph Toolkit — это коллекция многократно используемых, не зависящих от платформы компонентов и поставщиков проверки подлинности для доступа и работы в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5507f-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic components and authentication providers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="5507f-105">Готовые компоненты являются полностью функциональными и включают встроенных поставщиков, которые проверяют подлинность и получают данные из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5507f-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="5507f-106">С помощью Microsoft Graph Toolkit можно легко использовать Microsoft Graph в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="5507f-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="5507f-107">В следующем примере вошедший пользователь и события его календаря отображаются всего лишь в двух строках кода с помощью компонентов [Вход](./components/login.md) и [Повестка дня](./components/agenda.md).</span><span class="sxs-lookup"><span data-stu-id="5507f-107">In the following example, a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="5507f-108">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="5507f-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="5507f-109">Что включает Microsoft Graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="5507f-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="5507f-110">Компоненты</span><span class="sxs-lookup"><span data-stu-id="5507f-110">Components</span></span>

<span data-ttu-id="5507f-111">Microsoft Graph Toolkit включает коллекцию веб-компонентов для наиболее распространенных встроенных возможностей на базе API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5507f-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span> 

<span data-ttu-id="5507f-112">Они также доступны как [компоненты React](./get-started/mgt-react.md).</span><span class="sxs-lookup"><span data-stu-id="5507f-112">The components are also available as [React components](./get-started/mgt-react.md).</span></span>

|<span data-ttu-id="5507f-113">Компонент</span><span class="sxs-lookup"><span data-stu-id="5507f-113">Component</span></span>|<span data-ttu-id="5507f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5507f-114">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="5507f-115">Вход</span><span class="sxs-lookup"><span data-stu-id="5507f-115">Login</span></span>](./components/login.md)|<span data-ttu-id="5507f-116">Кнопка и элемент управления "Всплывающий элемент" для проверки подлинности пользователя с помощью платформы удостоверений Майкрософт и отображения сведений из профиля пользователя при входе.</span><span class="sxs-lookup"><span data-stu-id="5507f-116">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="5507f-117">Человек</span><span class="sxs-lookup"><span data-stu-id="5507f-117">Person</span></span>](./components/person.md)|<span data-ttu-id="5507f-118">Отображает пользователя или контакт с помощью его фотографии, имени и/или адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5507f-118">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="5507f-119">Люди</span><span class="sxs-lookup"><span data-stu-id="5507f-119">People</span></span>](./components/people.md)|<span data-ttu-id="5507f-120">Отображает группу людей или контактов с помощью их фотографий или инициалов.</span><span class="sxs-lookup"><span data-stu-id="5507f-120">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="5507f-121">Повестка дня</span><span class="sxs-lookup"><span data-stu-id="5507f-121">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="5507f-122">Отображает события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="5507f-122">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="5507f-123">Задачи</span><span class="sxs-lookup"><span data-stu-id="5507f-123">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="5507f-124">Отображает и включает добавление, удаление, выполнение или редактирование задач из Планировщика (Майкрософт) или Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="5507f-124">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To Do.</span></span>|
|[<span data-ttu-id="5507f-125">Выбор людей</span><span class="sxs-lookup"><span data-stu-id="5507f-125">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="5507f-126">Предоставляет возможность поиска людей и отображает список результатов.</span><span class="sxs-lookup"><span data-stu-id="5507f-126">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="5507f-127">Карточка контакта</span><span class="sxs-lookup"><span data-stu-id="5507f-127">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="5507f-128">Всплывающий элемент, который используется в компоненте "Человек", чтобы отобразить больше сведений профиля о пользователе.</span><span class="sxs-lookup"><span data-stu-id="5507f-128">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="5507f-129">Get</span><span class="sxs-lookup"><span data-stu-id="5507f-129">Get</span></span>](./components/get.md)|<span data-ttu-id="5507f-130">Создание GET-запроса к API Microsoft Graph прямо в HTML.</span><span class="sxs-lookup"><span data-stu-id="5507f-130">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="5507f-131">Средство выбора каналов</span><span class="sxs-lookup"><span data-stu-id="5507f-131">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="5507f-132">Предоставляет возможность поиска каналов Microsoft Teams и выбора канала из отображенного списка результатов.</span><span class="sxs-lookup"><span data-stu-id="5507f-132">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|
|[<span data-ttu-id="5507f-133">To Do</span><span class="sxs-lookup"><span data-stu-id="5507f-133">To Do</span></span>](./components/todo.md)|<span data-ttu-id="5507f-134">Отображает и включает добавление, удаление, выполнение или редактирование задач из Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="5507f-134">Displays and enables adding, removing, completing, or editing of tasks from Microsoft To Do.</span></span>|

### <a name="providers"></a><span data-ttu-id="5507f-135">Поставщики</span><span class="sxs-lookup"><span data-stu-id="5507f-135">Providers</span></span>

<span data-ttu-id="5507f-136">[Поставщики](/providers/providers.md) включают проверку подлинности, предоставляют реализацию для приобретения маркеров доступа на разных платформах и используют клиент Microsoft Graph для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5507f-136">[Providers](/providers/providers.md) enable authentication and provide the implementation for acquiring access tokens on various platforms and expose a Microsoft Graph client for calling the Microsoft Graph APIs.</span></span> <span data-ttu-id="5507f-137">Компоненты работают наилучшим образом, если используются с поставщиком, однако поставщики могут использоваться самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="5507f-137">The components work best when used with a provider, but the providers can be used on their own.</span></span>

|<span data-ttu-id="5507f-138">Поставщики</span><span class="sxs-lookup"><span data-stu-id="5507f-138">Providers</span></span>|<span data-ttu-id="5507f-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5507f-139">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="5507f-140">MSAL</span><span class="sxs-lookup"><span data-stu-id="5507f-140">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="5507f-141">Использует MSAL.js для входа в систему и получения маркеров, которые применяются с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5507f-141">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="5507f-142">Msal 2.0</span><span class="sxs-lookup"><span data-stu-id="5507f-142">Msal 2.0</span></span>](./providers/msal2.md)| <span data-ttu-id="5507f-143">Использует msal-браузер для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5507f-143">Uses msal-browser to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="5507f-144">Электрон</span><span class="sxs-lookup"><span data-stu-id="5507f-144">Electron</span></span>](./providers/electron.md)|<span data-ttu-id="5507f-145">Проверка подлинности и Graph доступа к компонентам в приложениях Electron</span><span class="sxs-lookup"><span data-stu-id="5507f-145">Authenticates and provides Microsoft Graph access to components inside of Electron apps</span></span>|
|[<span data-ttu-id="5507f-146">SharePoint</span><span class="sxs-lookup"><span data-stu-id="5507f-146">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="5507f-147">Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5507f-147">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="5507f-148">Teams</span><span class="sxs-lookup"><span data-stu-id="5507f-148">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="5507f-149">Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам во вкладках Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5507f-149">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="5507f-150">Прокси-сервер</span><span class="sxs-lookup"><span data-stu-id="5507f-150">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="5507f-151">Позволяет использовать проверку подлинности на внутреннем сервере с помощью маршрутизации всех вызовов Microsoft Graph через внутренний сервер.</span><span class="sxs-lookup"><span data-stu-id="5507f-151">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="5507f-152">Настраиваемый</span><span class="sxs-lookup"><span data-stu-id="5507f-152">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="5507f-153">Создание настраиваемого поставщика для включения проверки подлинности и доступа к Microsoft Graph с помощью существующего кода проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="5507f-153">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="5507f-154">Зачем использовать Microsoft Graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="5507f-154">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="5507f-155">Microsoft Graph Toolkit позволяет быстро и легко интегрировать общие возможности на платформе Microsoft Graph в собственное приложение.</span><span class="sxs-lookup"><span data-stu-id="5507f-155">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="5507f-156">**Сокращает срок разработки**</span><span class="sxs-lookup"><span data-stu-id="5507f-156">**Cut Development Time**</span></span>

    <span data-ttu-id="5507f-157">Работа по подключению API Microsoft Graph и отображению данных в пользовательском интерфейсе, который выглядит и работает как возможность Microsoft365, выполняется за вас, без обязательной настройки.</span><span class="sxs-lookup"><span data-stu-id="5507f-157">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="5507f-158">**Работает везде**</span><span class="sxs-lookup"><span data-stu-id="5507f-158">**Works Everywhere**</span></span>

    <span data-ttu-id="5507f-159">Все компоненты соответствуют веб-стандартам и работают без проблем с любым современным браузером и веб-платформой (React, Angular, Vue и т. д.).</span><span class="sxs-lookup"><span data-stu-id="5507f-159">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="5507f-160">**Красивый, но гибкий**</span><span class="sxs-lookup"><span data-stu-id="5507f-160">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="5507f-161">Компоненты выглядят и работают как возможности Microsoft365, но также могут быть настроены с помощью [настраиваемых свойств CSS](./customize-components/style.md) и [шаблонов](./customize-components/templates.md).</span><span class="sxs-lookup"><span data-stu-id="5507f-161">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./customize-components/style.md) and [templating](./customize-components/templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="5507f-162">Кто должен его использовать?</span><span class="sxs-lookup"><span data-stu-id="5507f-162">Who should use it?</span></span>

<span data-ttu-id="5507f-163">Microsoft Graph набор средств отлично подходит для разработчиков всех уровней опыта, которые ищут возможность разработки приложения, которое подключается к данным microsoft Graph, например:</span><span class="sxs-lookup"><span data-stu-id="5507f-163">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop an app that connects to and accesses data from Microsoft Graph, such as a:</span></span>
- <span data-ttu-id="5507f-164">Веб-приложение</span><span class="sxs-lookup"><span data-stu-id="5507f-164">Web app</span></span>
- <span data-ttu-id="5507f-165">Microsoft Teams вкладка</span><span class="sxs-lookup"><span data-stu-id="5507f-165">Microsoft Teams tab</span></span>
- <span data-ttu-id="5507f-166">Прогрессивное веб-приложение (PWA)</span><span class="sxs-lookup"><span data-stu-id="5507f-166">Progressive Web App (PWA)</span></span>
- <span data-ttu-id="5507f-167">Электронное приложение</span><span class="sxs-lookup"><span data-stu-id="5507f-167">Electron app</span></span>
- <span data-ttu-id="5507f-168">SharePoint веб-части</span><span class="sxs-lookup"><span data-stu-id="5507f-168">SharePoint web part</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="5507f-169">Где его можно использовать?</span><span class="sxs-lookup"><span data-stu-id="5507f-169">Where can I use it?</span></span>

<span data-ttu-id="5507f-170">Microsoft Graph Toolkit поддерживается в следующих браузерах.</span><span class="sxs-lookup"><span data-stu-id="5507f-170">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="5507f-177">**Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="5507f-177">**Edge**</span></span>|<span data-ttu-id="5507f-178">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="5507f-178">**Firefox**</span></span>|<span data-ttu-id="5507f-179">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="5507f-179">**Chrome**</span></span>|<span data-ttu-id="5507f-180">**Safari**</span><span class="sxs-lookup"><span data-stu-id="5507f-180">**Safari**</span></span>|<span data-ttu-id="5507f-181">**Opera**</span><span class="sxs-lookup"><span data-stu-id="5507f-181">**Opera**</span></span>|<span data-ttu-id="5507f-182">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="5507f-182">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="5507f-183">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="5507f-183">Next steps</span></span>

- <span data-ttu-id="5507f-184">Попробуйте компоненты в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="5507f-184">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="5507f-185">[Начало работы](./get-started/overview.md) с Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="5507f-185">[Get started](./get-started/overview.md) with the Microsoft Graph Toolkit.</span></span>
- <span data-ttu-id="5507f-186">Ознакомьтесь с Microsoft Graph Toolkit на [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="5507f-186">Check out the Microsoft Graph Toolkit on [GitHub](https://aka.ms/mgt).</span></span>
