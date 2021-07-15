---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 3a6c02b4f70cce4ac44090f5981372096fa17bce
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443128"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a><span data-ttu-id="2071b-103">Обзор API Поиска (Майкрософт) в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2071b-103">Overview of the Microsoft Search API in Microsoft Graph</span></span>

<span data-ttu-id="2071b-104">Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации.</span><span class="sxs-lookup"><span data-stu-id="2071b-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="2071b-105">Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей.</span><span class="sxs-lookup"><span data-stu-id="2071b-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="2071b-106">Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing.</span><span class="sxs-lookup"><span data-stu-id="2071b-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="2071b-107">Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  </span><span class="sxs-lookup"><span data-stu-id="2071b-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>


<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="2071b-108">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="2071b-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="2071b-109">Единая конечная точка поиска для данных Microsoft Cloud</span><span class="sxs-lookup"><span data-stu-id="2071b-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="2071b-110">API Поиска (Майкрософт) предоставляет единую конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query) в Microsoft Cloud данных (сообщений и событий в почтовых ящиках Outlook, а также файлов в OneDrive и SharePoint), индексированных в Поиске (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="2071b-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience-preview"></a><span data-ttu-id="2071b-111">Включение настраиваемых внешних данных в интерфейс поиска (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2071b-111">Include custom external data in search experience (preview)</span></span>

<span data-ttu-id="2071b-112">Используйте [соединители Microsoft Graph](/microsoftsearch/connectors-overview), чтобы включить данные из-за пределов облака Майкрософт в свой интерфейс поиска.</span><span class="sxs-lookup"><span data-stu-id="2071b-112">Use [Microsoft Graph connectors](/microsoftsearch/connectors-overview) to include data outside of the Microsoft cloud in your search experience.</span></span> <span data-ttu-id="2071b-113">Например, подключитесь к базе данных отдела кадров организации или к каталогу продуктов.</span><span class="sxs-lookup"><span data-stu-id="2071b-113">For instance, connect to an organization's human resources database or product catalog.</span></span> <span data-ttu-id="2071b-114">Затем используйте API Поиска (Майкрософт), чтобы легко [запросить](/graph/api/search-query) внешний источник данных.</span><span class="sxs-lookup"><span data-stu-id="2071b-114">Then use the Microsoft Search API to seamlessly [query](/graph/api/search-query) the external data source.</span></span> 

<span data-ttu-id="2071b-115">Просмотрите [коллекцию соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы найти готовые к использованию соединители.</span><span class="sxs-lookup"><span data-stu-id="2071b-115">Browse the [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) to find ready-to-use connectors.</span></span> <span data-ttu-id="2071b-116">Вы также можете [создавать собственные соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), чтобы индексировать внешние настраиваемые элементы и отправлять запросы к определенным внешним источникам данных.</span><span class="sxs-lookup"><span data-stu-id="2071b-116">Alternatively, you can [build your own connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases) to index external custom items and query specific external data sources.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="2071b-117">Единый актуальный интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="2071b-117">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="2071b-118">При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2071b-118">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="2071b-119">Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.</span><span class="sxs-lookup"><span data-stu-id="2071b-119">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="2071b-120">Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="2071b-120">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="2071b-121">API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:</span><span class="sxs-lookup"><span data-stu-id="2071b-121">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span> 

- <span data-ttu-id="2071b-122">Ресурсы [message](/graph/api/resources/message) почты Outlook и [event](/graph/api/resources/event) календаря.</span><span class="sxs-lookup"><span data-stu-id="2071b-122">Outlook email [message](/graph/api/resources/message) and calendar [event](/graph/api/resources/event) resources.</span></span>
- <span data-ttu-id="2071b-123">Файлы и папки в SharePoint и OneDrive (ресурсы [driveItem](/graph/api/resources/driveitem)), ресурсы [list](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site) и [drive](/graph/api/resources/drive).</span><span class="sxs-lookup"><span data-stu-id="2071b-123">SharePoint and OneDrive files and folders ([driveItem](/graph/api/resources/driveitem) resources), [list](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site), and [drive](/graph/api/resources/drive) resources.</span></span>
- <span data-ttu-id="2071b-124">Ресурсы [person](/graph/api/resources/person) в организации, наиболее релевантные для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2071b-124">[Person](/graph/api/resources/person) resources in an organization who are most relevant to a user.</span></span>
- <span data-ttu-id="2071b-125">Содержимое, отправляемое через платформу соединителей Microsoft Graph: ресурсы [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="2071b-125">Content ingested through the Microsoft Graph connectors platform : [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) resources.</span></span>

## <a name="api-reference"></a><span data-ttu-id="2071b-126">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="2071b-126">API reference</span></span>

<span data-ttu-id="2071b-127">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="2071b-127">Looking for the API reference for this service?</span></span>

- <span data-ttu-id="2071b-128">[Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true)(версия 1.0)</span><span class="sxs-lookup"><span data-stu-id="2071b-128">[Use the Microsoft Search API to query data](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true) (v1.0)</span></span>
- <span data-ttu-id="2071b-129">[Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)(предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2071b-129">[Use the Microsoft Search API to query data](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) (preview)</span></span>
- <span data-ttu-id="2071b-130">[Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2071b-130">[Use the Microsoft Search API to index data](/graph/api/resources/indexing-api-overview) (preview)</span></span>

## <a name="next-steps"></a><span data-ttu-id="2071b-131">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2071b-131">Next steps</span></span>

- <span data-ttu-id="2071b-132">Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="2071b-132">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="2071b-133">Подробнее о некоторых основных вариантах использования:</span><span class="sxs-lookup"><span data-stu-id="2071b-133">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="2071b-134">Управление подключениями для индексирования внешнего контента</span><span class="sxs-lookup"><span data-stu-id="2071b-134">Manage connections to index external content</span></span>](connecting-external-content-manage-connections.md)
  - [<span data-ttu-id="2071b-135">Индексирование внешнего контента</span><span class="sxs-lookup"><span data-stu-id="2071b-135">Index external content</span></span>](connecting-external-content-manage-items.md)
  - [<span data-ttu-id="2071b-136">Поиск сообщений Outlook</span><span class="sxs-lookup"><span data-stu-id="2071b-136">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="2071b-137">Поиск событий календаря</span><span class="sxs-lookup"><span data-stu-id="2071b-137">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="2071b-138">Поиск содержимого в OneDrive и SharePoint</span><span class="sxs-lookup"><span data-stu-id="2071b-138">Search content in Sharepoint and OneDrive</span></span>](search-concept-files.md)
  - [<span data-ttu-id="2071b-139">Поиск внешнего контента</span><span class="sxs-lookup"><span data-stu-id="2071b-139">Search external content</span></span>](search-concept-custom-types.md)
  - <span data-ttu-id="2071b-140">[Поиск человека](search-concept-person.md) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2071b-140">[Search person](search-concept-person.md) (preview)</span></span>
  - <span data-ttu-id="2071b-141">[Сортировка результатов поиска](search-concept-sort.md) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2071b-141">[Sort search results](search-concept-sort.md) (preview)</span></span>
  - <span data-ttu-id="2071b-142">[Уточнение результатов поиска](search-concept-aggregation.md) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2071b-142">[Refine search results](search-concept-aggregation.md) (preview)</span></span>
  - <span data-ttu-id="2071b-143">[Исправление орфографии в запросе](search-concept-speller.md) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2071b-143">[Request spelling correction](search-concept-speller.md) (preview)</span></span>
  - <span data-ttu-id="2071b-144">[Макет отображения при поиске](search-concept-display-layout.md) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2071b-144">[Search display layout](search-concept-display-layout.md) (preview)</span></span>
 
  
- <span data-ttu-id="2071b-145">Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="2071b-145">Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="2071b-146">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.</span><span class="sxs-lookup"><span data-stu-id="2071b-146">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="2071b-147">См. также</span><span class="sxs-lookup"><span data-stu-id="2071b-147">See also</span></span>

- <span data-ttu-id="2071b-148">Участвуйте в работе сообщества на сайте [Вопросы и ответы Майкрософт](/answers/products/m365#microsoft-graph) или на GitHub.</span><span class="sxs-lookup"><span data-stu-id="2071b-148">Engage with the community on [Microsoft Q&A](/answers/products/m365#microsoft-graph)  or on GitHub</span></span>
