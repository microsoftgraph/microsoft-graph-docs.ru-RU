---
title: Тип ресурса Session
description: Тип сеанса
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8c1af52332c5650123d604b8e405bf88d0c2f965
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353128"
---
# <a name="session-resource-type"></a><span data-ttu-id="0f731-103">Тип ресурса Session</span><span class="sxs-lookup"><span data-stu-id="0f731-103">session resource type</span></span>

<span data-ttu-id="0f731-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="0f731-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f731-105">Представляет пользовательское взаимодействие с пользователем или собрание пользователя в случае вызова конференции.</span><span class="sxs-lookup"><span data-stu-id="0f731-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="0f731-106">Methods</span><span class="sxs-lookup"><span data-stu-id="0f731-106">Methods</span></span>

<span data-ttu-id="0f731-107">Не существует методов для прямого доступа к сеансам.</span><span class="sxs-lookup"><span data-stu-id="0f731-107">No methods exist to directly access sessions.</span></span> <span data-ttu-id="0f731-108">Используйте API [Get каллрекорд](../api/callrecords-callrecord-get.md) , `$expand=sessions` чтобы получить сеансы для [каллрекорд](callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="0f731-108">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions` to get the sessions for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0f731-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f731-109">Properties</span></span>

| <span data-ttu-id="0f731-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f731-110">Property</span></span>     | <span data-ttu-id="0f731-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0f731-111">Type</span></span>        | <span data-ttu-id="0f731-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0f731-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f731-113">id</span><span class="sxs-lookup"><span data-stu-id="0f731-113">id</span></span>|<span data-ttu-id="0f731-114">string</span><span class="sxs-lookup"><span data-stu-id="0f731-114">string</span></span>|<span data-ttu-id="0f731-115">Уникальный идентификатор сеанса.</span><span class="sxs-lookup"><span data-stu-id="0f731-115">Unique identifier for the session.</span></span> <span data-ttu-id="0f731-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f731-116">Read-only.</span></span>|
|<span data-ttu-id="0f731-117">объекта</span><span class="sxs-lookup"><span data-stu-id="0f731-117">caller</span></span>|[<span data-ttu-id="0f731-118">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="0f731-118">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="0f731-119">Конечная точка, которая инициировала сеанс.</span><span class="sxs-lookup"><span data-stu-id="0f731-119">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="0f731-120">вызываемого абонента</span><span class="sxs-lookup"><span data-stu-id="0f731-120">callee</span></span>|[<span data-ttu-id="0f731-121">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="0f731-121">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="0f731-122">Конечная точка, которая ответила на сеанс.</span><span class="sxs-lookup"><span data-stu-id="0f731-122">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="0f731-123">failureInfo</span><span class="sxs-lookup"><span data-stu-id="0f731-123">failureInfo</span></span>|[<span data-ttu-id="0f731-124">Microsoft. Graph. Каллрекордс. Фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="0f731-124">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="0f731-125">Сведения о сбое, связанные с сеансом в случае сбоя сеанса.</span><span class="sxs-lookup"><span data-stu-id="0f731-125">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="0f731-126">модальности</span><span class="sxs-lookup"><span data-stu-id="0f731-126">modalities</span></span>|<span data-ttu-id="0f731-127">коллекция Microsoft. Graph. Каллрекордс. Modal</span><span class="sxs-lookup"><span data-stu-id="0f731-127">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="0f731-128">Список модальности, присутствующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="0f731-128">List of modalities present in the session.</span></span> <span data-ttu-id="0f731-129">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0f731-129">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0f731-130">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0f731-130">startDateTime</span></span>|<span data-ttu-id="0f731-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f731-131">DateTimeOffset</span></span>|<span data-ttu-id="0f731-132">UTC Фиме, когда первый пользователь присоединился к сеансу.</span><span class="sxs-lookup"><span data-stu-id="0f731-132">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="0f731-133">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0f731-133">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f731-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0f731-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0f731-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0f731-135">endDateTime</span></span>|<span data-ttu-id="0f731-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f731-136">DateTimeOffset</span></span>|<span data-ttu-id="0f731-137">Время в формате UTC, когда последний пользователь оставил сеанс.</span><span class="sxs-lookup"><span data-stu-id="0f731-137">UTC time when the last user left the session.</span></span> <span data-ttu-id="0f731-138">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0f731-138">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f731-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0f731-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="0f731-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="0f731-140">Relationships</span></span>

| <span data-ttu-id="0f731-141">Связь</span><span class="sxs-lookup"><span data-stu-id="0f731-141">Relationship</span></span> | <span data-ttu-id="0f731-142">Тип</span><span class="sxs-lookup"><span data-stu-id="0f731-142">Type</span></span>        | <span data-ttu-id="0f731-143">Описание</span><span class="sxs-lookup"><span data-stu-id="0f731-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f731-144">segments</span><span class="sxs-lookup"><span data-stu-id="0f731-144">segments</span></span>|<span data-ttu-id="0f731-145">Коллекция [Microsoft. Graph. каллрекордс. segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="0f731-145">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="0f731-146">Список сегментов, участвующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="0f731-146">The list of segments involved in the session.</span></span> <span data-ttu-id="0f731-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f731-147">Read-only.</span></span> <span data-ttu-id="0f731-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0f731-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f731-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f731-149">JSON representation</span></span>

<span data-ttu-id="0f731-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f731-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "modalities": ["string"],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "session resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->