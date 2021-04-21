---
title: Работа с Graph Explorer
description: Узнайте, как использовать некоторые важные функции в Graph Explorer.
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: a0a6ce380942d6677877c65ac20242d3b3ad37fa
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921135"
---
# <a name="working-with-graph-explorer"></a><span data-ttu-id="c2323-103">Работа с Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="c2323-103">Working with Graph Explorer</span></span>

<span data-ttu-id="c2323-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) — это средство разработчика, которое позволяет удобно делать запросы API API Для Microsoft Graph REST и просматривать соответствующие ответы.</span><span class="sxs-lookup"><span data-stu-id="c2323-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) is a developer tool that lets you conveniently make Microsoft Graph REST API requests and view corresponding responses.</span></span> <span data-ttu-id="c2323-105">В этой статье описывается использование некоторых важных функций в Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="c2323-105">This article describes how to use some of the important features in Graph Explorer.</span></span>

## <a name="consent-to-permissions"></a><span data-ttu-id="c2323-106">Согласие на разрешения</span><span class="sxs-lookup"><span data-stu-id="c2323-106">Consent to permissions</span></span>

<span data-ttu-id="c2323-107">Пользователь или администратор должны предоставить Graph Explorer правильные разрешения с помощью процесса согласия для доступа к данным в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2323-107">The user or administrator must grant Graph Explorer the correct permissions via a consent process to access data in Microsoft Graph.</span></span> <span data-ttu-id="c2323-108">Согласие на разрешения в Graph Explorer либо с помощью вкладки **Изменение** разрешений, либо параметра **Select permissions** в шестеренке параметров рядом с профилем при вписке.</span><span class="sxs-lookup"><span data-stu-id="c2323-108">Consent to permissions in Graph Explorer either via the **Modify permissions** tab or the **Select permissions** option in the settings gear next to your profile when you’re signed in.</span></span> <span data-ttu-id="c2323-109">На **вкладке Изменение** разрешений перечислены все разрешения, необходимые для выполнения запроса в панели адресов.</span><span class="sxs-lookup"><span data-stu-id="c2323-109">The **Modify permissions** tab lists all permissions you need to run the query in the address bar.</span></span> 

<span data-ttu-id="c2323-110">Согласие на разрешения:</span><span class="sxs-lookup"><span data-stu-id="c2323-110">To consent to permissions:</span></span>

1.  <span data-ttu-id="c2323-111">Выберите пример запроса и запустите его.</span><span class="sxs-lookup"><span data-stu-id="c2323-111">Select a sample query and run it.</span></span>
2.  <span data-ttu-id="c2323-112">Выберите **вкладку Изменение разрешений.**</span><span class="sxs-lookup"><span data-stu-id="c2323-112">Select the **Modify permissions** tab.</span></span>
3.  <span data-ttu-id="c2323-113">Список разрешений, необходимых для выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="c2323-113">See the list of permissions required to run the query.</span></span>
4.  <span data-ttu-id="c2323-114">Выберите кнопку согласия рядом с разрешением, на который требуется согласие.</span><span class="sxs-lookup"><span data-stu-id="c2323-114">Select the consent button next to the permission you want to consent to.</span></span> 

![Снимок экрана обозревателя graph с шагами для согласия на выделенные разрешения](./images/modify-permissions.png)

<span data-ttu-id="c2323-116">Функция **Изменение разрешений** в настоящее время находится в предварительном просмотре, и некоторые запросы могут быть отсутствуют разрешения.</span><span class="sxs-lookup"><span data-stu-id="c2323-116">The **Modify  permissions** feature is currently in preview, and some queries might be missing permissions.</span></span> <span data-ttu-id="c2323-117">Если для запроса отсутствуют разрешения, параметр **Select permissions** в шестеренки параметров рядом с профилем содержит список всех доступных разрешений:</span><span class="sxs-lookup"><span data-stu-id="c2323-117">If permissions are missing for a query, the **Select permissions** option in the settings gear next to your profile contains the list of all available permissions:</span></span>

1.  <span data-ttu-id="c2323-118">Перейдите к шестеренку параметров и нажмите кнопку **Выбор разрешений.**</span><span class="sxs-lookup"><span data-stu-id="c2323-118">Go the settings gear and click the **Select permissions** option.</span></span> <span data-ttu-id="c2323-119">Этот параметр содержит список всех доступных разрешений.</span><span class="sxs-lookup"><span data-stu-id="c2323-119">This option contains the list of all available permissions.</span></span>
2.  <span data-ttu-id="c2323-120">Из списка всех разрешений, согласие на те, которые вы хотите.</span><span class="sxs-lookup"><span data-stu-id="c2323-120">From the list of all the permissions, consent to the ones you want.</span></span>

![Снимок экрана обозревателя graph с выделенной опцией Выбор разрешений](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a><span data-ttu-id="c2323-122">Получить маркер доступа или проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="c2323-122">Get an access or authentication token</span></span>

<span data-ttu-id="c2323-123">Graph Explorer включает вкладку **маркера Access,** которая показывает маркер доступа при входе.</span><span class="sxs-lookup"><span data-stu-id="c2323-123">Graph Explorer includes an **Access token** tab that shows your access token when you are signed in.</span></span> <span data-ttu-id="c2323-124">На **вкладке Маркер Доступа** можно скопировать маркер, если необходимо использовать его в любимом клиентской приложении REST.</span><span class="sxs-lookup"><span data-stu-id="c2323-124">On the **Access token** tab, you can copy the token if you need to use it in your favorite REST client application.</span></span>

![Снимок экрана вкладки маркера Access в Graph Explorer с выделенной кнопкой Копирование](./images/access-token.png)

## <a name="copy-code-snippets"></a><span data-ttu-id="c2323-126">Фрагменты кода копирования</span><span class="sxs-lookup"><span data-stu-id="c2323-126">Copy code snippets</span></span>

<span data-ttu-id="c2323-127">Для каждого запроса API REST, который вы выбираете или вводите в Graph Explorer, вы  можете найти способ вызова этого API на каждом из четырех языков, демонстрируемого на вкладке фрагментов кода — C#, Java, JavaScript и Objective-C.</span><span class="sxs-lookup"><span data-stu-id="c2323-127">For each REST API query you select or enter in Graph Explorer, you can find how to call that API in each of the four languages showcased under the **Code snippets** tab - C#, Java, JavaScript, and Objective-C.</span></span> 

![Снимок экрана обозревателя graph с выделенной вкладке фрагментов кода](./images/code-snippets.png)

## <a name="ui-component-integration"></a><span data-ttu-id="c2323-129">Интеграция компонентов пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="c2323-129">UI component integration</span></span>

<span data-ttu-id="c2323-130">Graph Explorer включает несколько функций, упрощающих реализацию пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c2323-130">Graph Explorer includes several features to make implementing UI easier.</span></span> <span data-ttu-id="c2323-131">Повторное использование этих компонентов и в приложениях.</span><span class="sxs-lookup"><span data-stu-id="c2323-131">Reuse these components in your apps too.</span></span>

### <a name="microsoft-graph-toolkit-integration"></a><span data-ttu-id="c2323-132">Интеграция microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="c2323-132">Microsoft Graph Toolkit integration</span></span>

<span data-ttu-id="c2323-133">Веб-набор средств Microsoft [Graph —](../toolkit/overview.md) это коллекция многоиспользоваемых веб-компонентов и помощников для доступа и работы с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2323-133">The [Microsoft Graph Toolkit](../toolkit/overview.md) is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="c2323-134">Компоненты полностью функциональны, встроенные в поставщиков, которые аутентификация и извлечение данных из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2323-134">The components are fully functional, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="c2323-135">Graph Explorer предоставляет примеры запросов API REST, которые соответствуют компонентам Microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="c2323-135">Graph Explorer provides sample REST API queries that correspond to Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="c2323-136">Синяя точка на вкладке **набор средств** указывает, что набор средств предоставляет компонент для указанного в настоящее время запроса API REST в Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="c2323-136">A blue dot on the **Toolkit component** tab indicates that the Toolkit provides a component for the currently specified REST API query in Graph Explorer.</span></span> <span data-ttu-id="c2323-137">Код компонента можно удобно скопировать в приложении.</span><span class="sxs-lookup"><span data-stu-id="c2323-137">You can conveniently copy the code for the component to your app.</span></span>

<span data-ttu-id="c2323-138">В следующей таблице перечислены примеры запросов, которые в настоящее время включают набор средств компонент.</span><span class="sxs-lookup"><span data-stu-id="c2323-138">The following table lists the sample queries that currently include a Toolkit component.</span></span>

| <span data-ttu-id="c2323-139">**Пример запроса Graph Explorer**</span><span class="sxs-lookup"><span data-stu-id="c2323-139">**Graph Explorer sample query**</span></span> | <span data-ttu-id="c2323-140">**набор средств URL-адрес iFrame**</span><span class="sxs-lookup"><span data-stu-id="c2323-140">**Toolkit sample iFrame URL**</span></span> |
| --- | --- |
| <span data-ttu-id="c2323-141">GET мой профиль</span><span class="sxs-lookup"><span data-stu-id="c2323-141">GET my profile</span></span> | [<span data-ttu-id="c2323-142"> https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover</span><span class="sxs-lookup"><span data-stu-id="c2323-142">https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| <span data-ttu-id="c2323-143">GET people I work with</span><span class="sxs-lookup"><span data-stu-id="c2323-143">GET people I work with</span></span> | [<span data-ttu-id="c2323-144"> https://mgt.dev/iframe.html?id=components-mgt-people—люди</span><span class="sxs-lookup"><span data-stu-id="c2323-144">https://mgt.dev/iframe.html?id=components-mgt-people—people</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| <span data-ttu-id="c2323-145">GET all my planner tasks</span><span class="sxs-lookup"><span data-stu-id="c2323-145">GET all my planner tasks</span></span> | [<span data-ttu-id="c2323-146"> https://mgt.dev/iframe.html?id=components-mgt-tasks— задачи</span><span class="sxs-lookup"><span data-stu-id="c2323-146">https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| <span data-ttu-id="c2323-147">Get my events for the next week</span><span class="sxs-lookup"><span data-stu-id="c2323-147">GET my events for the next week</span></span> | [<span data-ttu-id="c2323-148"> https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week</span><span class="sxs-lookup"><span data-stu-id="c2323-148">https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| <span data-ttu-id="c2323-149">Получение своей фотографии</span><span class="sxs-lookup"><span data-stu-id="c2323-149">GET my photo</span></span> | [<span data-ttu-id="c2323-150"> https://mgt.dev/iframe.html?id=components-mgt-person—только для фотографий</span><span class="sxs-lookup"><span data-stu-id="c2323-150">https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Снимок экрана, показывающий вкладку набор средств компонентов с кодом для создания выделенного компонента](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a><span data-ttu-id="c2323-152">Интеграция адаптивных карт</span><span class="sxs-lookup"><span data-stu-id="c2323-152">Adaptive cards integration</span></span>

<span data-ttu-id="c2323-153">[Адаптивные карточки](https://adaptivecards.io/) — это фрагменты пользовательского интерфейса с платформой агностика, автором которой является JSON, которые приложения и службы могут открыто обмениваться.</span><span class="sxs-lookup"><span data-stu-id="c2323-153">[Adaptive cards](https://adaptivecards.io/) are platform-agnostic snippets of UI, authored in JSON, that apps and services can openly exchange.</span></span> <span data-ttu-id="c2323-154">При запуске запроса и доступной адаптивной карты на вкладке **Адаптивные** карты появляется синяя точка.</span><span class="sxs-lookup"><span data-stu-id="c2323-154">When you run a query and an adaptive card is available, a blue dot appears on the **Adaptive cards** tab.</span></span>

![Снимок экрана вкладки адаптивных карт в Graph Explorer с выделенными деталями ответа](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a><span data-ttu-id="c2323-156">Настройка темы в Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="c2323-156">Customize the theme in Graph Explorer</span></span>

<span data-ttu-id="c2323-157">Выберите тему для Graph Explorer, выбрав параметр **Change theme** под шестеренкой параметров.</span><span class="sxs-lookup"><span data-stu-id="c2323-157">Choose the theme for Graph Explorer by selecting the **Change theme** option under the settings gear.</span></span> <span data-ttu-id="c2323-158">Параметры темы : светлый, темный и высокий контраст.</span><span class="sxs-lookup"><span data-stu-id="c2323-158">Theme options are Light, Dark, and High contrast.</span></span>

![Снимок экрана параметра Изменение темы в Graph Explorer с выделенными вариантами темы](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a><span data-ttu-id="c2323-160">Хранение и общий доступ к запросам</span><span class="sxs-lookup"><span data-stu-id="c2323-160">Storing and sharing queries</span></span>

<span data-ttu-id="c2323-161">Запросы, которые запускаются в Graph Explorer, сохраняются в течение 30 дней на **вкладке История.** На вкладке История можно:</span><span class="sxs-lookup"><span data-stu-id="c2323-161">Queries run in Graph Explorer are saved for 30 days in the **History** tab. On the History tab, you can:</span></span>

1.  <span data-ttu-id="c2323-162">Экспорт всех элементов истории в формате .har.</span><span class="sxs-lookup"><span data-stu-id="c2323-162">Export all history items in .har format.</span></span>
2.  <span data-ttu-id="c2323-163">Удаление всех элементов истории.</span><span class="sxs-lookup"><span data-stu-id="c2323-163">Delete all history items.</span></span>
3.  <span data-ttu-id="c2323-164">Просмотр этого элемента истории.</span><span class="sxs-lookup"><span data-stu-id="c2323-164">View this history item.</span></span>
4.  <span data-ttu-id="c2323-165">Запустите этот запрос.</span><span class="sxs-lookup"><span data-stu-id="c2323-165">Run this query.</span></span>
5.  <span data-ttu-id="c2323-166">Экспорт этого элемента истории в формате .har.</span><span class="sxs-lookup"><span data-stu-id="c2323-166">Export this history item in .har format.</span></span>
6.  <span data-ttu-id="c2323-167">Удалите этот элемент истории.</span><span class="sxs-lookup"><span data-stu-id="c2323-167">Delete this history item.</span></span>

![Снимок экрана вкладки История с выделенными опциями](./images/storing-and-sharing-queries.png)

<span data-ttu-id="c2323-169">Чтобы обмениваться запросами, которые вы запустите, щелкните кнопку запроса share в области ответа и щелкните **скопировать**.</span><span class="sxs-lookup"><span data-stu-id="c2323-169">To share queries that you run, click the share query button in the response pane and click **copy**.</span></span> <span data-ttu-id="c2323-170">Это копирует ссылку для обмена данными и позволяет другим пользователям видеть ваш запрос и результаты.</span><span class="sxs-lookup"><span data-stu-id="c2323-170">This copies a link to share and allow others to see your query and the results.</span></span>

![Снимок экрана обозревателя graph с выделенными вариантами Share и Copy](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a><span data-ttu-id="c2323-172">Функции пользовательского интерфейса Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="c2323-172">Graph Explorer UI features</span></span>

<span data-ttu-id="c2323-173">Обрушение и расширение компонента боковой панели в Graph Explorer при расширении области запроса и ответа.</span><span class="sxs-lookup"><span data-stu-id="c2323-173">Collapse and expand the sidebar component in Graph Explorer when you want to widen the request and response area.</span></span> <span data-ttu-id="c2323-174">Чтобы свернуть компонент боковой панели, выберите значок гамбургера в верхней левой части боковой панели.</span><span class="sxs-lookup"><span data-stu-id="c2323-174">To collapse the sidebar component, select the hamburger icon on the top left of the sidebar.</span></span>

![Снимок экрана обозревателя graph с выделенными вариантами расширения и коллапса](./images/expand-collapse-sidebar-component.png)

<span data-ttu-id="c2323-176">Расширь и обрушив предварительный просмотр ответа, выбрав стрелку расширения в окне предварительного просмотра отклика.</span><span class="sxs-lookup"><span data-stu-id="c2323-176">Expand and collapse the response preview by selecting the expand arrow in the response preview window.</span></span>

![Снимок экрана области отклика с выделенными вариантами расширения и коллапса](./images/expand-collapse-response-preview.png)

<span data-ttu-id="c2323-178">Удобный доступ к сайту программы разработчиков Microsoft 365 из пользовательского интерфейса Graph Explorer, чтобы получить бесплатную песочницу с примерами данных для экспериментов.</span><span class="sxs-lookup"><span data-stu-id="c2323-178">Conveniently access the Microsoft 365 Developer Program site from the Graph Explorer UI to get a free sandbox with sample data to experiment with.</span></span> <span data-ttu-id="c2323-179">В настройках выберите **"Получить песочницу" с примерными данными.**</span><span class="sxs-lookup"><span data-stu-id="c2323-179">Under the setting gear, select **Get a sandbox with sample data**.</span></span>

![Снимок экрана обозревателя графа с помощью "Получить песочницу" с выделенным параметром выборки данных](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a><span data-ttu-id="c2323-181">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="c2323-181">Next steps</span></span>

- <span data-ttu-id="c2323-182">Посетите [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) и изучите примеры запросов.</span><span class="sxs-lookup"><span data-stu-id="c2323-182">Visit [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) and explore sample queries.</span></span>
- <span data-ttu-id="c2323-183">Ознакомьтесь с [документацией по набор средств Microsoft Graph.](../toolkit/overview.md)</span><span class="sxs-lookup"><span data-stu-id="c2323-183">Explore the [Microsoft Graph Toolkit documentation](../toolkit/overview.md).</span></span>
- <span data-ttu-id="c2323-184">Внести или предоставить обратную связь в [репо Graph Explorer GitHub](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="c2323-184">Contribute or provide feedback in the [Graph Explorer GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).</span></span>