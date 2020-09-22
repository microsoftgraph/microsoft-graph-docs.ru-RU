---
title: Тип ресурса "сегмент"
description: Тип сегмента
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9b722b6e306c4eb52de19827580b1b0d2807d0e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069339"
---
# <a name="segment-resource-type"></a><span data-ttu-id="e9e43-103">Тип ресурса "сегмент"</span><span class="sxs-lookup"><span data-stu-id="e9e43-103">segment resource type</span></span>

<span data-ttu-id="e9e43-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="e9e43-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="e9e43-105">Представляет часть взаимодействия пользователя с пользователем или собрание по телефону в случае Конференции.</span><span class="sxs-lookup"><span data-stu-id="e9e43-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="e9e43-106">Типичный вызов VOIP будет иметь по одному сегменту на сеанс.</span><span class="sxs-lookup"><span data-stu-id="e9e43-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="e9e43-107">В определенных сценариях, таких как звонки по протоколу PSTN, для каждого сеанса будет использоваться несколько сегментов из-за дополнительного обмена данными между серверами, необходимыми для подключения вызова.</span><span class="sxs-lookup"><span data-stu-id="e9e43-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="e9e43-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e9e43-108">Methods</span></span>

<span data-ttu-id="e9e43-109">Не существует методов для прямого доступа к сегментам.</span><span class="sxs-lookup"><span data-stu-id="e9e43-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="e9e43-110">Для получения сегментов для Каллрекорд используйте API [Get каллрекорд](../api/callrecords-callrecord-get.md) с `$expand=sessions($expand=segments)` API [сеанса или списка](../api/callrecords-session-list.md) `$expand=segments` . [callRecord](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="e9e43-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e9e43-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9e43-111">Properties</span></span>

| <span data-ttu-id="e9e43-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9e43-112">Property</span></span>     | <span data-ttu-id="e9e43-113">Тип</span><span class="sxs-lookup"><span data-stu-id="e9e43-113">Type</span></span>        | <span data-ttu-id="e9e43-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e43-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9e43-115">id</span><span class="sxs-lookup"><span data-stu-id="e9e43-115">id</span></span>|<span data-ttu-id="e9e43-116">Строка</span><span class="sxs-lookup"><span data-stu-id="e9e43-116">String</span></span>|<span data-ttu-id="e9e43-117">Уникальный идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="e9e43-117">Unique identifier for the segment.</span></span> <span data-ttu-id="e9e43-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9e43-118">Read-only.</span></span>|
|<span data-ttu-id="e9e43-119">объекта</span><span class="sxs-lookup"><span data-stu-id="e9e43-119">caller</span></span>|[<span data-ttu-id="e9e43-120">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="e9e43-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="e9e43-121">Конечная точка, которая инициировала этот сегмент.</span><span class="sxs-lookup"><span data-stu-id="e9e43-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="e9e43-122">вызываемого абонента</span><span class="sxs-lookup"><span data-stu-id="e9e43-122">callee</span></span>|[<span data-ttu-id="e9e43-123">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="e9e43-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="e9e43-124">Конечная точка, которая ответила на этот сегмент.</span><span class="sxs-lookup"><span data-stu-id="e9e43-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="e9e43-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="e9e43-125">failureInfo</span></span>|[<span data-ttu-id="e9e43-126">Microsoft. Graph. Каллрекордс. Фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="e9e43-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="e9e43-127">Сведения об ошибке, связанные с сегментом, если произошел сбой.</span><span class="sxs-lookup"><span data-stu-id="e9e43-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="e9e43-128">media</span><span class="sxs-lookup"><span data-stu-id="e9e43-128">media</span></span>|<span data-ttu-id="e9e43-129">Коллекция [Microsoft. Graph. каллрекордс. Media](callrecords-media.md)</span><span class="sxs-lookup"><span data-stu-id="e9e43-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="e9e43-130">Носитель, связанный с этим сегментом.</span><span class="sxs-lookup"><span data-stu-id="e9e43-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="e9e43-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e9e43-131">startDateTime</span></span>|<span data-ttu-id="e9e43-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9e43-132">DateTimeOffset</span></span>|<span data-ttu-id="e9e43-133">Время в формате UTC, когда начался сегмент.</span><span class="sxs-lookup"><span data-stu-id="e9e43-133">UTC time when the segment started.</span></span> <span data-ttu-id="e9e43-134">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e9e43-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9e43-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e9e43-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e9e43-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e9e43-136">endDateTime</span></span>|<span data-ttu-id="e9e43-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9e43-137">DateTimeOffset</span></span>|<span data-ttu-id="e9e43-138">Время в формате UTC, когда сегмент закончился.</span><span class="sxs-lookup"><span data-stu-id="e9e43-138">UTC time when the segment ended.</span></span> <span data-ttu-id="e9e43-139">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e9e43-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9e43-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e9e43-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9e43-141">Связи</span><span class="sxs-lookup"><span data-stu-id="e9e43-141">Relationships</span></span>

<span data-ttu-id="e9e43-142">Нет</span><span class="sxs-lookup"><span data-stu-id="e9e43-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9e43-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9e43-143">JSON representation</span></span>

<span data-ttu-id="e9e43-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9e43-144">The following is a JSON representation of the resource.</span></span>

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
