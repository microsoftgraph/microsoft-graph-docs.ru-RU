---
title: тип ресурса searchRequest
description: Запрос на поиск, который будет отправлен в конечную точку запроса. Он содержит тип сущностями, ожидаемыми в ответе, основные источники, параметры paging, запрос полей и фактический запрос поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4a797126a1dc6bc5fbecc9aad050711b499945ff
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207989"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="ce903-104">тип ресурса searchRequest</span><span class="sxs-lookup"><span data-stu-id="ce903-104">searchRequest resource type</span></span>

<span data-ttu-id="ce903-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce903-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce903-106">Запрос поиска, отформатированный в blob JSON.</span><span class="sxs-lookup"><span data-stu-id="ce903-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="ce903-107">BLOB JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры paging, параметры сортировки, запрашиваемая агрегация и поля, а также фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="ce903-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="ce903-108">Примеры [запросов](#see-also) на поиск см. на различных ресурсах.</span><span class="sxs-lookup"><span data-stu-id="ce903-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="ce903-109">Будьте в курсе [известных ограничений](search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, а также сортировку или агрегирование результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="ce903-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="ce903-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce903-110">Properties</span></span>

| <span data-ttu-id="ce903-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce903-111">Property</span></span>     | <span data-ttu-id="ce903-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ce903-112">Type</span></span>        | <span data-ttu-id="ce903-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ce903-113">Description</span></span> |             |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="ce903-114">contentSources</span><span class="sxs-lookup"><span data-stu-id="ce903-114">contentSources</span></span>|<span data-ttu-id="ce903-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ce903-115">String collection</span></span>|<span data-ttu-id="ce903-116">Содержит адресное подключение.</span><span class="sxs-lookup"><span data-stu-id="ce903-116">Contains the connection to be targeted.</span></span>|
|<span data-ttu-id="ce903-117">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="ce903-117">enableTopResults</span></span>|<span data-ttu-id="ce903-118">Логический</span><span class="sxs-lookup"><span data-stu-id="ce903-118">Boolean</span></span>|<span data-ttu-id="ce903-119">Это вызывает гибридную сортировку сообщений: первые 3 сообщения являются наиболее актуальными.</span><span class="sxs-lookup"><span data-stu-id="ce903-119">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="ce903-120">Это свойство применимо только к entityType= `message` .</span><span class="sxs-lookup"><span data-stu-id="ce903-120">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="ce903-121">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ce903-121">Optional.</span></span>|
|<span data-ttu-id="ce903-122">entityTypes</span><span class="sxs-lookup"><span data-stu-id="ce903-122">entityTypes</span></span>|<span data-ttu-id="ce903-123">Коллекция entityType</span><span class="sxs-lookup"><span data-stu-id="ce903-123">entityType collection</span></span>| <span data-ttu-id="ce903-124">Один или несколько типов ресурсов, ожидаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="ce903-124">One or more types of resources expected in the response.</span></span> <span data-ttu-id="ce903-125">Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="ce903-125">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span></span> <span data-ttu-id="ce903-126">См. [известные ограничения](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущности, поддерживаемых в одном запросе поиска.</span><span class="sxs-lookup"><span data-stu-id="ce903-126">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="ce903-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ce903-127">Required.</span></span>|
|<span data-ttu-id="ce903-128">fields</span><span class="sxs-lookup"><span data-stu-id="ce903-128">fields</span></span>|<span data-ttu-id="ce903-129">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ce903-129">String collection</span></span> |<span data-ttu-id="ce903-130">Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **entityTypes,** что позволяет настраивать поля, возвращаемые по умолчанию, в том числе дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ce903-130">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive.</span></span> <span data-ttu-id="ce903-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ce903-131">Optional.</span></span>|
|<span data-ttu-id="ce903-132">from</span><span class="sxs-lookup"><span data-stu-id="ce903-132">from</span></span>|<span data-ttu-id="ce903-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ce903-133">Int32</span></span>|<span data-ttu-id="ce903-134">Указывает смещение результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="ce903-134">Specifies the offset for the search results.</span></span> <span data-ttu-id="ce903-135">Смещение 0 возвращает самый первый результат.</span><span class="sxs-lookup"><span data-stu-id="ce903-135">Offset 0 returns the very first result.</span></span> <span data-ttu-id="ce903-136">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ce903-136">Optional.</span></span>|
|<span data-ttu-id="ce903-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce903-137">query</span></span>|[<span data-ttu-id="ce903-138">searchQuery</span><span class="sxs-lookup"><span data-stu-id="ce903-138">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="ce903-139">Содержит термины запроса.</span><span class="sxs-lookup"><span data-stu-id="ce903-139">Contains the query terms.</span></span> <span data-ttu-id="ce903-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ce903-140">Required.</span></span>|
|<span data-ttu-id="ce903-141">size</span><span class="sxs-lookup"><span data-stu-id="ce903-141">size</span></span>|<span data-ttu-id="ce903-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ce903-142">Int32</span></span>|<span data-ttu-id="ce903-143">Размер извлекаемой страницы.</span><span class="sxs-lookup"><span data-stu-id="ce903-143">The size of the page to be retrieved.</span></span> <span data-ttu-id="ce903-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ce903-144">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce903-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce903-145">JSON representation</span></span>

<span data-ttu-id="ce903-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce903-146">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ce903-147">См. также</span><span class="sxs-lookup"><span data-stu-id="ce903-147">See also</span></span>
- <span data-ttu-id="ce903-148">Поиск [сообщений почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="ce903-148">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="ce903-149">События [календаря поиска](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="ce903-149">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="ce903-150">Поиск контента в SharePoint и OneDrive[(файлы, списки и сайты)](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="ce903-150">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


