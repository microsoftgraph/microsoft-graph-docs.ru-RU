---
title: Обзор API Поиска (предварительная версия)
description: Узнайте, как использовать API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: b8840f382442319d49e3db72503e02ddbdadfd57
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950418"
---
# <a name="overview-for-extending-the-microsoft-search-experience-for-apps-on-microsoft-graph-preview"></a><span data-ttu-id="76781-103">Обзор расширенных возможностей Поиска (Майкрософт) для приложений в Microsoft Graph (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="76781-103">Overview for extending the Microsoft Search experience for apps on Microsoft Graph (preview)</span></span>

<span data-ttu-id="76781-104">Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации.</span><span class="sxs-lookup"><span data-stu-id="76781-104">Microsoft Search is an enterprise search experience that increases productivity and saves time by delivering more relevant search results for your organization</span></span> <span data-ttu-id="76781-105">Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей.</span><span class="sxs-lookup"><span data-stu-id="76781-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="76781-106">Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing.</span><span class="sxs-lookup"><span data-stu-id="76781-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span>

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="76781-107">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="76781-107">Why use the Microsoft Graph Security API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="76781-108">Единая конечная точка поиска для данных Microsoft Cloud</span><span class="sxs-lookup"><span data-stu-id="76781-108">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="76781-109">API Поиска (Майкрософт) предоставляет единую конечную точку поиска, позволяющую разработчикам [запрашивать](/graph/api/search-query?view=graph-rest-beta) в Microsoft Cloud данные (сообщения и события в почтовых ящиках Outlook, а также файлы в OneDrive и SharePoint), индексированные в Поиске (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="76781-109">The Microsoft Search API provides one unified search endpoint to let developers [query](/graph/api/search-query?view=graph-rest-beta) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - data that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="76781-110">Включение настраиваемых внешних данных в интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="76781-110">Include custom external data in search experience</span></span>

<span data-ttu-id="76781-111">Пользователи, желающие включить в свой поиск данные, не входящие в Microsoft Cloud, могут использовать [соединители](/microsoftsearch/connectors-overview), чтобы подключиться к определенному источнику данных, такому как база данных отдела кадров организации или каталог продуктов, и использовать API Поиска (Майкрософт) для [запроса](/graph/api/search-query?view=graph-rest-beta) внешнего источника данных.</span><span class="sxs-lookup"><span data-stu-id="76781-111">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta) the external data source.</span></span> <span data-ttu-id="76781-112">[Коллекция соединителей Microsoft Graph](/microsoftsearch/connectors-gallery) включает ряд готовых к использованию соединителей.</span><span class="sxs-lookup"><span data-stu-id="76781-112">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="76781-113">Пользователи также могут [создавать соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), индексировать внешние настраиваемые элементы и файлы и запрашивать определенные внешние источники данных.</span><span class="sxs-lookup"><span data-stu-id="76781-113">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), index external custom items and files, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="76781-114">Единый актуальный интерфейс поиска</span><span class="sxs-lookup"><span data-stu-id="76781-114">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="76781-115">Используя API Поиска (Майкрософт), клиенты получают персонализированные релевантные результаты благодаря Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="76781-115">Using the Microsoft Search API, customers benefit from getting more personalized relevant results powered by Microsoft Graph.</span></span> <span data-ttu-id="76781-116">Кроме того, поиск в ваших приложениях возвращает результаты, согласованные с поиском в приложениях Office.</span><span class="sxs-lookup"><span data-stu-id="76781-116">This also makes search in your apps return results consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-these-apis"></a><span data-ttu-id="76781-117">Какие данные можно добавить и к каким получить доступ с помощью этих API?</span><span class="sxs-lookup"><span data-stu-id="76781-117">What data can I add or access by using these APIs?</span></span>

<span data-ttu-id="76781-118">Поиск (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:</span><span class="sxs-lookup"><span data-stu-id="76781-118">Microsoft Search supports searching content in the Microsoft cloud:</span></span>

- <span data-ttu-id="76781-119">Объекты [message](/graph/api/resources/message?view=graph-rest-beta) и [event](/graph/api/resources/event?view=graph-rest-beta) в Outlook</span><span class="sxs-lookup"><span data-stu-id="76781-119">Outlook [message](/graph/api/resources/message?view=graph-rest-beta) and [event](/graph/api/resources/event?view=graph-rest-beta) objects</span></span>
- <span data-ttu-id="76781-120">Файловые объекты [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) в SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="76781-120">SharePoint and OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) file objects</span></span>

<span data-ttu-id="76781-121">Кроме того, вы можете индексировать и искать внешний контент:</span><span class="sxs-lookup"><span data-stu-id="76781-121">In addition, you can index and search external content:</span></span>

- <span data-ttu-id="76781-122">Объекты [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) настраиваемого типа</span><span class="sxs-lookup"><span data-stu-id="76781-122">[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) objects which are of custom types</span></span>
- <span data-ttu-id="76781-123">Объекты [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) известного типа</span><span class="sxs-lookup"><span data-stu-id="76781-123">[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) objects which are of well-known types</span></span>

## <a name="api-reference"></a><span data-ttu-id="76781-124">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="76781-124">API reference</span></span>

<span data-ttu-id="76781-125">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="76781-125">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="76781-126">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="76781-126">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="76781-127">Использование API Поиска (Майкрософт) для индексирования данных</span><span class="sxs-lookup"><span data-stu-id="76781-127">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="76781-128">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="76781-128">Next steps</span></span>

- <span data-ttu-id="76781-129">Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="76781-129">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="76781-130">Подробнее о некоторых основных вариантах использования:</span><span class="sxs-lookup"><span data-stu-id="76781-130">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="76781-131">Поиск сообщений Outlook</span><span class="sxs-lookup"><span data-stu-id="76781-131">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="76781-132">Поиск событий календаря</span><span class="sxs-lookup"><span data-stu-id="76781-132">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="76781-133">Управление подключениями для индексирования внешнего контента</span><span class="sxs-lookup"><span data-stu-id="76781-133">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="76781-134">Индексирование внешнего контента</span><span class="sxs-lookup"><span data-stu-id="76781-134">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="76781-135">Поиск объектов настраиваемого типа (externalItem)</span><span class="sxs-lookup"><span data-stu-id="76781-135">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="76781-136">Поиск файлов (включая externalFile)</span><span class="sxs-lookup"><span data-stu-id="76781-136">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="76781-137">Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="76781-137">Explore the APIs in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="76781-138">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.</span><span class="sxs-lookup"><span data-stu-id="76781-138">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="76781-139">См. также</span><span class="sxs-lookup"><span data-stu-id="76781-139">See also</span></span>

<span data-ttu-id="76781-140">Взаимодействие с сообществом:</span><span class="sxs-lookup"><span data-stu-id="76781-140">Engage with the community:</span></span>

- [<span data-ttu-id="76781-141">Обсуждения на сайте StackOverflow</span><span class="sxs-lookup"><span data-stu-id="76781-141">Discuss on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/microsoft-search)
