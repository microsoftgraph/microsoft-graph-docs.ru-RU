---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 0ef20f80c003d880d25eff00c993bc1800545dc7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952677"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a><span data-ttu-id="6b0f4-103">Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6b0f4-103">Overview of the Microsoft Search API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="6b0f4-104">Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="6b0f4-105">Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="6b0f4-106">Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="6b0f4-107">Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  </span><span class="sxs-lookup"><span data-stu-id="6b0f4-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="6b0f4-108">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="6b0f4-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="6b0f4-109">Единая конечная точка поиска для данных Microsoft Cloud</span><span class="sxs-lookup"><span data-stu-id="6b0f4-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="6b0f4-110">API Поиска (Майкрософт) предоставляет единую конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) в Microsoft Cloud данных (сообщений и событий в почтовых ящиках Outlook, а также файлов в OneDrive и SharePoint), индексированных в Поиске (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="6b0f4-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="6b0f4-111">Включение настраиваемых внешних данных в интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="6b0f4-111">Include custom external data in search experience</span></span>

<span data-ttu-id="6b0f4-112">Используйте [соединители Microsoft Graph](/microsoftsearch/connectors-overview), чтобы включить данные из-за пределов облака Майкрософт в свой интерфейс поиска.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-112">Use [Microsoft Graph connectors](/microsoftsearch/connectors-overview) to include data outside of the Microsoft cloud in your search experience.</span></span> <span data-ttu-id="6b0f4-113">Например, подключитесь к базе данных отдела кадров организации или к каталогу продуктов.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-113">For instance, connect to an organization's human resources database or product catalog.</span></span> <span data-ttu-id="6b0f4-114">Затем используйте API Поиска (Майкрософт), чтобы легко [запросить](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) внешний источник данных.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-114">Then use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) the external data source.</span></span> 

<span data-ttu-id="6b0f4-115">Просмотрите [коллекцию соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы найти готовые к использованию соединители.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-115">Browse the [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) to find ready-to-use connectors.</span></span> <span data-ttu-id="6b0f4-116">Вы также можете [создавать собственные соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), чтобы индексировать внешние настраиваемые элементы и отправлять запросы к определенным внешним источникам данных.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-116">Alternatively, you can [build your own connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases) to index external custom items and query specific external data sources.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="6b0f4-117">Единый актуальный интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="6b0f4-117">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="6b0f4-118">При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-118">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="6b0f4-119">Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-119">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="6b0f4-120">Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="6b0f4-120">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="6b0f4-121">API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:</span><span class="sxs-lookup"><span data-stu-id="6b0f4-121">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span>

- <span data-ttu-id="6b0f4-122">Объекты [сообщений](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) электронной почты и [события](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) календаря Outlook</span><span class="sxs-lookup"><span data-stu-id="6b0f4-122">Outlook email [messages](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) and calendar [events](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) objects</span></span>
- <span data-ttu-id="6b0f4-123">Файлы и папки в SharePoint и OneDrive ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [списки](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) [сайты](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) и [диски.](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="6b0f4-123">SharePoint and OneDrive files and folders ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [lists](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItems](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true), [sites](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) and [drives](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)</span></span>
- <span data-ttu-id="6b0f4-124">Содержимое, отправляемое через платформу Graph Connectors: [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="6b0f4-124">Content ingested throught the Graph Connectors platform : [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span></span>

## <a name="api-reference"></a><span data-ttu-id="6b0f4-125">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="6b0f4-125">API reference</span></span>

<span data-ttu-id="6b0f4-126">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="6b0f4-126">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="6b0f4-127">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="6b0f4-127">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="6b0f4-128">Использование API Поиска (Майкрософт) для индексирования данных</span><span class="sxs-lookup"><span data-stu-id="6b0f4-128">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a><span data-ttu-id="6b0f4-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="6b0f4-129">Next steps</span></span>

- <span data-ttu-id="6b0f4-130">Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="6b0f4-130">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="6b0f4-131">Подробнее о некоторых основных вариантах использования:</span><span class="sxs-lookup"><span data-stu-id="6b0f4-131">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="6b0f4-132">Управление подключениями для индексирования внешнего контента</span><span class="sxs-lookup"><span data-stu-id="6b0f4-132">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="6b0f4-133">Индексирование внешнего контента</span><span class="sxs-lookup"><span data-stu-id="6b0f4-133">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="6b0f4-134">Поиск сообщений Outlook</span><span class="sxs-lookup"><span data-stu-id="6b0f4-134">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="6b0f4-135">Поиск событий календаря</span><span class="sxs-lookup"><span data-stu-id="6b0f4-135">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="6b0f4-136">Поиск содержимого в OneDrive и SharePoint</span><span class="sxs-lookup"><span data-stu-id="6b0f4-136">Search content in Sharepoint and OneDrive</span></span>](search-concept-files.md)
  - [<span data-ttu-id="6b0f4-137">Поиск внешнего контента</span><span class="sxs-lookup"><span data-stu-id="6b0f4-137">Search external content</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="6b0f4-138">Сортировка результатов поиска</span><span class="sxs-lookup"><span data-stu-id="6b0f4-138">Sort search results</span></span>](search-concept-sort.md)
  - [<span data-ttu-id="6b0f4-139">Уточнение результатов поиска</span><span class="sxs-lookup"><span data-stu-id="6b0f4-139">Refine search results</span></span>](search-concept-aggregation.md)
  
- <span data-ttu-id="6b0f4-140">Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6b0f4-140">Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="6b0f4-141">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-141">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="6b0f4-142">См. также</span><span class="sxs-lookup"><span data-stu-id="6b0f4-142">See also</span></span>

- <span data-ttu-id="6b0f4-143">Участвуйте в работе сообщества на [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) или на GitHub.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-143">Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) or on GitHub</span></span>
