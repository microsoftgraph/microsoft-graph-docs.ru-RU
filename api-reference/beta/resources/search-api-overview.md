---
title: Использование API Поиска (Майкрософт) для запросов данных
description: С помощью API поиска приложения могут искать данные Office 365 в контексте пользователя, прошедшего проверку подлинности.
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: afbb9ba469dad7751422902ea4a9876b6ca6b904
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704131"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a><span data-ttu-id="1bcf1-103">Использование API Поиска (Майкрософт) для запросов данных</span><span class="sxs-lookup"><span data-stu-id="1bcf1-103">Use the Microsoft Search API to query data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bcf1-104">С помощью API Поиска (Майкрософт) приложения могут запрашивать данные Office 365.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-104">Using the Microsoft Search API, apps can query Office 365 data.</span></span>

<span data-ttu-id="1bcf1-105">Поисковые запросы выполняются в контексте вошедшего пользователя, указанного [маркером доступа с делегированными разрешениями](/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="1bcf1-105">Search requests are executed in the context of the signed-in user, identified using an [access token with delegated permissions](/graph/auth-v2-user).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="1bcf1-106">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="1bcf1-106">Common use cases</span></span>

<span data-ttu-id="1bcf1-107">API предоставляет метод [query](../api/search-query.md) для поиска данных в службе "Поиск (Майкрософт)".</span><span class="sxs-lookup"><span data-stu-id="1bcf1-107">The search API provides a [query](../api/search-query.md) method to search across your data in Microsoft Search.</span></span> <span data-ttu-id="1bcf1-108">В этом разделе перечислены распространенные варианты использования с применением свойств, заданных в тексте запроса **query**.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-108">This section lists the common use cases, based on the properties you set in the **query** request body.</span></span>

<span data-ttu-id="1bcf1-109">Поисковые запросы выполняются от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-109">Search requests are executed on behalf of user.</span></span> <span data-ttu-id="1bcf1-110">Результаты поиска усекаются для применения правил контроля доступа к элементам.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-110">Search results are trimmed down to enforce any access control applied to the items.</span></span>  <span data-ttu-id="1bcf1-111">Например, в контексте файлов разрешения для них оцениваются в составе поискового запроса.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-111">For example, in the context of files, permissions on the files will be evaluated part of the search request.</span></span> <span data-ttu-id="1bcf1-112">С помощью поиска пользователи не смогут получить доступ к тем элементам, которые недоступны им через API перечисления.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-112">Users cannot access more items in search than they would be able to from the enumeration API.</span></span>

| <span data-ttu-id="1bcf1-113">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="1bcf1-113">Use cases</span></span> | <span data-ttu-id="1bcf1-114">Свойства, определяемые в тексте запроса query</span><span class="sxs-lookup"><span data-stu-id="1bcf1-114">Properties to define in the query request body</span></span> |
|:------------------|:---------|
|[<span data-ttu-id="1bcf1-115">Поиск в области по типам объектов</span><span class="sxs-lookup"><span data-stu-id="1bcf1-115">Scope search based on entity types</span></span>](#scope-search-based-on-entity-types)| <span data-ttu-id="1bcf1-116">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="1bcf1-116">**entityTypes**</span></span> |
|[<span data-ttu-id="1bcf1-117">Результаты со страницы</span><span class="sxs-lookup"><span data-stu-id="1bcf1-117">Page results</span></span>](#page-search-results) | <span data-ttu-id="1bcf1-118">**from** и **size**</span><span class="sxs-lookup"><span data-stu-id="1bcf1-118">**from** and **size**</span></span> |
|[<span data-ttu-id="1bcf1-119">Получение наиболее релевантных электронных писем</span><span class="sxs-lookup"><span data-stu-id="1bcf1-119">Get the most relevant emails</span></span>](#get-the-most-relevant-emails) | <span data-ttu-id="1bcf1-120">**enableTopResults**</span><span class="sxs-lookup"><span data-stu-id="1bcf1-120">**enableTopResults**</span></span> |
|[<span data-ttu-id="1bcf1-121">Получение выбранных свойств</span><span class="sxs-lookup"><span data-stu-id="1bcf1-121">Get selected properties</span></span>](#get-selected-properties) | <span data-ttu-id="1bcf1-122">**stored_fields**</span><span class="sxs-lookup"><span data-stu-id="1bcf1-122">**stored_fields**</span></span> |
|[<span data-ttu-id="1bcf1-123">Использование KQL в терминах запросов</span><span class="sxs-lookup"><span data-stu-id="1bcf1-123">Use KQL in query terms</span></span>](#keyword-query-language-kql-support) | <span data-ttu-id="1bcf1-124">**query**</span><span class="sxs-lookup"><span data-stu-id="1bcf1-124">**query**</span></span> |
|[<span data-ttu-id="1bcf1-125">Поиск внешних файлов</span><span class="sxs-lookup"><span data-stu-id="1bcf1-125">Search external Files</span></span>](/graph/search-concept-files)| <span data-ttu-id="1bcf1-126">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="1bcf1-126">**entityTypes**</span></span> |
|[<span data-ttu-id="1bcf1-127">Поиск в определенном объекте contentSource (API индексирования)</span><span class="sxs-lookup"><span data-stu-id="1bcf1-127">Search within a specific contentSource (indexing API)</span></span>](/graph/search-concept-custom-types)| <span data-ttu-id="1bcf1-128">**contentSources**</span><span class="sxs-lookup"><span data-stu-id="1bcf1-128">**contentSources**</span></span> |

### <a name="scope-search-based-on-entity-types"></a><span data-ttu-id="1bcf1-129">Поиск в области по типам объектов</span><span class="sxs-lookup"><span data-stu-id="1bcf1-129">Scope search based on entity types</span></span>

<span data-ttu-id="1bcf1-130">Область действия поискового запроса определяется с помощью свойства **entityTypes** полезных данных запроса **query**.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-130">Define the scope of the search request using the **entityTypes** property in the **query** request payload.</span></span>
<span data-ttu-id="1bcf1-131">Ниже перечислены поддерживаемые типы объектов.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-131">The following are the supported entity types:</span></span>

- [<span data-ttu-id="1bcf1-132">event</span><span class="sxs-lookup"><span data-stu-id="1bcf1-132">event</span></span>](event.md)
- [<span data-ttu-id="1bcf1-133">message</span><span class="sxs-lookup"><span data-stu-id="1bcf1-133">message</span></span>](message.md)
- [<span data-ttu-id="1bcf1-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="1bcf1-134">driveItem</span></span>](driveitem.md)
- [<span data-ttu-id="1bcf1-135">externalFile</span><span class="sxs-lookup"><span data-stu-id="1bcf1-135">externalFile</span></span>](externalfile.md)
- [<span data-ttu-id="1bcf1-136">externalItem</span><span class="sxs-lookup"><span data-stu-id="1bcf1-136">externalItem</span></span>](externalitem.md)

### <a name="page-search-results"></a><span data-ttu-id="1bcf1-137">Результаты поиска на странице</span><span class="sxs-lookup"><span data-stu-id="1bcf1-137">Page search results</span></span>

<span data-ttu-id="1bcf1-138">Управляйте разбивкой результатов поиска на страницы, указав описанные ниже два свойства в тексте запроса **query**.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-138">Control pagination of the search results by specifying the following two properties in the **query** request body:</span></span>

- <span data-ttu-id="1bcf1-139">**from** — целое значение, указывающее начальную точку (начиная с 0) для перечисления результатов поиска на странице.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-139">**from** which is an integer that indicates the 0-based starting point to list search results on the page.</span></span> <span data-ttu-id="1bcf1-140">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-140">The default value is 0.</span></span>

- <span data-ttu-id="1bcf1-141">**size** — целое число, обозначающее количество результатов, возвращаемых для страницы.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-141">**size** which is an integer that indicates the number of results to be returned for a page.</span></span> <span data-ttu-id="1bcf1-142">Значение по умолчанию: 25.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-142">The default value is 25.</span></span>

<span data-ttu-id="1bcf1-143">При поиске объекта **event** или **message** учитывайте указанные ниже ограничения.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-143">Note the following limits if you're searching the **event** or **message** entity:</span></span>

- <span data-ttu-id="1bcf1-144">Значение **from** должно начинаться нуля для запроса первой страницы. В противном случае запрос возвращает ошибку HTTP 400 `Bad request`.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-144">**from** must start at zero in the first page request, otherwise the request results in HTTP 400 `Bad request`.</span></span>
- <span data-ttu-id="1bcf1-145">Максимальное количество результатов на странице (**size**) составляет 200.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-145">The maximum results per page (**size**) is 200.</span></span>
- <span data-ttu-id="1bcf1-146">Максимальное общее количество элементов, которые могут быть возвращены с разбивкой на страницы, составляет 1000.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-146">The maximum total number of items that can be returned by paginating is 1000.</span></span>
- <span data-ttu-id="1bcf1-147">При превышении ограничений возвращается наилучший возможный отклик.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-147">Going beyond the limits returns a best effort response.</span></span> <span data-ttu-id="1bcf1-148">Запрос не возвращает ошибку HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-148">The request does not result in HTTP 400.</span></span>

<span data-ttu-id="1bcf1-149">Рекомендации:</span><span class="sxs-lookup"><span data-stu-id="1bcf1-149">Best practices:</span></span>

- <span data-ttu-id="1bcf1-150">В исходном запросе задайте меньший размер первой страницы.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-150">Specify a smaller first page in the initial request.</span></span> <span data-ttu-id="1bcf1-151">Например, задайте для свойства **from** значение 0, а для свойства **size** — 25.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-151">For example, specify **from** as 0, **size** as 25.</span></span>
- <span data-ttu-id="1bcf1-152">Для получения последующих страниц обновите свойства **from** и **size**.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-152">Paginate subsequent pages by updating the **from** and **size** properties.</span></span> <span data-ttu-id="1bcf1-153">Вы можете увеличивать размер страницы в каждом последующем запросе.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-153">You can increase the page size in each subsequent request.</span></span> <span data-ttu-id="1bcf1-154">В приведенной ниже таблице показан пример.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-154">The following table shows an example.</span></span>

    | <span data-ttu-id="1bcf1-155">Страница</span><span class="sxs-lookup"><span data-stu-id="1bcf1-155">Page</span></span> | <span data-ttu-id="1bcf1-156">from</span><span class="sxs-lookup"><span data-stu-id="1bcf1-156">from</span></span> | <span data-ttu-id="1bcf1-157">size</span><span class="sxs-lookup"><span data-stu-id="1bcf1-157">size</span></span> |
    |:-----|:-----|:-----|
    | <span data-ttu-id="1bcf1-158">1</span><span class="sxs-lookup"><span data-stu-id="1bcf1-158">1</span></span>    | <span data-ttu-id="1bcf1-159">0</span><span class="sxs-lookup"><span data-stu-id="1bcf1-159">0</span></span> | <span data-ttu-id="1bcf1-160">25</span><span class="sxs-lookup"><span data-stu-id="1bcf1-160">25</span></span> |
    | <span data-ttu-id="1bcf1-161">2</span><span class="sxs-lookup"><span data-stu-id="1bcf1-161">2</span></span>    | <span data-ttu-id="1bcf1-162">25</span><span class="sxs-lookup"><span data-stu-id="1bcf1-162">25</span></span> | <span data-ttu-id="1bcf1-163">50</span><span class="sxs-lookup"><span data-stu-id="1bcf1-163">50</span></span> |
    | <span data-ttu-id="1bcf1-164">3</span><span class="sxs-lookup"><span data-stu-id="1bcf1-164">3</span></span>    | <span data-ttu-id="1bcf1-165">75</span><span class="sxs-lookup"><span data-stu-id="1bcf1-165">75</span></span> | <span data-ttu-id="1bcf1-166">75</span><span class="sxs-lookup"><span data-stu-id="1bcf1-166">75</span></span> |
    | <span data-ttu-id="1bcf1-167">4</span><span class="sxs-lookup"><span data-stu-id="1bcf1-167">4</span></span>    | <span data-ttu-id="1bcf1-168">150</span><span class="sxs-lookup"><span data-stu-id="1bcf1-168">150</span></span> | <span data-ttu-id="1bcf1-169">100</span><span class="sxs-lookup"><span data-stu-id="1bcf1-169">100</span></span> |

### <a name="get-the-most-relevant-emails"></a><span data-ttu-id="1bcf1-170">Получение наиболее релевантных электронных писем</span><span class="sxs-lookup"><span data-stu-id="1bcf1-170">Get the most relevant emails</span></span>

<span data-ttu-id="1bcf1-171">Если при поиске объекта **message** задать для свойства **enableTopResults** значение `true`, возвращается гибридный список сообщений: первые три сообщения в отклике сортируются по релевантности, а остальные — по дате.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-171">When searching the **message** entity, specifying **enableTopResults** as `true` returns a hybrid list of messages : the first 3 messages in the response are sorted by relevance, the remaining messages are sorted by date.</span></span>

### <a name="get-selected-properties"></a><span data-ttu-id="1bcf1-172">Получение выбранных свойств</span><span class="sxs-lookup"><span data-stu-id="1bcf1-172">Get selected properties</span></span>

<span data-ttu-id="1bcf1-173">При поиске объекта **externalItem** используйте свойство **stored_fields**, чтобы задать поля, возвращаемые в отклике.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-173">When searching an **externalItem** entity, use the **stored_fields** property to specify the fields to be returned in the response.</span></span>

<span data-ttu-id="1bcf1-174">Имена, указанные в свойстве **stored_fields**, должны быть управляемыми свойствами, поддерживающими извлечение.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-174">The names specified in **stored_fields** should be the retrievable Managed Property.</span></span> <span data-ttu-id="1bcf1-175">Эти имена свойств были настроены для подключения в центре администрирования клиента службы "Поиск (Майкрософт)".</span><span class="sxs-lookup"><span data-stu-id="1bcf1-175">These property names have been configured for the connection in the  tenant administration of Microsoft Search.</span></span>

### <a name="keyword-query-language-kql-support"></a><span data-ttu-id="1bcf1-176">Поддержка языка KQL</span><span class="sxs-lookup"><span data-stu-id="1bcf1-176">Keyword Query Language (KQL) support</span></span>

<span data-ttu-id="1bcf1-177">Вы можете указать произвольный текст ключевых слов (например, `AND` и `OR`) и ограничения свойств в синтаксисе KQL в фактической строке поискового запроса (свойства **query** в тексте запроса **query**).</span><span class="sxs-lookup"><span data-stu-id="1bcf1-177">Specify free text keywords, operators (such as `AND`, `OR`), and property restrictions in KQL syntax in the actual search query string (**query** property of the **query** request body).</span></span> <span data-ttu-id="1bcf1-178">Синтаксис и команда зависят от типов объектов (в свойстве **entityTypes**), указанных в тексте того же запроса **query**.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-178">The syntax and command depend on the entity types (in the **entityTypes** property) you target in the same **query** request body.</span></span>

<span data-ttu-id="1bcf1-179">Свойства, доступные для поиска, зависят от типа объекта.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-179">Depending on the entity type, the searchable properties vary:</span></span>

- [<span data-ttu-id="1bcf1-180">Свойства объекта message</span><span class="sxs-lookup"><span data-stu-id="1bcf1-180">message properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [<span data-ttu-id="1bcf1-181">Свойства объекта driveItem</span><span class="sxs-lookup"><span data-stu-id="1bcf1-181">driveItem properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="error-handling"></a><span data-ttu-id="1bcf1-182">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="1bcf1-182">Error handling</span></span>

<span data-ttu-id="1bcf1-183">API поиска возвращает отклики с ошибками, описанные в [определении объектов ошибок OData](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse), каждый из которых представляет собой объект JSON, содержащий код и сообщение.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-183">The search API returns error responses as defined by [OData error object definition](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse), each of which is a JSON object containing a code and a message.</span></span>

<!---TODO Describe the know errors : bad requests.--->

## <a name="known-limitations"></a><span data-ttu-id="1bcf1-184">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="1bcf1-184">Known limitations</span></span>

<span data-ttu-id="1bcf1-185">На API поиска распространяются описанные ниже ограничения.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-185">The search API has the following limitations:</span></span>

- <span data-ttu-id="1bcf1-186">Метод **query** определяется, чтобы разрешить передачу коллекции из одного или нескольких экземпляров **searchRequest**.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-186">The **query** method is defined to allow passing a collection of one or more **searchRequest** instances at once.</span></span> <span data-ttu-id="1bcf1-187">Однако в настоящее время служба может обрабатывать только по одному экземпляру [searchRequest](./searchrequest.md) за раз.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-187">However, the service currently supports only a single [searchRequest](./searchrequest.md) at a time.</span></span>

- <span data-ttu-id="1bcf1-188">Ресурс [searchRequest](./searchrequest.md) поддерживает одновременную передачу объектов нескольких типов.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-188">The [searchRequest](./searchrequest.md) resource supports passing multiple types of entities at a time.</span></span> <span data-ttu-id="1bcf1-189">Однако в настоящее время поддерживается только сочетание объектов **driveItem** и **externalFile**.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-189">However, currently the only supported combination is **driveItem** and **externalFile**.</span></span> <span data-ttu-id="1bcf1-190">Остальные сочетания недопустимы.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-190">Other combinations are invalid.</span></span>

- <span data-ttu-id="1bcf1-191">Свойство **contentSource**, которое определяет используемое соединение, применимо, только если для свойства **entityType** задано значение `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-191">The **contentSource** property, which defines the connection to use, is only applicable when **entityType** is specified as `externalItem`.</span></span>
<!--todo nmoreauteam Fix the link to ContentSource  pls provide the content source url--->

- <span data-ttu-id="1bcf1-192">API поиска не поддерживает настраиваемую сортировку и всегда сортирует результаты следующим образом:</span><span class="sxs-lookup"><span data-stu-id="1bcf1-192">The search API does not support custom sort and always sorts results in the following ways:</span></span>

  - <span data-ttu-id="1bcf1-193">результаты типов **message** и **event** сортируются по дате;</span><span class="sxs-lookup"><span data-stu-id="1bcf1-193">Sort **message** or **event** type results by date.</span></span>

  - <span data-ttu-id="1bcf1-194">результаты типов **driveItem**, **externalFile** и **externalItem** сортируются по релевантности.</span><span class="sxs-lookup"><span data-stu-id="1bcf1-194">Sort **driveItem**, **externalFile**, or **externalItem** type results by relevance.</span></span>
