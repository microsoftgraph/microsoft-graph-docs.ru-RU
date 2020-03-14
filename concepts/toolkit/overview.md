---
title: 'Набор средств Microsoft Graph: веб-компоненты на платформе Microsoft Graph'
description: Набор инструментов Microsoft Graph представляет собой набор ресуабле, независимых от платформы веб-компонентов и вспомогательных средств для доступа к Microsoft Graph и работы с ним.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 348e08212010f66fdde5ee3b752fe901699fbaa9
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639555"
---
# <a name="microsoft-graph-toolkit-web-components-powered-by-microsoft-graph"></a><span data-ttu-id="74602-103">Набор средств Microsoft Graph: веб-компоненты на платформе Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="74602-103">Microsoft Graph Toolkit: Web Components powered by Microsoft Graph</span></span>

<span data-ttu-id="74602-104">Набор инструментов Microsoft Graph представляет собой набор компонентов и вспомогательных программ для доступа к Microsoft Graph, не зависящего от платформы.</span><span class="sxs-lookup"><span data-stu-id="74602-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="74602-105">Компоненты полностью функционируют прямо из этого поля со встроенными поставщиками, которые проходят проверку подлинности и извлекают данные из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="74602-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="74602-106">Набор средств Microsoft Graph позволяет легко использовать Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="74602-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="74602-107">В приведенном ниже примере показано, как пользователи, вошедшего в систему, и их события календаря отображаются только с двумя строками кода, используя компоненты [входа](./components/login.md) и [повестки](./components/agenda.md) .</span><span class="sxs-lookup"><span data-stu-id="74602-107">In the example below, see how a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="74602-108">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="74602-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="74602-109">Что входит в набор средств Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="74602-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="74602-110">Компоненты</span><span class="sxs-lookup"><span data-stu-id="74602-110">Components</span></span>

<span data-ttu-id="74602-111">Набор средств Microsoft Graph включает в себя набор веб-компонентов для наиболее часто создаваемых интерфейсов API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="74602-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span>

|<span data-ttu-id="74602-112">Компонент</span><span class="sxs-lookup"><span data-stu-id="74602-112">Component</span></span>|<span data-ttu-id="74602-113">Описание</span><span class="sxs-lookup"><span data-stu-id="74602-113">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="74602-114">Вход</span><span class="sxs-lookup"><span data-stu-id="74602-114">Login</span></span>](./components/login.md)|<span data-ttu-id="74602-115">Кнопка и всплывающий элемент управления для проверки подлинности пользователя с платформой Microsoft Identity и отображения сведений о профиле пользователя при входе.</span><span class="sxs-lookup"><span data-stu-id="74602-115">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="74602-116">Пользователь</span><span class="sxs-lookup"><span data-stu-id="74602-116">Person</span></span>](./components/person.md)|<span data-ttu-id="74602-117">Отображает пользователя или контакт по фотографии, названию и/или адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="74602-117">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="74602-118">Люди</span><span class="sxs-lookup"><span data-stu-id="74602-118">People</span></span>](./components/people.md)|<span data-ttu-id="74602-119">Отображает группу людей или контактов по их фотографиям или инициалам.</span><span class="sxs-lookup"><span data-stu-id="74602-119">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="74602-120">Повестка</span><span class="sxs-lookup"><span data-stu-id="74602-120">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="74602-121">Отображает события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="74602-121">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="74602-122">Tasks</span><span class="sxs-lookup"><span data-stu-id="74602-122">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="74602-123">Показывает и разрешает добавлять, удалять, завершать или изменять задачи из планировщика (Майкрософт) или задачи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="74602-123">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To-Do.</span></span>|
|[<span data-ttu-id="74602-124">Средство выбора людей</span><span class="sxs-lookup"><span data-stu-id="74602-124">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="74602-125">Предоставляет возможность поиска людей и отображения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="74602-125">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="74602-126">Карточка лица</span><span class="sxs-lookup"><span data-stu-id="74602-126">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="74602-127">Раскрывающееся меню, используемое компонентом Person для отображения дополнительных сведений о профиле пользователя.</span><span class="sxs-lookup"><span data-stu-id="74602-127">A flyout used on the person component to display more profile information about a user.</span></span>|
|<span data-ttu-id="74602-128">[получение](./components/get.md);</span><span class="sxs-lookup"><span data-stu-id="74602-128">[Get](./components/get.md)</span></span>|<span data-ttu-id="74602-129">Сделайте запрос GET к любому API Microsoft Graph непосредственно в HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="74602-129">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|

### <a name="providers"></a><span data-ttu-id="74602-130">Поставщики</span><span class="sxs-lookup"><span data-stu-id="74602-130">Providers</span></span>

<span data-ttu-id="74602-131">Компоненты лучше всего подходят для использования с [поставщиками](/providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="74602-131">The components work best when used with a [provider](/providers/providers.md).</span></span> <span data-ttu-id="74602-132">Поставщики обеспечивают проверку подлинности и предоставляют реализацию для получения маркеров доступа для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="74602-132">Providers enable authentication and provide the implementation for acquiring the access tokens for calling the Microsoft Graph APIs.</span></span>

|<span data-ttu-id="74602-133">Поставщики</span><span class="sxs-lookup"><span data-stu-id="74602-133">Providers</span></span>|<span data-ttu-id="74602-134">Описание</span><span class="sxs-lookup"><span data-stu-id="74602-134">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="74602-135">Msal</span><span class="sxs-lookup"><span data-stu-id="74602-135">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="74602-136">Использует MSAL. js для входа пользователей и получения маркеров для использования с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="74602-136">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="74602-137">SharePoint</span><span class="sxs-lookup"><span data-stu-id="74602-137">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="74602-138">Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.</span><span class="sxs-lookup"><span data-stu-id="74602-138">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="74602-139">Teams</span><span class="sxs-lookup"><span data-stu-id="74602-139">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="74602-140">Проверка подлинности и предоставление доступа Microsoft Graph к компонентам внутри вкладок Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="74602-140">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="74602-141">Сервера</span><span class="sxs-lookup"><span data-stu-id="74602-141">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="74602-142">Позволяет использовать внутреннюю проверку подлинности путем маршрутизации всех вызовов Microsoft Graph через серверный сервер.</span><span class="sxs-lookup"><span data-stu-id="74602-142">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="74602-143">Пользовательский</span><span class="sxs-lookup"><span data-stu-id="74602-143">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="74602-144">Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph с помощью существующего кода проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="74602-144">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="74602-145">Зачем использовать набор средств Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="74602-145">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="74602-146">Набор средств Microsoft Graph позволяет быстро и легко интегрировать общедоступные возможности Microsoft Graph в свое приложение.</span><span class="sxs-lookup"><span data-stu-id="74602-146">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="74602-147">**Сокращение времени разработки**</span><span class="sxs-lookup"><span data-stu-id="74602-147">**Cut Development Time**</span></span>

    <span data-ttu-id="74602-148">Работа по подключению к API Microsoft Graph и визуализация данных в пользовательском интерфейсе, которая выглядит так же, как Microsoft365, выполняется без необходимости настройки.</span><span class="sxs-lookup"><span data-stu-id="74602-148">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="74602-149">**Работает везде**</span><span class="sxs-lookup"><span data-stu-id="74602-149">**Works Everywhere**</span></span>

    <span data-ttu-id="74602-150">Все компоненты основываются на веб-стандартах и тесно работают с любым современным браузером и веб-средой (реагируем, радиально, Vue и т. д.).</span><span class="sxs-lookup"><span data-stu-id="74602-150">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="74602-151">**Прекрасная, но гибкая**</span><span class="sxs-lookup"><span data-stu-id="74602-151">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="74602-152">Компоненты предназначены для внешнего вида и работы с Microsoft365, но также могут настраиваться с помощью [настраиваемых свойств CSS](./style.md) и [шаблонов](./templates.md).</span><span class="sxs-lookup"><span data-stu-id="74602-152">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./style.md) and [templating](./templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="74602-153">Кто должен использовать его?</span><span class="sxs-lookup"><span data-stu-id="74602-153">Who should use it?</span></span>

<span data-ttu-id="74602-154">Набор средств Microsoft Graph прекрасно подходит разработчикам всех уровней опыта разработки веб-приложения, вкладки Microsoft Teams или веб-части SharePoint, которые подключаются к данным из Microsoft Graph и обращаются к ним.</span><span class="sxs-lookup"><span data-stu-id="74602-154">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop a web application, Microsoft Teams tab, or SharePoint web part that connects to and accesses data from Microsoft Graph.</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="74602-155">Где можно использовать его?</span><span class="sxs-lookup"><span data-stu-id="74602-155">Where can I use it?</span></span>

<span data-ttu-id="74602-156">Набор средств Microsoft Graph поддерживается в следующих браузерах.</span><span class="sxs-lookup"><span data-stu-id="74602-156">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Microsoft Edge](images/edgeIcon.png)|![Internet Explorer 11](images/internetExplorerIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="74602-164">**Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="74602-164">**Edge**</span></span>|<span data-ttu-id="74602-165">**IE 11**</span><span class="sxs-lookup"><span data-stu-id="74602-165">**IE 11**</span></span>|<span data-ttu-id="74602-166">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="74602-166">**Firefox**</span></span>|<span data-ttu-id="74602-167">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="74602-167">**Chrome**</span></span>|<span data-ttu-id="74602-168">**Safari**</span><span class="sxs-lookup"><span data-stu-id="74602-168">**Safari**</span></span>|<span data-ttu-id="74602-169">**Opera**</span><span class="sxs-lookup"><span data-stu-id="74602-169">**Opera**</span></span>|<span data-ttu-id="74602-170">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="74602-170">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="74602-171">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="74602-171">Next steps</span></span>

- <span data-ttu-id="74602-172">Опробуйте компоненты в [интерактивная среда](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="74602-172">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="74602-173">Приступите к [работе](get-started.md) с набором инструментов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="74602-173">[Get started](get-started.md) with the Microsoft Graph Toolkit.</span></span>
