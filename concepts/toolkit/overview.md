---
title: 'Набор средств Microsoft Graph: веб-компоненты на платформе Microsoft Graph'
description: Набор инструментов Microsoft Graph представляет собой набор ресуабле, независимых от платформы веб-компонентов и вспомогательных средств для доступа к Microsoft Graph и работы с ним.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: ba19e1697700800de22d193f8bbb1a959776a18f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036865"
---
# <a name="microsoft-graph-toolkit-web-components-powered-by-microsoft-graph"></a><span data-ttu-id="5fc7f-103">Набор средств Microsoft Graph: веб-компоненты на платформе Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5fc7f-103">Microsoft Graph Toolkit: Web Components powered by Microsoft Graph</span></span>

<span data-ttu-id="5fc7f-104">Набор инструментов Microsoft Graph представляет собой набор компонентов и вспомогательных программ для доступа к Microsoft Graph, не зависящего от платформы.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="5fc7f-105">Компоненты полностью функционируют прямо из этого поля со встроенными поставщиками, которые проходят проверку подлинности и извлекают данные из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="5fc7f-106">Набор средств Microsoft Graph позволяет легко использовать Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="5fc7f-107">В приведенном ниже примере показано, как пользователи, вошедшего в систему, и их события календаря отображаются только с двумя строками кода, используя компоненты [входа](./components/login.md) и [повестки](./components/agenda.md) .</span><span class="sxs-lookup"><span data-stu-id="5fc7f-107">In the example below, see how a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="5fc7f-108">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="5fc7f-109">Что входит в набор средств Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="5fc7f-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="5fc7f-110">Компоненты</span><span class="sxs-lookup"><span data-stu-id="5fc7f-110">Components</span></span>

<span data-ttu-id="5fc7f-111">Набор средств Microsoft Graph включает в себя набор веб-компонентов для наиболее часто создаваемых интерфейсов API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span>

|<span data-ttu-id="5fc7f-112">Компонент</span><span class="sxs-lookup"><span data-stu-id="5fc7f-112">Component</span></span>|<span data-ttu-id="5fc7f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5fc7f-113">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="5fc7f-114">Вход</span><span class="sxs-lookup"><span data-stu-id="5fc7f-114">Login</span></span>](./components/login.md)|<span data-ttu-id="5fc7f-115">Кнопка и всплывающий элемент управления для проверки подлинности пользователя с платформой Microsoft Identity и отображения сведений о профиле пользователя при входе.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-115">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="5fc7f-116">Пользователь</span><span class="sxs-lookup"><span data-stu-id="5fc7f-116">Person</span></span>](./components/person.md)|<span data-ttu-id="5fc7f-117">Отображает пользователя или контакт по фотографии, названию и/или адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-117">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="5fc7f-118">Люди</span><span class="sxs-lookup"><span data-stu-id="5fc7f-118">People</span></span>](./components/people.md)|<span data-ttu-id="5fc7f-119">Отображает группу людей или контактов по их фотографиям или инициалам.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-119">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="5fc7f-120">Повестка</span><span class="sxs-lookup"><span data-stu-id="5fc7f-120">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="5fc7f-121">Отображает события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-121">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="5fc7f-122">Задачи</span><span class="sxs-lookup"><span data-stu-id="5fc7f-122">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="5fc7f-123">Показывает и разрешает добавлять, удалять, завершать или изменять задачи из планировщика (Майкрософт) или задачи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-123">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To-Do.</span></span>|
|[<span data-ttu-id="5fc7f-124">Средство выбора людей</span><span class="sxs-lookup"><span data-stu-id="5fc7f-124">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="5fc7f-125">Предоставляет возможность поиска людей и отображения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-125">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="5fc7f-126">Карточка лица</span><span class="sxs-lookup"><span data-stu-id="5fc7f-126">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="5fc7f-127">Раскрывающееся меню, используемое компонентом Person для отображения дополнительных сведений о профиле пользователя.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-127">A flyout used on the person component to display more profile information about a user.</span></span>|
|<span data-ttu-id="5fc7f-128">[получение](./components/get.md);</span><span class="sxs-lookup"><span data-stu-id="5fc7f-128">[Get](./components/get.md)</span></span>|<span data-ttu-id="5fc7f-129">Сделайте запрос GET к любому API Microsoft Graph непосредственно в HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-129">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="5fc7f-130">Выбор канала</span><span class="sxs-lookup"><span data-stu-id="5fc7f-130">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="5fc7f-131">Обеспечивает возможность поиска каналов Microsoft Teams для выбора канала из подготовленного списка результатов.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-131">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|

### <a name="providers"></a><span data-ttu-id="5fc7f-132">Поставщики</span><span class="sxs-lookup"><span data-stu-id="5fc7f-132">Providers</span></span>

<span data-ttu-id="5fc7f-133">Компоненты лучше всего подходят для использования с [поставщиками](/providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="5fc7f-133">The components work best when used with a [provider](/providers/providers.md).</span></span> <span data-ttu-id="5fc7f-134">Поставщики обеспечивают проверку подлинности и предоставляют реализацию для получения маркеров доступа для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-134">Providers enable authentication and provide the implementation for acquiring the access tokens for calling the Microsoft Graph APIs.</span></span>

|<span data-ttu-id="5fc7f-135">Поставщики</span><span class="sxs-lookup"><span data-stu-id="5fc7f-135">Providers</span></span>|<span data-ttu-id="5fc7f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="5fc7f-136">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="5fc7f-137">Msal</span><span class="sxs-lookup"><span data-stu-id="5fc7f-137">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="5fc7f-138">Использует MSAL.js для входа пользователей и получения маркеров для использования с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-138">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="5fc7f-139">SharePoint</span><span class="sxs-lookup"><span data-stu-id="5fc7f-139">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="5fc7f-140">Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-140">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="5fc7f-141">Teams</span><span class="sxs-lookup"><span data-stu-id="5fc7f-141">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="5fc7f-142">Проверка подлинности и предоставление доступа Microsoft Graph к компонентам внутри вкладок Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-142">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="5fc7f-143">Сервера</span><span class="sxs-lookup"><span data-stu-id="5fc7f-143">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="5fc7f-144">Позволяет использовать внутреннюю проверку подлинности путем маршрутизации всех вызовов Microsoft Graph через серверный сервер.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-144">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="5fc7f-145">Пользовательский</span><span class="sxs-lookup"><span data-stu-id="5fc7f-145">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="5fc7f-146">Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph с помощью существующего кода проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-146">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="5fc7f-147">Зачем использовать набор средств Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="5fc7f-147">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="5fc7f-148">Набор средств Microsoft Graph позволяет быстро и легко интегрировать общедоступные возможности Microsoft Graph в свое приложение.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-148">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="5fc7f-149">**Сокращение времени разработки**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-149">**Cut Development Time**</span></span>

    <span data-ttu-id="5fc7f-150">Работа по подключению к API Microsoft Graph и визуализация данных в пользовательском интерфейсе, которая выглядит так же, как Microsoft365, выполняется без необходимости настройки.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-150">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="5fc7f-151">**Работает везде**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-151">**Works Everywhere**</span></span>

    <span data-ttu-id="5fc7f-152">Все компоненты основываются на веб-стандартах и тесно работают с любым современным браузером и веб-средой (реагируем, радиально, Vue и т. д.).</span><span class="sxs-lookup"><span data-stu-id="5fc7f-152">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="5fc7f-153">**Прекрасная, но гибкая**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-153">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="5fc7f-154">Компоненты предназначены для внешнего вида и работы с Microsoft365, но также могут настраиваться с помощью [настраиваемых свойств CSS](./style.md) и [шаблонов](./templates.md).</span><span class="sxs-lookup"><span data-stu-id="5fc7f-154">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./style.md) and [templating](./templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="5fc7f-155">Кто должен использовать его?</span><span class="sxs-lookup"><span data-stu-id="5fc7f-155">Who should use it?</span></span>

<span data-ttu-id="5fc7f-156">Набор средств Microsoft Graph прекрасно подходит разработчикам всех уровней опыта разработки веб-приложения, вкладки Microsoft Teams или веб-части SharePoint, которые подключаются к данным из Microsoft Graph и обращаются к ним.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-156">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop a web application, Microsoft Teams tab, or SharePoint web part that connects to and accesses data from Microsoft Graph.</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="5fc7f-157">Где можно использовать его?</span><span class="sxs-lookup"><span data-stu-id="5fc7f-157">Where can I use it?</span></span>

<span data-ttu-id="5fc7f-158">Набор средств Microsoft Graph поддерживается в следующих браузерах.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-158">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Microsoft Edge](images/edgeIcon.png)|![Internet Explorer 11](images/internetExplorerIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="5fc7f-166">**Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-166">**Edge**</span></span>|<span data-ttu-id="5fc7f-167">**IE 11**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-167">**IE 11**</span></span>|<span data-ttu-id="5fc7f-168">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-168">**Firefox**</span></span>|<span data-ttu-id="5fc7f-169">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-169">**Chrome**</span></span>|<span data-ttu-id="5fc7f-170">**Safari**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-170">**Safari**</span></span>|<span data-ttu-id="5fc7f-171">**Opera**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-171">**Opera**</span></span>|<span data-ttu-id="5fc7f-172">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="5fc7f-172">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="5fc7f-173">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="5fc7f-173">Next steps</span></span>

- <span data-ttu-id="5fc7f-174">Опробуйте компоненты в [интерактивная среда](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="5fc7f-174">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="5fc7f-175">Приступите к [работе](./get-started/overview.md) с набором инструментов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fc7f-175">[Get started](./get-started/overview.md) with the Microsoft Graph Toolkit.</span></span>
- <span data-ttu-id="5fc7f-176">Ознакомьтесь со статьей Microsoft Graph Toolkit на сайте [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="5fc7f-176">Check out the Microsoft Graph Toolkit on [GitHub](https://aka.ms/mgt).</span></span>
