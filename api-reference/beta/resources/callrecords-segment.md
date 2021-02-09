---
title: тип ресурса segment
description: Тип сегмента
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ef965bcfb10eeafd0a2c4f58351aa74650abcd05
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159642"
---
# <a name="segment-resource-type"></a><span data-ttu-id="8c310-103">тип ресурса segment</span><span class="sxs-lookup"><span data-stu-id="8c310-103">segment resource type</span></span>

<span data-ttu-id="8c310-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="8c310-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c310-105">Представляет часть User-User или User-Meeting связи в случае конференц-связи.</span><span class="sxs-lookup"><span data-stu-id="8c310-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="8c310-106">Типичный вызов VOIP будет иметь один сегмент на сеанс.</span><span class="sxs-lookup"><span data-stu-id="8c310-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="8c310-107">В некоторых сценариях, таких как вызовы STN, в сеансе будет несколько сегментов, так как для подключения вызова требуется дополнительная связь "сервер-сервер".</span><span class="sxs-lookup"><span data-stu-id="8c310-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="8c310-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8c310-108">Methods</span></span>

<span data-ttu-id="8c310-109">Методы прямого доступа к сегментам не существуют.</span><span class="sxs-lookup"><span data-stu-id="8c310-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="8c310-110">Используйте API [Get callRecord](../api/callrecords-callrecord-get.md) с API или API сеанса списка, чтобы получить сегменты `$expand=sessions($expand=segments)` для [](../api/callrecords-session-list.md) `$expand=segments` [callRecord](callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="8c310-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8c310-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c310-111">Properties</span></span>

| <span data-ttu-id="8c310-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c310-112">Property</span></span>     | <span data-ttu-id="8c310-113">Тип</span><span class="sxs-lookup"><span data-stu-id="8c310-113">Type</span></span>        | <span data-ttu-id="8c310-114">Описание</span><span class="sxs-lookup"><span data-stu-id="8c310-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c310-115">id</span><span class="sxs-lookup"><span data-stu-id="8c310-115">id</span></span>|<span data-ttu-id="8c310-116">String</span><span class="sxs-lookup"><span data-stu-id="8c310-116">String</span></span>|<span data-ttu-id="8c310-117">Уникальный идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="8c310-117">Unique identifier for the segment.</span></span> <span data-ttu-id="8c310-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c310-118">Read-only.</span></span>|
|<span data-ttu-id="8c310-119">вызываемая</span><span class="sxs-lookup"><span data-stu-id="8c310-119">caller</span></span>|[<span data-ttu-id="8c310-120">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="8c310-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="8c310-121">Конечная точка, которая инициировала этот сегмент.</span><span class="sxs-lookup"><span data-stu-id="8c310-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="8c310-122">вызываемая</span><span class="sxs-lookup"><span data-stu-id="8c310-122">callee</span></span>|[<span data-ttu-id="8c310-123">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="8c310-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="8c310-124">Конечная точка, ответив на этот сегмент.</span><span class="sxs-lookup"><span data-stu-id="8c310-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="8c310-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="8c310-125">failureInfo</span></span>|[<span data-ttu-id="8c310-126">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="8c310-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="8c310-127">Сведения о сбое, связанные с сегментом в случае сбоя.</span><span class="sxs-lookup"><span data-stu-id="8c310-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="8c310-128">media</span><span class="sxs-lookup"><span data-stu-id="8c310-128">media</span></span>|<span data-ttu-id="8c310-129">[Коллекция microsoft.graph.callRecords.media](callrecords-media.md)</span><span class="sxs-lookup"><span data-stu-id="8c310-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="8c310-130">Носители, связанные с этим сегментом.</span><span class="sxs-lookup"><span data-stu-id="8c310-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="8c310-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8c310-131">startDateTime</span></span>|<span data-ttu-id="8c310-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c310-132">DateTimeOffset</span></span>|<span data-ttu-id="8c310-133">Время начала сегмента в UTC.</span><span class="sxs-lookup"><span data-stu-id="8c310-133">UTC time when the segment started.</span></span> <span data-ttu-id="8c310-134">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8c310-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8c310-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8c310-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8c310-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8c310-136">endDateTime</span></span>|<span data-ttu-id="8c310-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c310-137">DateTimeOffset</span></span>|<span data-ttu-id="8c310-138">Время окончания сегмента в UTC.</span><span class="sxs-lookup"><span data-stu-id="8c310-138">UTC time when the segment ended.</span></span> <span data-ttu-id="8c310-139">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8c310-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8c310-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8c310-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c310-141">Связи</span><span class="sxs-lookup"><span data-stu-id="8c310-141">Relationships</span></span>

<span data-ttu-id="8c310-142">Нет</span><span class="sxs-lookup"><span data-stu-id="8c310-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c310-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c310-143">JSON representation</span></span>

<span data-ttu-id="8c310-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c310-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "media": [{"@odata.type": "microsoft.graph.callRecords.media"}],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "segment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

