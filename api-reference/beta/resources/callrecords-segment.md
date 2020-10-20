---
title: Тип ресурса "сегмент"
description: Тип сегмента
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 84f18568d1890b331d1bedd6d9e7114518fad3cf
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601666"
---
# <a name="segment-resource-type"></a><span data-ttu-id="e0ba7-103">Тип ресурса "сегмент"</span><span class="sxs-lookup"><span data-stu-id="e0ba7-103">segment resource type</span></span>

<span data-ttu-id="e0ba7-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="e0ba7-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0ba7-105">Представляет часть User-User взаимодействия или User-Meeting связи в случае вызова конференции.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="e0ba7-106">Типичный вызов VOIP будет иметь по одному сегменту на сеанс.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="e0ba7-107">В определенных сценариях, таких как звонки по протоколу PSTN, для каждого сеанса будет использоваться несколько сегментов из-за дополнительного обмена данными между серверами, необходимыми для подключения вызова.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="e0ba7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e0ba7-108">Methods</span></span>

<span data-ttu-id="e0ba7-109">Не существует методов для прямого доступа к сегментам.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="e0ba7-110">Для получения сегментов для Каллрекорд используйте API [Get каллрекорд](../api/callrecords-callrecord-get.md) с `$expand=sessions($expand=segments)` API [сеанса или списка](../api/callrecords-session-list.md) `$expand=segments` . [callRecord](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="e0ba7-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e0ba7-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0ba7-111">Properties</span></span>

| <span data-ttu-id="e0ba7-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0ba7-112">Property</span></span>     | <span data-ttu-id="e0ba7-113">Тип</span><span class="sxs-lookup"><span data-stu-id="e0ba7-113">Type</span></span>        | <span data-ttu-id="e0ba7-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e0ba7-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0ba7-115">id</span><span class="sxs-lookup"><span data-stu-id="e0ba7-115">id</span></span>|<span data-ttu-id="e0ba7-116">String</span><span class="sxs-lookup"><span data-stu-id="e0ba7-116">String</span></span>|<span data-ttu-id="e0ba7-117">Уникальный идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-117">Unique identifier for the segment.</span></span> <span data-ttu-id="e0ba7-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-118">Read-only.</span></span>|
|<span data-ttu-id="e0ba7-119">объекта</span><span class="sxs-lookup"><span data-stu-id="e0ba7-119">caller</span></span>|[<span data-ttu-id="e0ba7-120">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="e0ba7-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="e0ba7-121">Конечная точка, которая инициировала этот сегмент.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="e0ba7-122">вызываемого абонента</span><span class="sxs-lookup"><span data-stu-id="e0ba7-122">callee</span></span>|[<span data-ttu-id="e0ba7-123">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="e0ba7-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="e0ba7-124">Конечная точка, которая ответила на этот сегмент.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="e0ba7-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="e0ba7-125">failureInfo</span></span>|[<span data-ttu-id="e0ba7-126">Microsoft. Graph. Каллрекордс. Фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="e0ba7-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="e0ba7-127">Сведения об ошибке, связанные с сегментом, если произошел сбой.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="e0ba7-128">media</span><span class="sxs-lookup"><span data-stu-id="e0ba7-128">media</span></span>|<span data-ttu-id="e0ba7-129">Коллекция [Microsoft. Graph. каллрекордс. Media](callrecords-media.md)</span><span class="sxs-lookup"><span data-stu-id="e0ba7-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="e0ba7-130">Носитель, связанный с этим сегментом.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="e0ba7-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e0ba7-131">startDateTime</span></span>|<span data-ttu-id="e0ba7-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0ba7-132">DateTimeOffset</span></span>|<span data-ttu-id="e0ba7-133">Время в формате UTC, когда начался сегмент.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-133">UTC time when the segment started.</span></span> <span data-ttu-id="e0ba7-134">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0ba7-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e0ba7-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e0ba7-136">endDateTime</span></span>|<span data-ttu-id="e0ba7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0ba7-137">DateTimeOffset</span></span>|<span data-ttu-id="e0ba7-138">Время в формате UTC, когда сегмент закончился.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-138">UTC time when the segment ended.</span></span> <span data-ttu-id="e0ba7-139">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0ba7-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0ba7-141">Связи</span><span class="sxs-lookup"><span data-stu-id="e0ba7-141">Relationships</span></span>

<span data-ttu-id="e0ba7-142">Нет</span><span class="sxs-lookup"><span data-stu-id="e0ba7-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0ba7-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0ba7-143">JSON representation</span></span>

<span data-ttu-id="e0ba7-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0ba7-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "baseType": "",
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

