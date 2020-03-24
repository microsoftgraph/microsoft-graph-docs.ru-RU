---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 76cc0a1e9b8ccd7ec3eef1fb9ddf7e381b0fd19b
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892795"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a><span data-ttu-id="53d33-103">Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="53d33-103">Overview of the Microsoft Search API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="53d33-104">Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации.</span><span class="sxs-lookup"><span data-stu-id="53d33-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="53d33-105">Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей.</span><span class="sxs-lookup"><span data-stu-id="53d33-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="53d33-106">Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing.</span><span class="sxs-lookup"><span data-stu-id="53d33-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="53d33-107">Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  </span><span class="sxs-lookup"><span data-stu-id="53d33-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="53d33-108">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="53d33-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="53d33-109">Единая конечная точка поиска для данных Microsoft Cloud</span><span class="sxs-lookup"><span data-stu-id="53d33-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="53d33-110">API Поиска (Майкрософт) предоставляет единую конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query?view=graph-rest-beta) в Microsoft Cloud данных (сообщений и событий в почтовых ящиках Outlook, а также файлов в OneDrive и SharePoint), индексированных в Поиске (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="53d33-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query?view=graph-rest-beta) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="53d33-111">Включение настраиваемых внешних данных в интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="53d33-111">Include custom external data in search experience</span></span>

<span data-ttu-id="53d33-112">Пользователи, желающие включить в свой поиск данные, не входящие в Microsoft Cloud, могут использовать [соединители](/microsoftsearch/connectors-overview), чтобы подключиться к определенному источнику данных, такому как база данных отдела кадров организации или каталог продуктов, и использовать API Поиска (Майкрософт) для [запроса](/graph/api/search-query?view=graph-rest-beta) внешнего источника данных.</span><span class="sxs-lookup"><span data-stu-id="53d33-112">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta) the external data source.</span></span> <span data-ttu-id="53d33-113">[Коллекция соединителей Microsoft Graph](/microsoftsearch/connectors-gallery) включает ряд готовых к использованию соединителей.</span><span class="sxs-lookup"><span data-stu-id="53d33-113">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="53d33-114">Пользователи также могут [создавать соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), индексировать внешние настраиваемые элементы и запрашивать определенные внешние источники данных.</span><span class="sxs-lookup"><span data-stu-id="53d33-114">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), index external custom items, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="53d33-115">Единый актуальный интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="53d33-115">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="53d33-116">При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="53d33-116">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="53d33-117">Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.</span><span class="sxs-lookup"><span data-stu-id="53d33-117">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="53d33-118">Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="53d33-118">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="53d33-119">API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:</span><span class="sxs-lookup"><span data-stu-id="53d33-119">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span>

- <span data-ttu-id="53d33-120">Объекты [message](/graph/api/resources/message?view=graph-rest-beta) и [event](/graph/api/resources/event?view=graph-rest-beta) в Outlook</span><span class="sxs-lookup"><span data-stu-id="53d33-120">Outlook [message](/graph/api/resources/message?view=graph-rest-beta) and [event](/graph/api/resources/event?view=graph-rest-beta) objects</span></span>
- <span data-ttu-id="53d33-121">Файловые объекты [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) в SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="53d33-121">SharePoint and OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) file objects</span></span>

<span data-ttu-id="53d33-122">Кроме того, вы можете индексировать и искать внешний контент, используя объект [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="53d33-122">In addition, you can index and search external content via the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) object.</span></span>

## <a name="api-reference"></a><span data-ttu-id="53d33-123">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="53d33-123">API reference</span></span>

<span data-ttu-id="53d33-124">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="53d33-124">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="53d33-125">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="53d33-125">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="53d33-126">Использование API Поиска (Майкрософт) для индексирования данных</span><span class="sxs-lookup"><span data-stu-id="53d33-126">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="53d33-127">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="53d33-127">Next steps</span></span>

- <span data-ttu-id="53d33-128">Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="53d33-128">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="53d33-129">Подробнее о некоторых основных вариантах использования:</span><span class="sxs-lookup"><span data-stu-id="53d33-129">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="53d33-130">Поиск сообщений Outlook</span><span class="sxs-lookup"><span data-stu-id="53d33-130">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="53d33-131">Поиск событий календаря</span><span class="sxs-lookup"><span data-stu-id="53d33-131">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="53d33-132">Управление подключениями для индексирования внешнего контента</span><span class="sxs-lookup"><span data-stu-id="53d33-132">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="53d33-133">Индексирование внешнего контента</span><span class="sxs-lookup"><span data-stu-id="53d33-133">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="53d33-134">Поиск объектов настраиваемого типа (externalItem)</span><span class="sxs-lookup"><span data-stu-id="53d33-134">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="53d33-135">Поиск файлов (включая externalFile)</span><span class="sxs-lookup"><span data-stu-id="53d33-135">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="53d33-136">Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="53d33-136">Explore the search APIs in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="53d33-137">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.</span><span class="sxs-lookup"><span data-stu-id="53d33-137">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="53d33-138">См. также</span><span class="sxs-lookup"><span data-stu-id="53d33-138">See also</span></span>

- <span data-ttu-id="53d33-139">Участвуйте в работе сообщества на [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search).</span><span class="sxs-lookup"><span data-stu-id="53d33-139">Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search).</span></span>
