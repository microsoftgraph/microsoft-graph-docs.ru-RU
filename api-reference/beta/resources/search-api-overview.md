---
title: Использование API Поиска (Майкрософт) для запросов данных
description: С помощью API поиска приложения могут искать данные Office 365 в контексте пользователя, прошедшего проверку подлинности.
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: db10ddaf3e1cb7984ddfe16854f60c3d68dbb7ae
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866625"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a><span data-ttu-id="6183f-103">Использование API Поиска (Майкрософт) для запросов данных</span><span class="sxs-lookup"><span data-stu-id="6183f-103">Use the Microsoft Search API to query data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6183f-104">Вы можете использовать API Поиска (Майкрософт) для запроса данных Office 365 в своих приложениях.</span><span class="sxs-lookup"><span data-stu-id="6183f-104">You can use the Microsoft Search API to query Office 365 data in your apps.</span></span>

<span data-ttu-id="6183f-105">Поисковые запросы выполняются в контексте вошедшего пользователя, указанного [маркером доступа с делегированными разрешениями](/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="6183f-105">Search requests are executed in the context of the signed-in user, identified using an [access token with delegated permissions](/graph/auth-v2-user).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="6183f-106">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="6183f-106">Common use cases</span></span>

<span data-ttu-id="6183f-107">API Поиска (Майкрософт) предоставляет метод [query](../api/search-query.md) для поиска данных в службе Поиска (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="6183f-107">The search API provides a [query](../api/search-query.md) method to search across your data in Microsoft Search.</span></span> <span data-ttu-id="6183f-108">В этом разделе перечислены распространенные варианты использования с применением свойств, заданных в тексте запроса **query**.</span><span class="sxs-lookup"><span data-stu-id="6183f-108">This section lists the common use cases, based on the properties you set in the **query** request body.</span></span>

<span data-ttu-id="6183f-109">Поисковые запросы выполняются от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="6183f-109">Search requests are executed on behalf of user.</span></span> <span data-ttu-id="6183f-110">Результаты поиска ограничиваются для применения правил контроля доступа к элементам.</span><span class="sxs-lookup"><span data-stu-id="6183f-110">Search results are trimmed down to enforce any access control applied to the items.</span></span>  <span data-ttu-id="6183f-111">Например, в контексте файлов разрешения для них оцениваются в составе поискового запроса.</span><span class="sxs-lookup"><span data-stu-id="6183f-111">For example, in the context of files, permissions on the files will be evaluated part of the search request.</span></span> <span data-ttu-id="6183f-112">С помощью поиска пользователи не смогут получить доступ к тем элементам, которые недоступны им через API перечисления.</span><span class="sxs-lookup"><span data-stu-id="6183f-112">Users cannot access more items in search than they would be able to from the enumeration API.</span></span>

| <span data-ttu-id="6183f-113">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="6183f-113">Use cases</span></span> | <span data-ttu-id="6183f-114">Свойства, определяемые в тексте запроса query</span><span class="sxs-lookup"><span data-stu-id="6183f-114">Properties to define in the query request body</span></span> |
|:------------------|:---------|
|[<span data-ttu-id="6183f-115">Поиск в области по типам объектов</span><span class="sxs-lookup"><span data-stu-id="6183f-115">Scope search based on entity types</span></span>](#scope-search-based-on-entity-types)| <span data-ttu-id="6183f-116">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="6183f-116">**entityTypes**</span></span> |
|[<span data-ttu-id="6183f-117">Результаты со страницы</span><span class="sxs-lookup"><span data-stu-id="6183f-117">Page results</span></span>](#page-search-results) | <span data-ttu-id="6183f-118">**from** и **size**</span><span class="sxs-lookup"><span data-stu-id="6183f-118">**from** and **size**</span></span> |
|[<span data-ttu-id="6183f-119">Получение наиболее релевантных электронных писем</span><span class="sxs-lookup"><span data-stu-id="6183f-119">Get the most relevant emails</span></span>](#get-the-most-relevant-emails) | <span data-ttu-id="6183f-120">**enableTopResults**</span><span class="sxs-lookup"><span data-stu-id="6183f-120">**enableTopResults**</span></span> |
|[<span data-ttu-id="6183f-121">Получение выбранных свойств</span><span class="sxs-lookup"><span data-stu-id="6183f-121">Get selected properties</span></span>](#get-selected-properties) | <span data-ttu-id="6183f-122">**stored_fields**</span><span class="sxs-lookup"><span data-stu-id="6183f-122">**stored_fields**</span></span> |
|[<span data-ttu-id="6183f-123">Использование KQL в терминах запросов</span><span class="sxs-lookup"><span data-stu-id="6183f-123">Use KQL in query terms</span></span>](#keyword-query-language-kql-support) | <span data-ttu-id="6183f-124">**query**</span><span class="sxs-lookup"><span data-stu-id="6183f-124">**query**</span></span> |
|[<span data-ttu-id="6183f-125">Поиск внешних файлов</span><span class="sxs-lookup"><span data-stu-id="6183f-125">Search external Files</span></span>](/graph/search-concept-files)| <span data-ttu-id="6183f-126">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="6183f-126">**entityTypes**</span></span> |
|[<span data-ttu-id="6183f-127">Поиск в определенном объекте contentSource (API индексирования)</span><span class="sxs-lookup"><span data-stu-id="6183f-127">Search within a specific contentSource (indexing API)</span></span>](/graph/search-concept-custom-types)| <span data-ttu-id="6183f-128">**contentSources**</span><span class="sxs-lookup"><span data-stu-id="6183f-128">**contentSources**</span></span> |

### <a name="scope-search-based-on-entity-types"></a><span data-ttu-id="6183f-129">Поиск в области по типам объектов</span><span class="sxs-lookup"><span data-stu-id="6183f-129">Scope search based on entity types</span></span>

<span data-ttu-id="6183f-130">Область действия поискового запроса определяется с помощью свойства **entityTypes** полезных данных запроса **query**.</span><span class="sxs-lookup"><span data-stu-id="6183f-130">Define the scope of the search request using the **entityTypes** property in the **query** request payload.</span></span>
<span data-ttu-id="6183f-131">Ниже перечислены поддерживаемые типы объектов.</span><span class="sxs-lookup"><span data-stu-id="6183f-131">The following are the supported entity types:</span></span>

- [<span data-ttu-id="6183f-132">event</span><span class="sxs-lookup"><span data-stu-id="6183f-132">event</span></span>](event.md)
- [<span data-ttu-id="6183f-133">message</span><span class="sxs-lookup"><span data-stu-id="6183f-133">message</span></span>](message.md)
- [<span data-ttu-id="6183f-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="6183f-134">driveItem</span></span>](driveitem.md)
- [<span data-ttu-id="6183f-135">externalFile</span><span class="sxs-lookup"><span data-stu-id="6183f-135">externalFile</span></span>](externalfile.md)
- [<span data-ttu-id="6183f-136">externalItem</span><span class="sxs-lookup"><span data-stu-id="6183f-136">externalItem</span></span>](externalitem.md)

### <a name="page-search-results"></a><span data-ttu-id="6183f-137">Результаты поиска на странице</span><span class="sxs-lookup"><span data-stu-id="6183f-137">Page search results</span></span>

<span data-ttu-id="6183f-138">Управляйте разбивкой результатов поиска на страницы, указав описанные ниже два свойства в тексте запроса **query**.</span><span class="sxs-lookup"><span data-stu-id="6183f-138">Control pagination of the search results by specifying the following two properties in the **query** request body:</span></span>

- <span data-ttu-id="6183f-139">**from** — целое значение, указывающее начальную точку (начиная с 0) для перечисления результатов поиска на странице.</span><span class="sxs-lookup"><span data-stu-id="6183f-139">**from** which is an integer that indicates the 0-based starting point to list search results on the page.</span></span> <span data-ttu-id="6183f-140">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="6183f-140">The default value is 0.</span></span>

- <span data-ttu-id="6183f-141">**size** — целое число, обозначающее количество результатов, возвращаемых для страницы.</span><span class="sxs-lookup"><span data-stu-id="6183f-141">**size** which is an integer that indicates the number of results to be returned for a page.</span></span> <span data-ttu-id="6183f-142">Значение по умолчанию: 25.</span><span class="sxs-lookup"><span data-stu-id="6183f-142">The default value is 25.</span></span>

<span data-ttu-id="6183f-143">При поиске объекта **event** или **message** учитывайте указанные ниже ограничения.</span><span class="sxs-lookup"><span data-stu-id="6183f-143">Note the following limits if you're searching the **event** or **message** entity:</span></span>

- <span data-ttu-id="6183f-144">Значение **from** должно начинаться с нуля для запроса первой страницы. В противном случае запрос возвращает ошибку HTTP 400 `Bad request`.</span><span class="sxs-lookup"><span data-stu-id="6183f-144">**from** must start at zero in the first page request, otherwise the request results in HTTP 400 `Bad request`.</span></span>
- <span data-ttu-id="6183f-145">Максимальное количество результатов на странице (**size**) составляет 200.</span><span class="sxs-lookup"><span data-stu-id="6183f-145">The maximum results per page (**size**) is 200.</span></span>
- <span data-ttu-id="6183f-146">Максимальное общее количество элементов, которые могут быть возвращены с разбивкой на страницы, составляет 1000.</span><span class="sxs-lookup"><span data-stu-id="6183f-146">The maximum total number of items that can be returned by paginating is 1000.</span></span>
- <span data-ttu-id="6183f-147">При превышении ограничений возвращается наилучший возможный отклик.</span><span class="sxs-lookup"><span data-stu-id="6183f-147">Going beyond the limits returns a best effort response.</span></span> <span data-ttu-id="6183f-148">Запрос не возвращает ошибку HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="6183f-148">The request does not result in HTTP 400.</span></span>

<span data-ttu-id="6183f-149">Рекомендации:</span><span class="sxs-lookup"><span data-stu-id="6183f-149">Best practices:</span></span>

- <span data-ttu-id="6183f-150">В исходном запросе задайте меньший размер первой страницы.</span><span class="sxs-lookup"><span data-stu-id="6183f-150">Specify a smaller first page in the initial request.</span></span> <span data-ttu-id="6183f-151">Например, задайте для свойства **from** значение 0, а для свойства **size** — 25.</span><span class="sxs-lookup"><span data-stu-id="6183f-151">For example, specify **from** as 0, **size** as 25.</span></span>
- <span data-ttu-id="6183f-152">Для получения последующих страниц обновите свойства **from** и **size**.</span><span class="sxs-lookup"><span data-stu-id="6183f-152">Paginate subsequent pages by updating the **from** and **size** properties.</span></span> <span data-ttu-id="6183f-153">Вы можете увеличивать размер страницы в каждом последующем запросе.</span><span class="sxs-lookup"><span data-stu-id="6183f-153">You can increase the page size in each subsequent request.</span></span> <span data-ttu-id="6183f-154">В приведенной ниже таблице показан пример.</span><span class="sxs-lookup"><span data-stu-id="6183f-154">The following table shows an example.</span></span>

    | <span data-ttu-id="6183f-155">Страница</span><span class="sxs-lookup"><span data-stu-id="6183f-155">Page</span></span> | <span data-ttu-id="6183f-156">from</span><span class="sxs-lookup"><span data-stu-id="6183f-156">from</span></span> | <span data-ttu-id="6183f-157">size</span><span class="sxs-lookup"><span data-stu-id="6183f-157">size</span></span> |
    |:-----|:-----|:-----|
    | <span data-ttu-id="6183f-158">1</span><span class="sxs-lookup"><span data-stu-id="6183f-158">1</span></span>    | <span data-ttu-id="6183f-159">0</span><span class="sxs-lookup"><span data-stu-id="6183f-159">0</span></span> | <span data-ttu-id="6183f-160">25</span><span class="sxs-lookup"><span data-stu-id="6183f-160">25</span></span> |
    | <span data-ttu-id="6183f-161">2</span><span class="sxs-lookup"><span data-stu-id="6183f-161">2</span></span>    | <span data-ttu-id="6183f-162">25</span><span class="sxs-lookup"><span data-stu-id="6183f-162">25</span></span> | <span data-ttu-id="6183f-163">50</span><span class="sxs-lookup"><span data-stu-id="6183f-163">50</span></span> |
    | <span data-ttu-id="6183f-164">3</span><span class="sxs-lookup"><span data-stu-id="6183f-164">3</span></span>    | <span data-ttu-id="6183f-165">75</span><span class="sxs-lookup"><span data-stu-id="6183f-165">75</span></span> | <span data-ttu-id="6183f-166">75</span><span class="sxs-lookup"><span data-stu-id="6183f-166">75</span></span> |
    | <span data-ttu-id="6183f-167">4</span><span class="sxs-lookup"><span data-stu-id="6183f-167">4</span></span>    | <span data-ttu-id="6183f-168">150</span><span class="sxs-lookup"><span data-stu-id="6183f-168">150</span></span> | <span data-ttu-id="6183f-169">100</span><span class="sxs-lookup"><span data-stu-id="6183f-169">100</span></span> |

### <a name="get-the-most-relevant-emails"></a><span data-ttu-id="6183f-170">Получение наиболее релевантных электронных писем</span><span class="sxs-lookup"><span data-stu-id="6183f-170">Get the most relevant emails</span></span>

<span data-ttu-id="6183f-171">Если при поиске объекта **message** задать для свойства **enableTopResults** значение `true`, возвращается гибридный список сообщений: первые три сообщения в отклике сортируются по релевантности, а остальные — по дате.</span><span class="sxs-lookup"><span data-stu-id="6183f-171">When searching the **message** entity, specifying **enableTopResults** as `true` returns a hybrid list of messages : the first 3 messages in the response are sorted by relevance, the remaining messages are sorted by date.</span></span>

### <a name="get-selected-properties"></a><span data-ttu-id="6183f-172">Получение выбранных свойств</span><span class="sxs-lookup"><span data-stu-id="6183f-172">Get selected properties</span></span>

<span data-ttu-id="6183f-173">При поиске объекта **externalItem** используйте свойство **stored_fields**, чтобы задать поля, возвращаемые в отклике.</span><span class="sxs-lookup"><span data-stu-id="6183f-173">When searching an **externalItem** entity, use the **stored_fields** property to specify the fields to be returned in the response.</span></span>

<span data-ttu-id="6183f-174">Поля, указанные в свойстве **stored_fields**, должны быть извлекаемыми управляемыми свойствами, настроенными для подключения в центре администрирования клиента службы Поиска (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="6183f-174">The fields specified in **stored_fields** should be retrievable managed properties that have been configured for the connection via the Microsoft Search tenant administration.</span></span>

### <a name="keyword-query-language-kql-support"></a><span data-ttu-id="6183f-175">Поддержка языка KQL</span><span class="sxs-lookup"><span data-stu-id="6183f-175">Keyword Query Language (KQL) support</span></span>

<span data-ttu-id="6183f-176">Вы можете указать произвольный текст ключевых слов (например, `AND` и `OR`) и ограничения свойств в синтаксисе KQL в фактической строке поискового запроса (свойства **query** в тексте запроса **query**).</span><span class="sxs-lookup"><span data-stu-id="6183f-176">Specify free text keywords, operators (such as `AND`, `OR`), and property restrictions in KQL syntax in the actual search query string (**query** property of the **query** request body).</span></span> <span data-ttu-id="6183f-177">Синтаксис и команда зависят от типов объектов (в свойстве **entityTypes**), указанных в тексте того же запроса **query**.</span><span class="sxs-lookup"><span data-stu-id="6183f-177">The syntax and command depend on the entity types (in the **entityTypes** property) you target in the same **query** request body.</span></span>

<span data-ttu-id="6183f-178">Свойства, доступные для поиска, зависят от типа объекта.</span><span class="sxs-lookup"><span data-stu-id="6183f-178">Depending on the entity type, the searchable properties vary:</span></span> <span data-ttu-id="6183f-179">Дополнительные сведения см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="6183f-179">For details, see:</span></span>

- [<span data-ttu-id="6183f-180">Свойства электронной почты</span><span class="sxs-lookup"><span data-stu-id="6183f-180">Email properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [<span data-ttu-id="6183f-181">Свойства сайта</span><span class="sxs-lookup"><span data-stu-id="6183f-181">Site properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="error-handling"></a><span data-ttu-id="6183f-182">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="6183f-182">Error handling</span></span>

<span data-ttu-id="6183f-183">API поиска возвращает отклики с ошибками, описанные в [определении объектов ошибок OData](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse), каждый из которых представляет собой объект JSON, содержащий код и сообщение.</span><span class="sxs-lookup"><span data-stu-id="6183f-183">The search API returns error responses as defined by [OData error object definition](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse), each of which is a JSON object containing a code and a message.</span></span>

<!---TODO Describe the know errors : bad requests.--->

## <a name="known-limitations"></a><span data-ttu-id="6183f-184">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="6183f-184">Known limitations</span></span>

<span data-ttu-id="6183f-185">На API поиска распространяются описанные ниже ограничения.</span><span class="sxs-lookup"><span data-stu-id="6183f-185">The search API has the following limitations:</span></span>

- <span data-ttu-id="6183f-186">Метод **query** определяется, чтобы разрешить передачу коллекции из одного или нескольких экземпляров **searchRequest**.</span><span class="sxs-lookup"><span data-stu-id="6183f-186">The **query** method is defined to allow passing a collection of one or more **searchRequest** instances at once.</span></span> <span data-ttu-id="6183f-187">Однако в настоящее время служба может обрабатывать только по одному экземпляру [searchRequest](./searchrequest.md) за раз.</span><span class="sxs-lookup"><span data-stu-id="6183f-187">However, the service currently supports only a single [searchRequest](./searchrequest.md) at a time.</span></span>

- <span data-ttu-id="6183f-188">Ресурс [searchRequest](./searchrequest.md) поддерживает одновременную передачу объектов нескольких типов.</span><span class="sxs-lookup"><span data-stu-id="6183f-188">The [searchRequest](./searchrequest.md) resource supports passing multiple types of entities at a time.</span></span> <span data-ttu-id="6183f-189">Однако в настоящее время поддерживается только сочетание объектов **driveItem** и **externalFile**.</span><span class="sxs-lookup"><span data-stu-id="6183f-189">However, currently the only supported combination is **driveItem** and **externalFile**.</span></span> <span data-ttu-id="6183f-190">Остальные сочетания недопустимы.</span><span class="sxs-lookup"><span data-stu-id="6183f-190">Other combinations are invalid.</span></span>

- <span data-ttu-id="6183f-191">Свойство **contentSource**, которое определяет используемое соединение, применимо, только если для свойства **entityType** задано значение `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="6183f-191">The **contentSource** property, which defines the connection to use, is only applicable when **entityType** is specified as `externalItem`.</span></span>
<!--todo nmoreauteam Fix the link to ContentSource  pls provide the content source url--->

- <span data-ttu-id="6183f-192">API поиска не поддерживает настраиваемую сортировку и всегда сортирует результаты следующим образом:</span><span class="sxs-lookup"><span data-stu-id="6183f-192">The search API does not support custom sort and always sorts results in the following ways:</span></span>

  - <span data-ttu-id="6183f-193">результаты типов **message** и **event** сортируются по дате;</span><span class="sxs-lookup"><span data-stu-id="6183f-193">Sort **message** or **event** type results by date.</span></span>

  - <span data-ttu-id="6183f-194">результаты типов **driveItem**, **externalFile** и **externalItem** сортируются по релевантности.</span><span class="sxs-lookup"><span data-stu-id="6183f-194">Sort **driveItem**, **externalFile**, or **externalItem** type results by relevance.</span></span>
