---
title: Тип ресурса searchRequest
description: Поисковый запрос, который будет отправлен в конечную точку запроса. Содержит тип сущностями, ожидаемыми в ответе, основные источники, параметры подкатки, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3bda8b317e1bc42e21943c23ca8a841572cf8cd0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883188"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="06986-104">Тип ресурса searchRequest</span><span class="sxs-lookup"><span data-stu-id="06986-104">searchRequest resource type</span></span>

<span data-ttu-id="06986-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06986-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="06986-106">Запрос поиска, отформатированный в BLOB-оке JSON.</span><span class="sxs-lookup"><span data-stu-id="06986-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="06986-107">Большой объем JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры разбития на поля, параметры сортировки, запрашиваемую агрегацию и поля, а также фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="06986-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="06986-108">См. [примеры](#see-also) запросов поиска на различных ресурсах.</span><span class="sxs-lookup"><span data-stu-id="06986-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="06986-109">Следует помнить об [известных ограничениях](search-api-overview.md#known-limitations) поиска определенных комбинаций типов сущностей, а также сортировки или агрегации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="06986-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="06986-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="06986-110">Properties</span></span>

| <span data-ttu-id="06986-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="06986-111">Property</span></span>     | <span data-ttu-id="06986-112">Тип</span><span class="sxs-lookup"><span data-stu-id="06986-112">Type</span></span>        | <span data-ttu-id="06986-113">Описание</span><span class="sxs-lookup"><span data-stu-id="06986-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="06986-114">aggregations</span><span class="sxs-lookup"><span data-stu-id="06986-114">aggregations</span></span>|<span data-ttu-id="06986-115">[коллекция aggregationOption](aggregationOption.md)</span><span class="sxs-lookup"><span data-stu-id="06986-115">[aggregationOption](aggregationOption.md) collection</span></span>|<span data-ttu-id="06986-116">Указывает агрегации (также известные как уточнения), которые должны возвращаться вместе с результатами поиска.</span><span class="sxs-lookup"><span data-stu-id="06986-116">Specifies aggregations (also known as refiners) to be returned alongside search results.</span></span> <span data-ttu-id="06986-117">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06986-117">Optional.</span></span>|
|<span data-ttu-id="06986-118">aggregationFilters</span><span class="sxs-lookup"><span data-stu-id="06986-118">aggregationFilters</span></span>|<span data-ttu-id="06986-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="06986-119">String collection</span></span>|<span data-ttu-id="06986-120">Содержит один или несколько фильтров для получения результатов поиска, агрегированных и отфильтрованных по определенному значению поля.</span><span class="sxs-lookup"><span data-stu-id="06986-120">Contains one or more filters to obtain search results aggregated and filtered to a specific value of a field.</span></span> <span data-ttu-id="06986-121">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06986-121">Optional.</span></span><br><span data-ttu-id="06986-122">Создайте этот фильтр на основе предыдущего поиска, агрегированного по одному полю.</span><span class="sxs-lookup"><span data-stu-id="06986-122">Build this filter based on a prior search that aggregates by the same field.</span></span> <span data-ttu-id="06986-123">В ответе предыдущего поиска определите [объект searchBucket,](searchBucket.md) который фильтрует результаты по определенному значению поля, используйте строку в свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}: \\ "{aggregationFilterToken} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="06986-123">From the response of the prior search, identify the [searchBucket](searchBucket.md) that filters results to the specific value of the field, use the string in its **aggregationFilterToken** property, and build an aggregation filter string in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <br><span data-ttu-id="06986-124">Если необходимо увести несколько значений для одного поля, используйте строки в его свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}:or( \\ "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**.</span><span class="sxs-lookup"><span data-stu-id="06986-124">If multiple values for the same field need to be provided, use the strings in its **aggregationFilterToken** property and build an aggregation filter string in the format **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**.</span></span> <br><span data-ttu-id="06986-125">Например, при поиске и агрегации элементов диска по типу файла возвращается **объект searchBucket** для типа файла `docx` в ответе.</span><span class="sxs-lookup"><span data-stu-id="06986-125">For example, searching and aggregating drive items by file type returns a **searchBucket** for the file type `docx` in the response.</span></span> <span data-ttu-id="06986-126">Вы можете удобно использовать **aggregationFilterToken,** возвращенный для этого **searchBucket,** в последующем поисковом запросе и фильтре совпадений вниз для элементов типа `docx` файла.</span><span class="sxs-lookup"><span data-stu-id="06986-126">You can conveniently use the **aggregationFilterToken** returned for this **searchBucket** in a subsequent search query and filter matches down to drive items of the `docx` file type.</span></span> <span data-ttu-id="06986-127">[В примере 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [и примере 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) показываются фактические запросы и ответы.</span><span class="sxs-lookup"><span data-stu-id="06986-127">[Example 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) and [example 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) show the actual requests and responses.</span></span>|
|<span data-ttu-id="06986-128">contentSources</span><span class="sxs-lookup"><span data-stu-id="06986-128">contentSources</span></span>|<span data-ttu-id="06986-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="06986-129">String collection</span></span>|<span data-ttu-id="06986-130">Содержит подключение, которое необходимо нацелить.</span><span class="sxs-lookup"><span data-stu-id="06986-130">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="06986-131">Соблюдает следующий формат: `/external/connections/connectionid` `connectionid` где находится ConnectionId, определенный в администрировании соединитеителей.</span><span class="sxs-lookup"><span data-stu-id="06986-131">Respects the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId defined in the Connectors Administration.</span></span> <br> <span data-ttu-id="06986-132">Примечание. contentSource применимо только в том случае, если entityType= `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="06986-132">Note : contentSource is only applicable when entityType=`externalItem`.</span></span> <span data-ttu-id="06986-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06986-133">Optional.</span></span>|
|<span data-ttu-id="06986-134">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="06986-134">enableTopResults</span></span>|<span data-ttu-id="06986-135">Логический</span><span class="sxs-lookup"><span data-stu-id="06986-135">Boolean</span></span>|<span data-ttu-id="06986-136">Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее релевантны.</span><span class="sxs-lookup"><span data-stu-id="06986-136">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="06986-137">Это свойство применимо только к entityType= `message` .</span><span class="sxs-lookup"><span data-stu-id="06986-137">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="06986-138">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06986-138">Optional.</span></span>|
|<span data-ttu-id="06986-139">entityTypes</span><span class="sxs-lookup"><span data-stu-id="06986-139">entityTypes</span></span>|<span data-ttu-id="06986-140">Коллекция entityType</span><span class="sxs-lookup"><span data-stu-id="06986-140">entityType collection</span></span>| <span data-ttu-id="06986-141">Один или несколько типов ресурсов, ожидаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="06986-141">One or more types of resources expected in the response.</span></span> <span data-ttu-id="06986-142">Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="06986-142">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span></span> <span data-ttu-id="06986-143">См. [известные ограничения](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов су субъектов, которые поддерживаются в одном поисковом запросе.</span><span class="sxs-lookup"><span data-stu-id="06986-143">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="06986-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06986-144">Required.</span></span>|
|<span data-ttu-id="06986-145">fields</span><span class="sxs-lookup"><span data-stu-id="06986-145">fields</span></span>|<span data-ttu-id="06986-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="06986-146">String collection</span></span> |<span data-ttu-id="06986-147">Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **entityTypes,** что позволяет настраивать поля, возвращаемые по умолчанию, в противном случае, включая дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive, или настраиваемые поля в **externalItem** из содержимого, посеяно соединителю Graph.</span><span class="sxs-lookup"><span data-stu-id="06986-147">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive, or custom fields in **externalItem** from content ingested by Graph connectors.</span></span> <span data-ttu-id="06986-148">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06986-148">Optional.</span></span>|
|<span data-ttu-id="06986-149">from</span><span class="sxs-lookup"><span data-stu-id="06986-149">from</span></span>|<span data-ttu-id="06986-150">Int32</span><span class="sxs-lookup"><span data-stu-id="06986-150">Int32</span></span>|<span data-ttu-id="06986-151">Указывает смещение результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="06986-151">Specifies the offset for the search results.</span></span> <span data-ttu-id="06986-152">Смещение 0 возвращает самый первый результат.</span><span class="sxs-lookup"><span data-stu-id="06986-152">Offset 0 returns the very first result.</span></span> <span data-ttu-id="06986-153">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06986-153">Optional.</span></span>|
|<span data-ttu-id="06986-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="06986-154">query</span></span>|[<span data-ttu-id="06986-155">searchQuery</span><span class="sxs-lookup"><span data-stu-id="06986-155">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="06986-156">Содержит термины запроса.</span><span class="sxs-lookup"><span data-stu-id="06986-156">Contains the query terms.</span></span> <span data-ttu-id="06986-157">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06986-157">Required.</span></span>|
|<span data-ttu-id="06986-158">size</span><span class="sxs-lookup"><span data-stu-id="06986-158">size</span></span>|<span data-ttu-id="06986-159">Int32</span><span class="sxs-lookup"><span data-stu-id="06986-159">Int32</span></span>|<span data-ttu-id="06986-160">Размер извлекаемой страницы.</span><span class="sxs-lookup"><span data-stu-id="06986-160">The size of the page to be retrieved.</span></span> <span data-ttu-id="06986-161">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06986-161">Optional.</span></span>|
|<span data-ttu-id="06986-162">sortProperties</span><span class="sxs-lookup"><span data-stu-id="06986-162">sortProperties</span></span>|<span data-ttu-id="06986-163">[Коллекция sortProperty](sortProperty.md)</span><span class="sxs-lookup"><span data-stu-id="06986-163">[sortProperty](sortProperty.md) collection</span></span>|<span data-ttu-id="06986-164">Содержит упорядоченную коллекцию полей и направление сортировки результатов.</span><span class="sxs-lookup"><span data-stu-id="06986-164">Contains the ordered collection of fields and direction to sort results.</span></span> <span data-ttu-id="06986-165">В коллекции может быть не более 5 свойств сортировки.</span><span class="sxs-lookup"><span data-stu-id="06986-165">There can be at most 5 sort properties in the collection.</span></span> <span data-ttu-id="06986-166">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06986-166">Optional.</span></span>|
|<span data-ttu-id="06986-167">stored_fields (неподготовлено)</span><span class="sxs-lookup"><span data-stu-id="06986-167">stored_fields (deprecated)</span></span>|<span data-ttu-id="06986-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="06986-168">String collection</span></span> |<span data-ttu-id="06986-169">Теперь это свойство заменяется **свойством fields.**</span><span class="sxs-lookup"><span data-stu-id="06986-169">This is now replaced by the **fields** property.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="06986-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06986-170">JSON representation</span></span>

<span data-ttu-id="06986-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06986-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "sortProperties": [{"@odata.type": "microsoft.graph.sortProperty"}],
  "aggregations": [{"@odata.type": "microsoft.graph.aggregationOption"}],
  "aggregationFilters": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a><span data-ttu-id="06986-172">См. также</span><span class="sxs-lookup"><span data-stu-id="06986-172">See also</span></span>
- <span data-ttu-id="06986-173">Поиск [в почтовых сообщениях](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="06986-173">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="06986-174">Поиск [событий календаря](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="06986-174">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="06986-175">Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты)](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="06986-175">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="06986-176">Поиск [пользовательских типов, импортируемых с помощью соединители)](/graph/search-concept-custom-types) данных</span><span class="sxs-lookup"><span data-stu-id="06986-176">Search [custom types imported using connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="06986-177">[Сортировка](/graph/search-concept-sort) результатов поиска</span><span class="sxs-lookup"><span data-stu-id="06986-177">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="06986-178">Использование [агрегаций для](/graph/search-concept-aggregations) уточнения результатов поиска</span><span class="sxs-lookup"><span data-stu-id="06986-178">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


