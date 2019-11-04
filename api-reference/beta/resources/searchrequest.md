---
title: Тип ресурса Сеарчрекуест
description: Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 22efb3e00689daad5c914d770a7cd0d41b3e35b7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939133"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="45604-104">Тип ресурса Сеарчрекуест</span><span class="sxs-lookup"><span data-stu-id="45604-104">searchRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45604-105">Запрос поиска, отправляемый конечной точке запроса.</span><span class="sxs-lookup"><span data-stu-id="45604-105">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="45604-106">Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="45604-106">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

## <a name="properties"></a><span data-ttu-id="45604-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="45604-107">Properties</span></span>

| <span data-ttu-id="45604-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="45604-108">Property</span></span>     | <span data-ttu-id="45604-109">Тип</span><span class="sxs-lookup"><span data-stu-id="45604-109">Type</span></span>        | <span data-ttu-id="45604-110">Описание</span><span class="sxs-lookup"><span data-stu-id="45604-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="45604-111">stored_fields</span><span class="sxs-lookup"><span data-stu-id="45604-111">stored_fields</span></span>|<span data-ttu-id="45604-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="45604-112">String collection</span></span> |<span data-ttu-id="45604-113">Содержит поля, возвращаемые для объекта еарч _so урцес.</span><span class="sxs-lookup"><span data-stu-id="45604-113">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="45604-114">Обратите внимание, что этот параметр применяется`externalItem` , только если в отклике указан тип EntityType =.</span><span class="sxs-lookup"><span data-stu-id="45604-114">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="45604-115">контентсаурцес</span><span class="sxs-lookup"><span data-stu-id="45604-115">contentSources</span></span>|<span data-ttu-id="45604-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="45604-116">String collection</span></span>|<span data-ttu-id="45604-117">Содержит подключение, которое необходимо задать.</span><span class="sxs-lookup"><span data-stu-id="45604-117">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="45604-118">В соответствии со следующим `/external/connections/connectionid` форматом `connectionid` : где Коннектионид был определен в администрировании соединителей</span><span class="sxs-lookup"><span data-stu-id="45604-118">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="45604-119">Note contentSource применяется только в том случае,`externalItem`если EntityType =.</span><span class="sxs-lookup"><span data-stu-id="45604-119">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="45604-120">енаблетопресултс</span><span class="sxs-lookup"><span data-stu-id="45604-120">enableTopResults</span></span>|<span data-ttu-id="45604-121">Логический</span><span class="sxs-lookup"><span data-stu-id="45604-121">Boolean</span></span>|<span data-ttu-id="45604-122">Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее актуальны</span><span class="sxs-lookup"><span data-stu-id="45604-122">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="45604-123">Это относится только к типу entityType =`message`.</span><span class="sxs-lookup"><span data-stu-id="45604-123">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="45604-124">entityTypes</span><span class="sxs-lookup"><span data-stu-id="45604-124">entityTypes</span></span>|<span data-ttu-id="45604-125">Коллекция `entityType`</span><span class="sxs-lookup"><span data-stu-id="45604-125">`entityType` collection</span></span>| <span data-ttu-id="45604-126">Возможные значения: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="45604-126">Possible values are: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span></span>|
|<span data-ttu-id="45604-127">from</span><span class="sxs-lookup"><span data-stu-id="45604-127">from</span></span>|<span data-ttu-id="45604-128">Int32</span><span class="sxs-lookup"><span data-stu-id="45604-128">Int32</span></span>|<span data-ttu-id="45604-129">Задает смещение результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="45604-129">Specifies the offset for the search results.</span></span> <span data-ttu-id="45604-130">Смещение 0 возвращает самый первый результат.</span><span class="sxs-lookup"><span data-stu-id="45604-130">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="45604-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="45604-131">query</span></span>|[<span data-ttu-id="45604-132">searchQuery</span><span class="sxs-lookup"><span data-stu-id="45604-132">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="45604-133">Содержит термины запроса.</span><span class="sxs-lookup"><span data-stu-id="45604-133">Contains the query terms.</span></span>|
|<span data-ttu-id="45604-134">size</span><span class="sxs-lookup"><span data-stu-id="45604-134">size</span></span>|<span data-ttu-id="45604-135">Int32</span><span class="sxs-lookup"><span data-stu-id="45604-135">Int32</span></span>|<span data-ttu-id="45604-136">Размер извлекаемой страницы.</span><span class="sxs-lookup"><span data-stu-id="45604-136">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45604-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45604-137">JSON representation</span></span>

<span data-ttu-id="45604-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45604-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "stored_fields": ["String"],
  "contentSources": ["String"],
  "entityTypes": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "enableTopResults": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
