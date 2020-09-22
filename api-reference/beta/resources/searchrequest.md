---
title: Тип ресурса Сеарчрекуест
description: Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fac759f190f193fb2fe37e769feedc1164fc3f95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973742"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="1c4a8-104">Тип ресурса Сеарчрекуест</span><span class="sxs-lookup"><span data-stu-id="1c4a8-104">searchRequest resource type</span></span>

<span data-ttu-id="1c4a8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c4a8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c4a8-106">Запрос поиска, отправляемый конечной точке запроса.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-106">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="1c4a8-107">Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-107">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="1c4a8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c4a8-108">Properties</span></span>

| <span data-ttu-id="1c4a8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c4a8-109">Property</span></span>     | <span data-ttu-id="1c4a8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1c4a8-110">Type</span></span>        | <span data-ttu-id="1c4a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1c4a8-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c4a8-112">stored_fields</span><span class="sxs-lookup"><span data-stu-id="1c4a8-112">stored_fields</span></span>|<span data-ttu-id="1c4a8-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1c4a8-113">String collection</span></span> |<span data-ttu-id="1c4a8-114">Содержит поля, возвращаемые для объекта еарч _so урцес.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-114">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="1c4a8-115">Обратите внимание, что этот параметр применяется, только если `externalItem` в отклике указан тип EntityType =.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-115">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="1c4a8-116">contentSources</span><span class="sxs-lookup"><span data-stu-id="1c4a8-116">contentSources</span></span>|<span data-ttu-id="1c4a8-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1c4a8-117">String collection</span></span>|<span data-ttu-id="1c4a8-118">Содержит подключение, которое необходимо задать.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-118">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="1c4a8-119">В соответствии со следующим форматом: `/external/connections/connectionid` где `connectionid` коннектионид был определен в администрировании соединителей</span><span class="sxs-lookup"><span data-stu-id="1c4a8-119">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="1c4a8-120">Note contentSource применяется только в том случае, если entityType = `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="1c4a8-120">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="1c4a8-121">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="1c4a8-121">enableTopResults</span></span>|<span data-ttu-id="1c4a8-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c4a8-122">Boolean</span></span>|<span data-ttu-id="1c4a8-123">Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее актуальны</span><span class="sxs-lookup"><span data-stu-id="1c4a8-123">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="1c4a8-124">Это относится только к типу entityType = `message` .</span><span class="sxs-lookup"><span data-stu-id="1c4a8-124">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="1c4a8-125">entityTypes</span><span class="sxs-lookup"><span data-stu-id="1c4a8-125">entityTypes</span></span>|<span data-ttu-id="1c4a8-126">Коллекция `entityType`</span><span class="sxs-lookup"><span data-stu-id="1c4a8-126">`entityType` collection</span></span>| <span data-ttu-id="1c4a8-127">Возможные значения: `event`, `message`, `driveItem`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-127">Possible values are: `event`, `message`, `driveItem`, `externalItem`.</span></span>|
|<span data-ttu-id="1c4a8-128">from</span><span class="sxs-lookup"><span data-stu-id="1c4a8-128">from</span></span>|<span data-ttu-id="1c4a8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="1c4a8-129">Int32</span></span>|<span data-ttu-id="1c4a8-130">Задает смещение результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-130">Specifies the offset for the search results.</span></span> <span data-ttu-id="1c4a8-131">Смещение 0 возвращает самый первый результат.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-131">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="1c4a8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c4a8-132">query</span></span>|[<span data-ttu-id="1c4a8-133">searchQuery</span><span class="sxs-lookup"><span data-stu-id="1c4a8-133">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="1c4a8-134">Содержит термины запроса.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-134">Contains the query terms.</span></span>|
|<span data-ttu-id="1c4a8-135">size</span><span class="sxs-lookup"><span data-stu-id="1c4a8-135">size</span></span>|<span data-ttu-id="1c4a8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1c4a8-136">Int32</span></span>|<span data-ttu-id="1c4a8-137">Размер извлекаемой страницы.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-137">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c4a8-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c4a8-138">JSON representation</span></span>

<span data-ttu-id="1c4a8-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c4a8-139">The following is a JSON representation of the resource.</span></span>

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


