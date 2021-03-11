---
title: тип ресурсов сегмента
description: Тип сегмента
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5cb95c665ed3967aeb9b18fcefd262ad52490306
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720230"
---
# <a name="segment-resource-type"></a><span data-ttu-id="9dc7d-103">тип ресурсов сегмента</span><span class="sxs-lookup"><span data-stu-id="9dc7d-103">segment resource type</span></span>

<span data-ttu-id="9dc7d-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="9dc7d-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dc7d-105">Представляет часть User-User или User-Meeting связи в случае конференц-звонка.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="9dc7d-106">Типичный вызов VOIP будет иметь один сегмент в сеансе.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="9dc7d-107">В некоторых сценариях, таких как вызовы PSTN, в сеансе будет несколько сегментов из-за дополнительной связи между сервером и сервером, необходимой для подключения вызова.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="9dc7d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="9dc7d-108">Methods</span></span>

<span data-ttu-id="9dc7d-109">Нет методов непосредственного доступа к сегментам.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="9dc7d-110">Чтобы получить сегменты [для callRecord,](../api/callrecords-callrecord-get.md) используйте api Get `$expand=sessions($expand=segments)` [](../api/callrecords-session-list.md) `$expand=segments` [callRecord](callrecords-callrecord.md)с api или API сеанса List.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9dc7d-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dc7d-111">Properties</span></span>

| <span data-ttu-id="9dc7d-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dc7d-112">Property</span></span>     | <span data-ttu-id="9dc7d-113">Тип</span><span class="sxs-lookup"><span data-stu-id="9dc7d-113">Type</span></span>        | <span data-ttu-id="9dc7d-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc7d-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9dc7d-115">id</span><span class="sxs-lookup"><span data-stu-id="9dc7d-115">id</span></span>|<span data-ttu-id="9dc7d-116">String</span><span class="sxs-lookup"><span data-stu-id="9dc7d-116">String</span></span>|<span data-ttu-id="9dc7d-117">Уникальный идентификатор для сегмента.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-117">Unique identifier for the segment.</span></span> <span data-ttu-id="9dc7d-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-118">Read-only.</span></span>|
|<span data-ttu-id="9dc7d-119">вызываемая</span><span class="sxs-lookup"><span data-stu-id="9dc7d-119">caller</span></span>|[<span data-ttu-id="9dc7d-120">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="9dc7d-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="9dc7d-121">Конечная точка, которая инициировала этот сегмент.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="9dc7d-122">вызываемая</span><span class="sxs-lookup"><span data-stu-id="9dc7d-122">callee</span></span>|[<span data-ttu-id="9dc7d-123">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="9dc7d-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="9dc7d-124">Конечная точка, которая ответила на этот сегмент.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="9dc7d-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="9dc7d-125">failureInfo</span></span>|[<span data-ttu-id="9dc7d-126">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="9dc7d-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="9dc7d-127">Сведения о сбое, связанные с сегментом в случае сбоя.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="9dc7d-128">мультимедиа</span><span class="sxs-lookup"><span data-stu-id="9dc7d-128">media</span></span>|<span data-ttu-id="9dc7d-129">[коллекция microsoft.graph.callRecords.media](callrecords-media.md)</span><span class="sxs-lookup"><span data-stu-id="9dc7d-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="9dc7d-130">Носители, связанные с этим сегментом.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="9dc7d-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc7d-131">startDateTime</span></span>|<span data-ttu-id="9dc7d-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc7d-132">DateTimeOffset</span></span>|<span data-ttu-id="9dc7d-133">Время UTC, когда начался сегмент.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-133">UTC time when the segment started.</span></span> <span data-ttu-id="9dc7d-134">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9dc7d-135">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="9dc7d-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc7d-136">endDateTime</span></span>|<span data-ttu-id="9dc7d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc7d-137">DateTimeOffset</span></span>|<span data-ttu-id="9dc7d-138">Время UTC после окончания сегмента.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-138">UTC time when the segment ended.</span></span> <span data-ttu-id="9dc7d-139">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9dc7d-140">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dc7d-141">Связи</span><span class="sxs-lookup"><span data-stu-id="9dc7d-141">Relationships</span></span>

<span data-ttu-id="9dc7d-142">Нет</span><span class="sxs-lookup"><span data-stu-id="9dc7d-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dc7d-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dc7d-143">JSON representation</span></span>

<span data-ttu-id="9dc7d-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dc7d-144">The following is a JSON representation of the resource.</span></span>

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

