---
title: Работа с graph Explorer
description: Узнайте, как использовать некоторые важные функции в обозревателе Graph.
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: d9fe847a4e9402f1f8523afcd350c77bf3a88766
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013755"
---
# <a name="working-with-graph-explorer"></a><span data-ttu-id="3e56b-103">Работа с graph Explorer</span><span class="sxs-lookup"><span data-stu-id="3e56b-103">Working with Graph Explorer</span></span>

<span data-ttu-id="3e56b-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) — это средство разработчика, которое позволяет удобно создавать запросы REST API Microsoft Graph и просматривать соответствующие ответы.</span><span class="sxs-lookup"><span data-stu-id="3e56b-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) is a developer tool that lets you conveniently make Microsoft Graph REST API requests and view corresponding responses.</span></span> <span data-ttu-id="3e56b-105">В этой статье описывается использование некоторых важных функций в обозревателе Graph.</span><span class="sxs-lookup"><span data-stu-id="3e56b-105">This article describes how to use some of the important features in Graph Explorer.</span></span>

## <a name="consent-to-permissions"></a><span data-ttu-id="3e56b-106">Согласие на разрешения</span><span class="sxs-lookup"><span data-stu-id="3e56b-106">Consent to permissions</span></span>

<span data-ttu-id="3e56b-107">Пользователь или администратор должен предоставить graph Explorer правильные разрешения с помощью процесса согласия на доступ к данным в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3e56b-107">The user or administrator must grant Graph Explorer the correct permissions via a consent process to access data in Microsoft Graph.</span></span> <span data-ttu-id="3e56b-108">Соглашаться на разрешения в проводнике Graph с  помощью вкладки "Изменение разрешений" или параметра "Выбор разрешений" в шестеренке параметров рядом с вашим профилем при выходе из нее. </span><span class="sxs-lookup"><span data-stu-id="3e56b-108">Consent to permissions in Graph Explorer either via the **Modify permissions** tab or the **Select permissions** option in the settings gear next to your profile when you’re signed in.</span></span> <span data-ttu-id="3e56b-109">На **вкладке "Изменение разрешений"** перечислены все разрешения, необходимые для выполнения запроса в адресной панели.</span><span class="sxs-lookup"><span data-stu-id="3e56b-109">The **Modify permissions** tab lists all permissions you need to run the query in the address bar.</span></span> 

<span data-ttu-id="3e56b-110">Чтобы дать согласие на разрешения:</span><span class="sxs-lookup"><span data-stu-id="3e56b-110">To consent to permissions:</span></span>

1.  <span data-ttu-id="3e56b-111">Выберите пример запроса и запустите его.</span><span class="sxs-lookup"><span data-stu-id="3e56b-111">Select a sample query and run it.</span></span>
2.  <span data-ttu-id="3e56b-112">Выберите **вкладку "Изменение разрешений".**</span><span class="sxs-lookup"><span data-stu-id="3e56b-112">Select the **Modify permissions** tab.</span></span>
3.  <span data-ttu-id="3e56b-113">См. список разрешений, необходимых для выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="3e56b-113">See the list of permissions required to run the query.</span></span>
4.  <span data-ttu-id="3e56b-114">Выберите кнопку согласия рядом с разрешением, на который вы хотите согласиться.</span><span class="sxs-lookup"><span data-stu-id="3e56b-114">Select the consent button next to the permission you want to consent to.</span></span> 

![Screenshot of Graph Explorer with the steps to consent to permissions highlighted](./images/modify-permissions.png)

<span data-ttu-id="3e56b-116">Функция **"Изменение разрешений"** в настоящее время находится на стадии предварительного просмотра, и в некоторых запросах могут от отсутствуют разрешения.</span><span class="sxs-lookup"><span data-stu-id="3e56b-116">The **Modify  permissions** feature is currently in preview, and some queries might be missing permissions.</span></span> <span data-ttu-id="3e56b-117">Если для запроса отсутствуют разрешения, параметр **"Выбор** разрешений" в шестеренки параметров рядом с профилем содержит список всех доступных разрешений:</span><span class="sxs-lookup"><span data-stu-id="3e56b-117">If permissions are missing for a query, the **Select permissions** option in the settings gear next to your profile contains the list of all available permissions:</span></span>

1.  <span data-ttu-id="3e56b-118">Перейдите к шестеренкой параметров и выберите параметр **"Выбор** разрешений".</span><span class="sxs-lookup"><span data-stu-id="3e56b-118">Go the settings gear and click the **Select permissions** option.</span></span> <span data-ttu-id="3e56b-119">Этот параметр содержит список всех доступных разрешений.</span><span class="sxs-lookup"><span data-stu-id="3e56b-119">This option contains the list of all available permissions.</span></span>
2.  <span data-ttu-id="3e56b-120">Из списка всех разрешений согласиться с нужными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="3e56b-120">From the list of all the permissions, consent to the ones you want.</span></span>

![Снимок экрана: обозреватель Graph с выделенной опцией "Выбор разрешений"](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a><span data-ttu-id="3e56b-122">Получить маркер доступа или проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="3e56b-122">Get an access or authentication token</span></span>

<span data-ttu-id="3e56b-123">В проводнике Graph есть вкладка **маркера доступа,** на которую указывается маркер доступа при входе.</span><span class="sxs-lookup"><span data-stu-id="3e56b-123">Graph Explorer includes an **Access token** tab that shows your access token when you are signed in.</span></span> <span data-ttu-id="3e56b-124">На **вкладке маркера** Access вы можете скопировать маркер, если его необходимо использовать в своем любимом клиентских приложениях REST.</span><span class="sxs-lookup"><span data-stu-id="3e56b-124">On the **Access token** tab, you can copy the token if you need to use it in your favorite REST client application.</span></span>

![Снимок экрана: вкладка маркера доступа в обозревателе Graph с выделенной кнопкой "Копировать"](./images/access-token.png)

## <a name="copy-code-snippets"></a><span data-ttu-id="3e56b-126">Копирование фрагментов кода</span><span class="sxs-lookup"><span data-stu-id="3e56b-126">Copy code snippets</span></span>

<span data-ttu-id="3e56b-127">Для каждого запроса REST API, который вы выбираете или вводите в обозревателе Graph,  вы можете узнать, как вызывать этот API на каждом из четырех языков, демонстрируемых на вкладке "Фрагменты кода" — C#, Java, JavaScript и Objective-C.</span><span class="sxs-lookup"><span data-stu-id="3e56b-127">For each REST API query you select or enter in Graph Explorer, you can find how to call that API in each of the four languages showcased under the **Code snippets** tab - C#, Java, JavaScript, and Objective-C.</span></span> 

![Снимок экрана: обозреватель Graph с выделенной вкладками фрагментов кода](./images/code-snippets.png)

## <a name="ui-component-integration"></a><span data-ttu-id="3e56b-129">Интеграция компонентов пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="3e56b-129">UI component integration</span></span>

<span data-ttu-id="3e56b-130">В обозревателе Graph есть несколько функций, упрощающих реализацию пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="3e56b-130">Graph Explorer includes several features to make implementing UI easier.</span></span> <span data-ttu-id="3e56b-131">Повторное использование этих компонентов и в приложениях.</span><span class="sxs-lookup"><span data-stu-id="3e56b-131">Reuse these components in your apps too.</span></span>

### <a name="microsoft-graph-toolkit-integration"></a><span data-ttu-id="3e56b-132">Интеграция набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3e56b-132">Microsoft Graph Toolkit integration</span></span>

<span data-ttu-id="3e56b-133">Microsoft [Graph набор средств](/graph/toolkit/overview) — это коллекция веб-компонентов, которые не зависит от структуры, и помощников для доступа к Microsoft Graph и работы с ним.</span><span class="sxs-lookup"><span data-stu-id="3e56b-133">The [Microsoft Graph Toolkit](/graph/toolkit/overview) is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="3e56b-134">Компоненты полностью функциональны: встроенные поставщики, которые аутентификация и извлечение данных из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3e56b-134">The components are fully functional, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="3e56b-135">В проводнике Graph есть примеры запросов REST API, которые соответствуют набор средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3e56b-135">Graph Explorer provides sample REST API queries that correspond to Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="3e56b-136">Синяя точка на вкладке **набор средств** компонента указывает, что набор средств предоставляет компонент для указанного в настоящее время запроса REST API в обозревателе Graph.</span><span class="sxs-lookup"><span data-stu-id="3e56b-136">A blue dot on the **Toolkit component** tab indicates that the Toolkit provides a component for the currently specified REST API query in Graph Explorer.</span></span> <span data-ttu-id="3e56b-137">Вы можете легко скопировать код компонента в приложение.</span><span class="sxs-lookup"><span data-stu-id="3e56b-137">You can conveniently copy the code for the component to your app.</span></span>

<span data-ttu-id="3e56b-138">В следующей таблице перечислены примеры запросов, которые в настоящее время включают набор средств компонента.</span><span class="sxs-lookup"><span data-stu-id="3e56b-138">The following table lists the sample queries that currently include a Toolkit component.</span></span>

| <span data-ttu-id="3e56b-139">**Пример запроса в проводнике Graph**</span><span class="sxs-lookup"><span data-stu-id="3e56b-139">**Graph Explorer sample query**</span></span> | <span data-ttu-id="3e56b-140">**набор средств примере URL-адреса iFrame**</span><span class="sxs-lookup"><span data-stu-id="3e56b-140">**Toolkit sample iFrame URL**</span></span> |
| --- | --- |
| <span data-ttu-id="3e56b-141">GET мой профиль</span><span class="sxs-lookup"><span data-stu-id="3e56b-141">GET my profile</span></span> | [<span data-ttu-id="3e56b-142"> https://mgt.dev/iframe.html?id=components-mgt-person-card- person-card-hover</span><span class="sxs-lookup"><span data-stu-id="3e56b-142">https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| <span data-ttu-id="3e56b-143">Get people I work with</span><span class="sxs-lookup"><span data-stu-id="3e56b-143">GET people I work with</span></span> | [<span data-ttu-id="3e56b-144"> https://mgt.dev/iframe.html?id=components-mgt-people— people</span><span class="sxs-lookup"><span data-stu-id="3e56b-144">https://mgt.dev/iframe.html?id=components-mgt-people—people</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| <span data-ttu-id="3e56b-145">GET все мои задачи планировщика</span><span class="sxs-lookup"><span data-stu-id="3e56b-145">GET all my planner tasks</span></span> | [<span data-ttu-id="3e56b-146"> https://mgt.dev/iframe.html?id=components-mgt-tasks- tasks</span><span class="sxs-lookup"><span data-stu-id="3e56b-146">https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| <span data-ttu-id="3e56b-147">Get my events for the next week</span><span class="sxs-lookup"><span data-stu-id="3e56b-147">GET my events for the next week</span></span> | [<span data-ttu-id="3e56b-148"> https://mgt.dev/iframe.html?id=components-mgt-agenda— get-events-for-next-week</span><span class="sxs-lookup"><span data-stu-id="3e56b-148">https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| <span data-ttu-id="3e56b-149">Получение своей фотографии</span><span class="sxs-lookup"><span data-stu-id="3e56b-149">GET my photo</span></span> | [<span data-ttu-id="3e56b-150"> https://mgt.dev/iframe.html?id=components-mgt-person— только для фото человека</span><span class="sxs-lookup"><span data-stu-id="3e56b-150">https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Screenshot showing the набор средств components tab with the code to generate the component highlighted](./images/graph-toolkit.png)

### <a name="adaptive-cards-integration"></a><span data-ttu-id="3e56b-152">Интеграция адаптивных карточек</span><span class="sxs-lookup"><span data-stu-id="3e56b-152">Adaptive cards integration</span></span>

<span data-ttu-id="3e56b-153">[Адаптивные карточки](https://adaptivecards.io/) — это не зависит от платформы фрагменты пользовательского интерфейса, авторские в JSON, которые приложения и службы могут открыто обмениваться.</span><span class="sxs-lookup"><span data-stu-id="3e56b-153">[Adaptive cards](https://adaptivecards.io/) are platform-agnostic snippets of UI, authored in JSON, that apps and services can openly exchange.</span></span> <span data-ttu-id="3e56b-154">При запуске запроса и наличии адаптивной карточки на вкладке адаптивных карт появляется синяя **точка.**</span><span class="sxs-lookup"><span data-stu-id="3e56b-154">When you run a query and an adaptive card is available, a blue dot appears on the **Adaptive cards** tab.</span></span>

![Screenshot of the adaptive cards tab in Graph Explorer with the response details highlighted](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a><span data-ttu-id="3e56b-156">Настройка темы в обозревателе Graph</span><span class="sxs-lookup"><span data-stu-id="3e56b-156">Customize the theme in Graph Explorer</span></span>

<span data-ttu-id="3e56b-157">Выберите тему для проводника Graph, выбрав параметр "Изменить **тему"** под шестеренкой параметров.</span><span class="sxs-lookup"><span data-stu-id="3e56b-157">Choose the theme for Graph Explorer by selecting the **Change theme** option under the settings gear.</span></span> <span data-ttu-id="3e56b-158">Параметры темы: Light, Dark и High contrast.</span><span class="sxs-lookup"><span data-stu-id="3e56b-158">Theme options are Light, Dark, and High contrast.</span></span>

![Снимок экрана: параметр "Изменить тему" в обозревателе Graph с выделенной темой](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a><span data-ttu-id="3e56b-160">Хранение запросов и совместное использование</span><span class="sxs-lookup"><span data-stu-id="3e56b-160">Storing and sharing queries</span></span>

<span data-ttu-id="3e56b-161">Запросы, которые запускаются в проводнике Graph, сохраняются в течение 30 дней на вкладке **"История".** На вкладке "История" можно:</span><span class="sxs-lookup"><span data-stu-id="3e56b-161">Queries run in Graph Explorer are saved for 30 days in the **History** tab. On the History tab, you can:</span></span>

1.  <span data-ttu-id="3e56b-162">Экспортировать все элементы истории в формате .har.</span><span class="sxs-lookup"><span data-stu-id="3e56b-162">Export all history items in .har format.</span></span>
2.  <span data-ttu-id="3e56b-163">Удаление всех элементов истории.</span><span class="sxs-lookup"><span data-stu-id="3e56b-163">Delete all history items.</span></span>
3.  <span data-ttu-id="3e56b-164">Просмотр этого элемента истории.</span><span class="sxs-lookup"><span data-stu-id="3e56b-164">View this history item.</span></span>
4.  <span data-ttu-id="3e56b-165">Запустите этот запрос.</span><span class="sxs-lookup"><span data-stu-id="3e56b-165">Run this query.</span></span>
5.  <span data-ttu-id="3e56b-166">Экспортировать этот элемент истории в формате .har.</span><span class="sxs-lookup"><span data-stu-id="3e56b-166">Export this history item in .har format.</span></span>
6.  <span data-ttu-id="3e56b-167">Удалите этот элемент истории.</span><span class="sxs-lookup"><span data-stu-id="3e56b-167">Delete this history item.</span></span>

![Снимок экрана: вкладка "История" с выделенной опцией](./images/storing-and-sharing-queries.png)

<span data-ttu-id="3e56b-169">Чтобы поделиться запросами, нажмите кнопку "Поделиться запросом" в области ответа и нажмите кнопку **"Копировать".**</span><span class="sxs-lookup"><span data-stu-id="3e56b-169">To share queries that you run, click the share query button in the response pane and click **copy**.</span></span> <span data-ttu-id="3e56b-170">Это копирует ссылку для обмена и позволяет другим пользователям видеть ваш запрос и результаты.</span><span class="sxs-lookup"><span data-stu-id="3e56b-170">This copies a link to share and allow others to see your query and the results.</span></span>

![Screenshot of Graph Explorer with the Share and Copy options highlighted](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a><span data-ttu-id="3e56b-172">Функции пользовательского интерфейса проводника Graph</span><span class="sxs-lookup"><span data-stu-id="3e56b-172">Graph Explorer UI features</span></span>

<span data-ttu-id="3e56b-173">Свернуть и развернуть компонент боковой панели в обозревателе Graph, чтобы расширить область запроса и ответа.</span><span class="sxs-lookup"><span data-stu-id="3e56b-173">Collapse and expand the sidebar component in Graph Explorer when you want to widen the request and response area.</span></span> <span data-ttu-id="3e56b-174">Чтобы свернуть компонент боковой панели, выберите значок гамбургера в верхней левой части боковой панели.</span><span class="sxs-lookup"><span data-stu-id="3e56b-174">To collapse the sidebar component, select the hamburger icon on the top left of the sidebar.</span></span>

![Снимок экрана: обозреватель Graph с выделенной опцией расширения и свернутого экрана](./images/expand-collapse-sidebar-component.png)

<span data-ttu-id="3e56b-176">Раз развернуть и свернуть предварительный просмотр отклика, выбрав стрелку расширения в окне предварительного просмотра отклика.</span><span class="sxs-lookup"><span data-stu-id="3e56b-176">Expand and collapse the response preview by selecting the expand arrow in the response preview window.</span></span>

![Screenshot of the response pane with the expand and collapse options highlighted](./images/expand-collapse-response-preview.png)

<span data-ttu-id="3e56b-178">Удобный доступ к сайту программы для разработчиков Microsoft 365 из пользовательского интерфейса песочницы Graph, чтобы получить бесплатную песочницу с примерами данных для экспериментов.</span><span class="sxs-lookup"><span data-stu-id="3e56b-178">Conveniently access the Microsoft 365 Developer Program site from the Graph Explorer UI to get a free sandbox with sample data to experiment with.</span></span> <span data-ttu-id="3e56b-179">Под шестеренкой параметра выберите **"Получить песочницу" с примерами данных.**</span><span class="sxs-lookup"><span data-stu-id="3e56b-179">Under the setting gear, select **Get a sandbox with sample data**.</span></span>

![Screenshot of Graph Explorer with the Get a sandbox with sample data option highlighted](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a><span data-ttu-id="3e56b-181">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3e56b-181">Next steps</span></span>

- <span data-ttu-id="3e56b-182">Посетите [обозреватель Graph и](https://developer.microsoft.com/graph/graph-explorer/) изучите примеры запросов.</span><span class="sxs-lookup"><span data-stu-id="3e56b-182">Visit [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) and explore sample queries.</span></span>
- <span data-ttu-id="3e56b-183">Изучите [документацию по набор средств Microsoft Graph.](/graph/toolkit/overview)</span><span class="sxs-lookup"><span data-stu-id="3e56b-183">Explore the [Microsoft Graph Toolkit documentation](/graph/toolkit/overview).</span></span>
- <span data-ttu-id="3e56b-184">Участие или предоставление отзывов в [репозитарии GitHub в обозревателе Graph.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)</span><span class="sxs-lookup"><span data-stu-id="3e56b-184">Contribute or provide feedback in the [Graph Explorer GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).</span></span>
