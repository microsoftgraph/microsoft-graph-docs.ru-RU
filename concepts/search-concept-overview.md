---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 6f7515682f7600a4c0d58e49213eacf17add44e0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866898"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a><span data-ttu-id="15c51-103">Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="15c51-103">Overview of the Microsoft Search API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="15c51-104">Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации.</span><span class="sxs-lookup"><span data-stu-id="15c51-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="15c51-105">Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей.</span><span class="sxs-lookup"><span data-stu-id="15c51-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="15c51-106">Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing.</span><span class="sxs-lookup"><span data-stu-id="15c51-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="15c51-107">Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  </span><span class="sxs-lookup"><span data-stu-id="15c51-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="15c51-108">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="15c51-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="15c51-109">Единая конечная точка поиска для данных Microsoft Cloud</span><span class="sxs-lookup"><span data-stu-id="15c51-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="15c51-110">API Поиска (Майкрософт) предоставляет единую конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query?view=graph-rest-beta) в Microsoft Cloud данных (сообщений и событий в почтовых ящиках Outlook, а также файлов в OneDrive и SharePoint), индексированных в Поиске (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="15c51-110">The Microsoft Search API provides one unified search endpoint to let developers [query](/graph/api/search-query?view=graph-rest-beta) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - data that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="15c51-111">Включение настраиваемых внешних данных в интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="15c51-111">Include custom external data in search experience</span></span>

<span data-ttu-id="15c51-112">Пользователи, желающие включить в свой поиск данные, не входящие в Microsoft Cloud, могут использовать [соединители](/microsoftsearch/connectors-overview), чтобы подключиться к определенному источнику данных, такому как база данных отдела кадров организации или каталог продуктов, и использовать API Поиска (Майкрософт) для [запроса](/graph/api/search-query?view=graph-rest-beta) внешнего источника данных.</span><span class="sxs-lookup"><span data-stu-id="15c51-112">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta) the external data source.</span></span> <span data-ttu-id="15c51-113">[Коллекция соединителей Microsoft Graph](/microsoftsearch/connectors-gallery) включает ряд готовых к использованию соединителей.</span><span class="sxs-lookup"><span data-stu-id="15c51-113">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="15c51-114">Пользователи также могут [создавать соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), индексировать внешние настраиваемые элементы и файлы и запрашивать определенные внешние источники данных.</span><span class="sxs-lookup"><span data-stu-id="15c51-114">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), index external custom items and files, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="15c51-115">Единый актуальный интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="15c51-115">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="15c51-116">При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="15c51-116">Using the Microsoft Search API, customers benefit from getting more personalized relevant results powered by Microsoft Graph.</span></span> <span data-ttu-id="15c51-117">Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.</span><span class="sxs-lookup"><span data-stu-id="15c51-117">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="15c51-118">Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="15c51-118">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="15c51-119">API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:</span><span class="sxs-lookup"><span data-stu-id="15c51-119">Microsoft Search supports searching content in the Microsoft cloud:</span></span>

- <span data-ttu-id="15c51-120">Объекты [message](/graph/api/resources/message?view=graph-rest-beta) и [event](/graph/api/resources/event?view=graph-rest-beta) в Outlook</span><span class="sxs-lookup"><span data-stu-id="15c51-120">Outlook [message](/graph/api/resources/message?view=graph-rest-beta) and [event](/graph/api/resources/event?view=graph-rest-beta) objects</span></span>
- <span data-ttu-id="15c51-121">Файловые объекты [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) в SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="15c51-121">SharePoint and OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) file objects</span></span>

<span data-ttu-id="15c51-122">Кроме того, вы можете индексировать и искать внешний контент, используя:</span><span class="sxs-lookup"><span data-stu-id="15c51-122">In addition, you can index and search external content:</span></span>

- <span data-ttu-id="15c51-123">Объекты [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) настраиваемого типа</span><span class="sxs-lookup"><span data-stu-id="15c51-123">[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) objects which are of custom types</span></span>
- <span data-ttu-id="15c51-124">Объекты [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) известного типа</span><span class="sxs-lookup"><span data-stu-id="15c51-124">[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) objects which are of well-known types</span></span>

## <a name="api-reference"></a><span data-ttu-id="15c51-125">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="15c51-125">API reference</span></span>

<span data-ttu-id="15c51-126">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="15c51-126">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="15c51-127">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="15c51-127">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="15c51-128">Использование API Поиска (Майкрософт) для индексирования данных</span><span class="sxs-lookup"><span data-stu-id="15c51-128">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="15c51-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="15c51-129">Next steps</span></span>

- <span data-ttu-id="15c51-130">Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="15c51-130">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="15c51-131">Подробнее о некоторых основных вариантах использования:</span><span class="sxs-lookup"><span data-stu-id="15c51-131">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="15c51-132">Поиск сообщений Outlook</span><span class="sxs-lookup"><span data-stu-id="15c51-132">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="15c51-133">Поиск событий календаря</span><span class="sxs-lookup"><span data-stu-id="15c51-133">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="15c51-134">Управление подключениями для индексирования внешнего контента</span><span class="sxs-lookup"><span data-stu-id="15c51-134">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="15c51-135">Индексирование внешнего контента</span><span class="sxs-lookup"><span data-stu-id="15c51-135">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="15c51-136">Поиск объектов настраиваемого типа (externalItem)</span><span class="sxs-lookup"><span data-stu-id="15c51-136">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="15c51-137">Поиск файлов (включая externalFile)</span><span class="sxs-lookup"><span data-stu-id="15c51-137">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="15c51-138">Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="15c51-138">Explore the search APIs in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="15c51-139">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.</span><span class="sxs-lookup"><span data-stu-id="15c51-139">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="15c51-140">См. также</span><span class="sxs-lookup"><span data-stu-id="15c51-140">See also</span></span>

- <span data-ttu-id="15c51-141">Участвуйте в работе сообщества на [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-search).</span><span class="sxs-lookup"><span data-stu-id="15c51-141">Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-search).</span></span>
