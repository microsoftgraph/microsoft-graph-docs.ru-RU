---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: d4c16bd0175f8ae0cd9d8e03f549bea9eff3db63
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373505"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a><span data-ttu-id="2cc89-103">Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2cc89-103">Overview of the Microsoft Search API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="2cc89-104">Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации.</span><span class="sxs-lookup"><span data-stu-id="2cc89-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="2cc89-105">Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей.</span><span class="sxs-lookup"><span data-stu-id="2cc89-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="2cc89-106">Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing.</span><span class="sxs-lookup"><span data-stu-id="2cc89-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="2cc89-107">Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  </span><span class="sxs-lookup"><span data-stu-id="2cc89-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="2cc89-108">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="2cc89-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="2cc89-109">Единая конечная точка поиска для данных Microsoft Cloud</span><span class="sxs-lookup"><span data-stu-id="2cc89-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="2cc89-110">API Поиска (Майкрософт) предоставляет единую конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) в Microsoft Cloud данных (сообщений и событий в почтовых ящиках Outlook, а также файлов в OneDrive и SharePoint), индексированных в Поиске (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="2cc89-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="2cc89-111">Включение настраиваемых внешних данных в интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="2cc89-111">Include custom external data in search experience</span></span>

<span data-ttu-id="2cc89-112">Пользователи, желающие включить в свой поиск данные, не входящие в Microsoft Cloud, могут использовать [соединители](/microsoftsearch/connectors-overview), чтобы подключиться к определенному источнику данных, такому как база данных отдела кадров организации или каталог продуктов, и использовать API Поиска (Майкрософт) для [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) внешнего источника данных.</span><span class="sxs-lookup"><span data-stu-id="2cc89-112">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) the external data source.</span></span> <span data-ttu-id="2cc89-113">[Коллекция соединителей Microsoft Graph](/microsoftsearch/connectors-gallery) включает ряд готовых к использованию соединителей.</span><span class="sxs-lookup"><span data-stu-id="2cc89-113">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="2cc89-114">Пользователи также могут [создавать соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), индексировать внешние настраиваемые элементы и запрашивать определенные внешние источники данных.</span><span class="sxs-lookup"><span data-stu-id="2cc89-114">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), index external custom items, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="2cc89-115">Единый актуальный интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="2cc89-115">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="2cc89-116">При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2cc89-116">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="2cc89-117">Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.</span><span class="sxs-lookup"><span data-stu-id="2cc89-117">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="2cc89-118">Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="2cc89-118">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="2cc89-119">API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:</span><span class="sxs-lookup"><span data-stu-id="2cc89-119">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span>

- <span data-ttu-id="2cc89-120">Объекты [сообщений](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) электронной почты и [события](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) календаря Outlook</span><span class="sxs-lookup"><span data-stu-id="2cc89-120">Outlook email [messages](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) and calendar [events](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) objects</span></span>
- <span data-ttu-id="2cc89-121">Файлы и папки в SharePoint и OneDrive ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [списки](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) [сайты](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) и [диски.](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="2cc89-121">SharePoint and OneDrive files and folders ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [lists](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItems](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true), [sites](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) and [drives](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)</span></span>
- <span data-ttu-id="2cc89-122">Содержимое, отправляемое через платформу Graph Connectors: [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="2cc89-122">Content ingested throught the Graph Connectors platform : [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span></span>

## <a name="api-reference"></a><span data-ttu-id="2cc89-123">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="2cc89-123">API reference</span></span>

<span data-ttu-id="2cc89-124">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="2cc89-124">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="2cc89-125">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="2cc89-125">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="2cc89-126">Использование API Поиска (Майкрософт) для индексирования данных</span><span class="sxs-lookup"><span data-stu-id="2cc89-126">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a><span data-ttu-id="2cc89-127">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2cc89-127">Next steps</span></span>

- <span data-ttu-id="2cc89-128">Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="2cc89-128">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="2cc89-129">Подробнее о некоторых основных вариантах использования:</span><span class="sxs-lookup"><span data-stu-id="2cc89-129">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="2cc89-130">Управление подключениями для индексирования внешнего контента</span><span class="sxs-lookup"><span data-stu-id="2cc89-130">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="2cc89-131">Индексирование внешнего контента</span><span class="sxs-lookup"><span data-stu-id="2cc89-131">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="2cc89-132">Поиск сообщений Outlook</span><span class="sxs-lookup"><span data-stu-id="2cc89-132">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="2cc89-133">Поиск событий календаря</span><span class="sxs-lookup"><span data-stu-id="2cc89-133">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="2cc89-134">Поиск содержимого в OneDrive и SharePoint</span><span class="sxs-lookup"><span data-stu-id="2cc89-134">Search content in Sharepoint and OneDrive</span></span>](search-concept-files.md)
  - [<span data-ttu-id="2cc89-135">Поиск внешнего контента</span><span class="sxs-lookup"><span data-stu-id="2cc89-135">Search external content</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="2cc89-136">Сортировка результатов поиска</span><span class="sxs-lookup"><span data-stu-id="2cc89-136">Sort search results</span></span>](search-concept-sort.md)
  - [<span data-ttu-id="2cc89-137">Уточнение результатов поиска</span><span class="sxs-lookup"><span data-stu-id="2cc89-137">Refine search results</span></span>](search-concept-aggregation.md)
  
- <span data-ttu-id="2cc89-138">Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="2cc89-138">Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="2cc89-139">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.</span><span class="sxs-lookup"><span data-stu-id="2cc89-139">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="2cc89-140">См. также</span><span class="sxs-lookup"><span data-stu-id="2cc89-140">See also</span></span>

- <span data-ttu-id="2cc89-141">Участвуйте в работе сообщества на [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) или на GitHub.</span><span class="sxs-lookup"><span data-stu-id="2cc89-141">Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) or on GitHub</span></span>
