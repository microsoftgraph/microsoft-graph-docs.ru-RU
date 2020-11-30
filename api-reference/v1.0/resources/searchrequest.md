---
title: Тип ресурса Сеарчрекуест
description: Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f673c551ce27c16fd4fddabc26e55cd234a9f19e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378023"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="d4ca7-104">Тип ресурса Сеарчрекуест</span><span class="sxs-lookup"><span data-stu-id="d4ca7-104">searchRequest resource type</span></span>

<span data-ttu-id="d4ca7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4ca7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4ca7-106">Запрос поиска, отформатированный в большом двоичном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="d4ca7-107">Большой двоичный объект JSON содержит типы ресурсов, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, параметры сортировки, запрошенные агрегаты и поля, а также фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="d4ca7-108">В этой статье приведены [примеры](#see-also) запросов на поиск в различных ресурсах.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="d4ca7-109">Помните об [известных ограничениях](search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, сортировку или статистическую обработку результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="d4ca7-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4ca7-110">Properties</span></span>

| <span data-ttu-id="d4ca7-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4ca7-111">Property</span></span>     | <span data-ttu-id="d4ca7-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d4ca7-112">Type</span></span>        | <span data-ttu-id="d4ca7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d4ca7-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="d4ca7-114">contentSources</span><span class="sxs-lookup"><span data-stu-id="d4ca7-114">contentSources</span></span>|<span data-ttu-id="d4ca7-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d4ca7-115">String collection</span></span>|<span data-ttu-id="d4ca7-116">Содержит подключение, которое необходимо задать.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-116">Contains the connection to be targeted.</span></span>|
|<span data-ttu-id="d4ca7-117">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="d4ca7-117">enableTopResults</span></span>|<span data-ttu-id="d4ca7-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ca7-118">Boolean</span></span>|<span data-ttu-id="d4ca7-119">Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее актуальны.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-119">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="d4ca7-120">Это свойство применяется только к entityType = `message` .</span><span class="sxs-lookup"><span data-stu-id="d4ca7-120">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="d4ca7-121">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-121">Optional.</span></span>|
|<span data-ttu-id="d4ca7-122">entityTypes</span><span class="sxs-lookup"><span data-stu-id="d4ca7-122">entityTypes</span></span>|<span data-ttu-id="d4ca7-123">Коллекция entityType</span><span class="sxs-lookup"><span data-stu-id="d4ca7-123">entityType collection</span></span>| <span data-ttu-id="d4ca7-124">Один или несколько типов ресурсов, ожидаемых в отклике.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-124">One or more types of resources expected in the response.</span></span> <span data-ttu-id="d4ca7-125">Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-125">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`.</span></span> <span data-ttu-id="d4ca7-126">Ознакомьтесь с [известными ограничениями](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущностей, которые поддерживаются в одном поисковом запросе.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-126">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="d4ca7-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-127">Required.</span></span>|
|<span data-ttu-id="d4ca7-128">fields</span><span class="sxs-lookup"><span data-stu-id="d4ca7-128">fields</span></span>|<span data-ttu-id="d4ca7-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d4ca7-129">String collection</span></span> |<span data-ttu-id="d4ca7-130">Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **EntityType**, что позволяет настраивать поля, возвращаемые по умолчанию, в том числе дополнительные поля, такие как настраиваемые управляемые свойства, из SharePoint и OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-130">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive.</span></span> <span data-ttu-id="d4ca7-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-131">Optional.</span></span>|
|<span data-ttu-id="d4ca7-132">from</span><span class="sxs-lookup"><span data-stu-id="d4ca7-132">from</span></span>|<span data-ttu-id="d4ca7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ca7-133">Int32</span></span>|<span data-ttu-id="d4ca7-134">Задает смещение результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-134">Specifies the offset for the search results.</span></span> <span data-ttu-id="d4ca7-135">Смещение 0 возвращает самый первый результат.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-135">Offset 0 returns the very first result.</span></span> <span data-ttu-id="d4ca7-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-136">Optional.</span></span>|
|<span data-ttu-id="d4ca7-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4ca7-137">query</span></span>|[<span data-ttu-id="d4ca7-138">searchQuery</span><span class="sxs-lookup"><span data-stu-id="d4ca7-138">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="d4ca7-139">Содержит термины запроса.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-139">Contains the query terms.</span></span> <span data-ttu-id="d4ca7-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-140">Required.</span></span>|
|<span data-ttu-id="d4ca7-141">size</span><span class="sxs-lookup"><span data-stu-id="d4ca7-141">size</span></span>|<span data-ttu-id="d4ca7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ca7-142">Int32</span></span>|<span data-ttu-id="d4ca7-143">Размер извлекаемой страницы.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-143">The size of the page to be retrieved.</span></span> <span data-ttu-id="d4ca7-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-144">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4ca7-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d4ca7-145">JSON representation</span></span>

<span data-ttu-id="d4ca7-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4ca7-146">The following is a JSON representation of the resource.</span></span>

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a><span data-ttu-id="d4ca7-147">См. также</span><span class="sxs-lookup"><span data-stu-id="d4ca7-147">See also</span></span>
- <span data-ttu-id="d4ca7-148">Поиск в [сообщениях электронной почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="d4ca7-148">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="d4ca7-149">Поиск [событий календаря](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="d4ca7-149">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="d4ca7-150">Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты](/graph/search-concept-files))</span><span class="sxs-lookup"><span data-stu-id="d4ca7-150">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


