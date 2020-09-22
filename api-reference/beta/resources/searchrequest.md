---
title: Тип ресурса Сеарчрекуест
description: Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a504edc53962b6ab2d6f62e39e23542588252566
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193262"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="8499f-104">Тип ресурса Сеарчрекуест</span><span class="sxs-lookup"><span data-stu-id="8499f-104">searchRequest resource type</span></span>

<span data-ttu-id="8499f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8499f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="8499f-106">Запрос поиска, отформатированный в большом двоичном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="8499f-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="8499f-107">Большой двоичный объект JSON содержит типы ресурсов, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, параметры сортировки, запрошенные агрегаты и поля, а также фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="8499f-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="8499f-108">В этой статье приведены [примеры](#see-also) запросов на поиск в различных ресурсах.</span><span class="sxs-lookup"><span data-stu-id="8499f-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="8499f-109">Помните об [известных ограничениях](search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, сортировку или статистическую обработку результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="8499f-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="8499f-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8499f-110">Properties</span></span>

| <span data-ttu-id="8499f-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8499f-111">Property</span></span>     | <span data-ttu-id="8499f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8499f-112">Type</span></span>        | <span data-ttu-id="8499f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8499f-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="8499f-114">Aggregations</span><span class="sxs-lookup"><span data-stu-id="8499f-114">aggregations</span></span>|<span data-ttu-id="8499f-115">Коллекция [аггрегатионоптион](aggregationOption.md)</span><span class="sxs-lookup"><span data-stu-id="8499f-115">[aggregationOption](aggregationOption.md) collection</span></span>|<span data-ttu-id="8499f-116">Задает агрегаты (также известные как уточнения), которые будут возвращены вместе с результатами поиска.</span><span class="sxs-lookup"><span data-stu-id="8499f-116">Specifies aggregations (also known as refiners) to be returned alongside search results.</span></span> <span data-ttu-id="8499f-117">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-117">Optional.</span></span>|
|<span data-ttu-id="8499f-118">аггрегатионфилтерс</span><span class="sxs-lookup"><span data-stu-id="8499f-118">aggregationFilters</span></span>|<span data-ttu-id="8499f-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8499f-119">String collection</span></span>|<span data-ttu-id="8499f-120">Содержит один или несколько фильтров для получения результатов поиска, сгруппированных и отфильтрованных по определенному значению поля.</span><span class="sxs-lookup"><span data-stu-id="8499f-120">Contains one or more filters to obtain search results aggregated and filtered to a specific value of a field.</span></span> <span data-ttu-id="8499f-121">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-121">Optional.</span></span><br><span data-ttu-id="8499f-122">Постройте этот фильтр на основе предыдущего поиска, который объединяется по одному полю.</span><span class="sxs-lookup"><span data-stu-id="8499f-122">Build this filter based on a prior search that aggregates by the same field.</span></span> <span data-ttu-id="8499f-123">В ответе предыдущего поиска Определите [сеарчбуккет](searchBucket.md) , который фильтрует результаты по определенному значению поля, используйте строку в свойстве **аггрегатионфилтертокен** и создайте строку фильтра статистической обработки в формате **"{Field}: \\ " {аггрегатионфилтертокен} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="8499f-123">From the response of the prior search, identify the [searchBucket](searchBucket.md) that filters results to the specific value of the field, use the string in its **aggregationFilterToken** property, and build an aggregation filter string in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <br><span data-ttu-id="8499f-124">Например, при поиске и статистической обработке элементов диска по типу файла возвращается объект **сеарчбуккет** для типа файла `docx` в ответе.</span><span class="sxs-lookup"><span data-stu-id="8499f-124">For example, searching and aggregating drive items by file type returns a **searchBucket** for the file type `docx` in the response.</span></span> <span data-ttu-id="8499f-125">Вы можете удобно использовать **аггрегатионфилтертокен** , возвращенный для этого **сеарчбуккет** в последующих запросах поиска, и фильтр соответствует элементам `docx` типа файла.</span><span class="sxs-lookup"><span data-stu-id="8499f-125">You can conveniently use the **aggregationFilterToken** returned for this **searchBucket** in a subsequent search query and filter matches down to drive items of the `docx` file type.</span></span> <span data-ttu-id="8499f-126">В [примере 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) и [2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) показаны фактические запросы и ответы.</span><span class="sxs-lookup"><span data-stu-id="8499f-126">[Example 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) and [example 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) show the actual requests and responses.</span></span>|
|<span data-ttu-id="8499f-127">contentSources</span><span class="sxs-lookup"><span data-stu-id="8499f-127">contentSources</span></span>|<span data-ttu-id="8499f-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8499f-128">String collection</span></span>|<span data-ttu-id="8499f-129">Содержит подключение, которое необходимо задать.</span><span class="sxs-lookup"><span data-stu-id="8499f-129">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="8499f-130">Соблюдается следующий формат: `/external/connections/connectionid` где `connectionid` — это коннектионид, определенные в администрировании соединителей.</span><span class="sxs-lookup"><span data-stu-id="8499f-130">Respects the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId defined in the Connectors Administration.</span></span> <br> <span data-ttu-id="8499f-131">Note: contentSource применяется, только если entityType = `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="8499f-131">Note : contentSource is only applicable when entityType=`externalItem`.</span></span> <span data-ttu-id="8499f-132">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-132">Optional.</span></span>|
|<span data-ttu-id="8499f-133">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="8499f-133">enableTopResults</span></span>|<span data-ttu-id="8499f-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="8499f-134">Boolean</span></span>|<span data-ttu-id="8499f-135">Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее актуальны.</span><span class="sxs-lookup"><span data-stu-id="8499f-135">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="8499f-136">Это свойство применяется только к entityType = `message` .</span><span class="sxs-lookup"><span data-stu-id="8499f-136">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="8499f-137">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-137">Optional.</span></span>|
|<span data-ttu-id="8499f-138">entityTypes</span><span class="sxs-lookup"><span data-stu-id="8499f-138">entityTypes</span></span>|<span data-ttu-id="8499f-139">Коллекция entityType</span><span class="sxs-lookup"><span data-stu-id="8499f-139">entityType collection</span></span>| <span data-ttu-id="8499f-140">Один или несколько типов ресурсов, ожидаемых в отклике.</span><span class="sxs-lookup"><span data-stu-id="8499f-140">One or more types of resources expected in the response.</span></span> <span data-ttu-id="8499f-141">Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="8499f-141">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span></span> <span data-ttu-id="8499f-142">Ознакомьтесь с [известными ограничениями](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущностей, которые поддерживаются в одном поисковом запросе.</span><span class="sxs-lookup"><span data-stu-id="8499f-142">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="8499f-143">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-143">Required.</span></span>|
|<span data-ttu-id="8499f-144">fields</span><span class="sxs-lookup"><span data-stu-id="8499f-144">fields</span></span>|<span data-ttu-id="8499f-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8499f-145">String collection</span></span> |<span data-ttu-id="8499f-146">Содержит поля, возвращаемые для объекта ресурса еарч, указанного в **EntityType**, что позволяет настраивать поля, возвращаемые по умолчанию, в том числе дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive, или настраиваемые поля в **екстерналитем** из контента, полученного с помощью графических соединителей.</span><span class="sxs-lookup"><span data-stu-id="8499f-146">Contains the fields to be returned for earch resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive, or custom fields in **externalItem** from content ingested by Graph connectors.</span></span> <span data-ttu-id="8499f-147">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-147">Optional.</span></span>|
|<span data-ttu-id="8499f-148">from</span><span class="sxs-lookup"><span data-stu-id="8499f-148">from</span></span>|<span data-ttu-id="8499f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8499f-149">Int32</span></span>|<span data-ttu-id="8499f-150">Задает смещение результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="8499f-150">Specifies the offset for the search results.</span></span> <span data-ttu-id="8499f-151">Смещение 0 возвращает самый первый результат.</span><span class="sxs-lookup"><span data-stu-id="8499f-151">Offset 0 returns the very first result.</span></span> <span data-ttu-id="8499f-152">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-152">Optional.</span></span>|
|<span data-ttu-id="8499f-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="8499f-153">query</span></span>|[<span data-ttu-id="8499f-154">searchQuery</span><span class="sxs-lookup"><span data-stu-id="8499f-154">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="8499f-155">Содержит термины запроса.</span><span class="sxs-lookup"><span data-stu-id="8499f-155">Contains the query terms.</span></span> <span data-ttu-id="8499f-156">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-156">Required.</span></span>|
|<span data-ttu-id="8499f-157">size</span><span class="sxs-lookup"><span data-stu-id="8499f-157">size</span></span>|<span data-ttu-id="8499f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8499f-158">Int32</span></span>|<span data-ttu-id="8499f-159">Размер извлекаемой страницы.</span><span class="sxs-lookup"><span data-stu-id="8499f-159">The size of the page to be retrieved.</span></span> <span data-ttu-id="8499f-160">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-160">Optional.</span></span>|
|<span data-ttu-id="8499f-161">сортпропертиес</span><span class="sxs-lookup"><span data-stu-id="8499f-161">sortProperties</span></span>|<span data-ttu-id="8499f-162">Коллекция [сортпроперти](sortProperty.md)</span><span class="sxs-lookup"><span data-stu-id="8499f-162">[sortProperty](sortProperty.md) collection</span></span>|<span data-ttu-id="8499f-163">Содержит упорядоченную коллекцию полей и направление для сортировки результатов.</span><span class="sxs-lookup"><span data-stu-id="8499f-163">Contains the ordered collection of fields and direction to sort results.</span></span> <span data-ttu-id="8499f-164">В коллекции может быть не более 5 свойств сортировки.</span><span class="sxs-lookup"><span data-stu-id="8499f-164">There can be at most 5 sort properties in the collection.</span></span> <span data-ttu-id="8499f-165">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8499f-165">Optional.</span></span>|
|<span data-ttu-id="8499f-166">stored_fields (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="8499f-166">stored_fields (deprecated)</span></span>|<span data-ttu-id="8499f-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8499f-167">String collection</span></span> |<span data-ttu-id="8499f-168">Теперь оно заменяется свойством **Fields** .</span><span class="sxs-lookup"><span data-stu-id="8499f-168">This is now replaced by the **fields** property.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="8499f-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8499f-169">JSON representation</span></span>

<span data-ttu-id="8499f-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8499f-170">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8499f-171">См. также</span><span class="sxs-lookup"><span data-stu-id="8499f-171">See also</span></span>
- <span data-ttu-id="8499f-172">Поиск в [сообщениях электронной почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="8499f-172">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="8499f-173">Поиск [событий календаря](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="8499f-173">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="8499f-174">Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты](/graph/search-concept-files))</span><span class="sxs-lookup"><span data-stu-id="8499f-174">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="8499f-175">Данные о [настраиваемых типах поиска (соединители Graph)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="8499f-175">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="8499f-176">[Сортировка](/graph/search-concept-sort) результатов поиска</span><span class="sxs-lookup"><span data-stu-id="8499f-176">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="8499f-177">Использование [агрегатов](/graph/search-concept-aggregations) для уточнения результатов поиска</span><span class="sxs-lookup"><span data-stu-id="8499f-177">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


