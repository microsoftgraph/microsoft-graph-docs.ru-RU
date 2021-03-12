---
title: Тип ресурса сеанса
description: Тип сеанса
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 837e72c52002c0084994b74d3991c69272bdf870
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721805"
---
# <a name="session-resource-type"></a><span data-ttu-id="4f3a8-103">Тип ресурса сеанса</span><span class="sxs-lookup"><span data-stu-id="4f3a8-103">session resource type</span></span>

<span data-ttu-id="4f3a8-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="4f3a8-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="4f3a8-105">Представляет собой User-User или User-Meeting связи в случае конференц-звонка.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="4f3a8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4f3a8-106">Methods</span></span>

| <span data-ttu-id="4f3a8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4f3a8-107">Method</span></span>       | <span data-ttu-id="4f3a8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4f3a8-108">Return Type</span></span> | <span data-ttu-id="4f3a8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4f3a8-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4f3a8-110">Перечисление сеансов</span><span class="sxs-lookup"><span data-stu-id="4f3a8-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="4f3a8-111">[коллекция microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="4f3a8-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="4f3a8-112">Извлечение списка сеансов, связанных с [объектом callRecord.](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="4f3a8-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="4f3a8-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f3a8-113">Properties</span></span>

| <span data-ttu-id="4f3a8-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f3a8-114">Property</span></span>     | <span data-ttu-id="4f3a8-115">Тип</span><span class="sxs-lookup"><span data-stu-id="4f3a8-115">Type</span></span>        | <span data-ttu-id="4f3a8-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4f3a8-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f3a8-117">id</span><span class="sxs-lookup"><span data-stu-id="4f3a8-117">id</span></span>|<span data-ttu-id="4f3a8-118">string</span><span class="sxs-lookup"><span data-stu-id="4f3a8-118">string</span></span>|<span data-ttu-id="4f3a8-119">Уникальный идентификатор для сеанса.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-119">Unique identifier for the session.</span></span> <span data-ttu-id="4f3a8-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-120">Read-only.</span></span>|
|<span data-ttu-id="4f3a8-121">вызываемая</span><span class="sxs-lookup"><span data-stu-id="4f3a8-121">caller</span></span>|[<span data-ttu-id="4f3a8-122">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="4f3a8-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="4f3a8-123">Конечная точка, которая инициировала сеанс.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="4f3a8-124">вызываемая</span><span class="sxs-lookup"><span data-stu-id="4f3a8-124">callee</span></span>|[<span data-ttu-id="4f3a8-125">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="4f3a8-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="4f3a8-126">Конечная точка, которая ответила на сеанс.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="4f3a8-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="4f3a8-127">failureInfo</span></span>|[<span data-ttu-id="4f3a8-128">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="4f3a8-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="4f3a8-129">Сведения о сбоях, связанных с сеансом, в случае сбоя сеанса.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="4f3a8-130">модальности</span><span class="sxs-lookup"><span data-stu-id="4f3a8-130">modalities</span></span>|<span data-ttu-id="4f3a8-131">коллекция microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="4f3a8-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="4f3a8-132">Список способов, присутствующих на сеансе.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-132">List of modalities present in the session.</span></span> <span data-ttu-id="4f3a8-133">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4f3a8-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4f3a8-134">startDateTime</span></span>|<span data-ttu-id="4f3a8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f3a8-135">DateTimeOffset</span></span>|<span data-ttu-id="4f3a8-136">Время UTC, когда первый пользователь присоединился к сеансу.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-136">UTC time when the first user joined the session.</span></span> <span data-ttu-id="4f3a8-137">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f3a8-138">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="4f3a8-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4f3a8-139">endDateTime</span></span>|<span data-ttu-id="4f3a8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f3a8-140">DateTimeOffset</span></span>|<span data-ttu-id="4f3a8-141">Время UTC, когда последний пользователь покинул сеанс.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="4f3a8-142">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f3a8-143">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|


## <a name="relationships"></a><span data-ttu-id="4f3a8-144">Связи</span><span class="sxs-lookup"><span data-stu-id="4f3a8-144">Relationships</span></span>

| <span data-ttu-id="4f3a8-145">Связь</span><span class="sxs-lookup"><span data-stu-id="4f3a8-145">Relationship</span></span> | <span data-ttu-id="4f3a8-146">Тип</span><span class="sxs-lookup"><span data-stu-id="4f3a8-146">Type</span></span>        | <span data-ttu-id="4f3a8-147">Описание</span><span class="sxs-lookup"><span data-stu-id="4f3a8-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f3a8-148">segments</span><span class="sxs-lookup"><span data-stu-id="4f3a8-148">segments</span></span>|<span data-ttu-id="4f3a8-149">[коллекция microsoft.graph.callRecords.segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="4f3a8-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="4f3a8-150">Список сегментов, участвующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-150">The list of segments involved in the session.</span></span> <span data-ttu-id="4f3a8-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-151">Read-only.</span></span> <span data-ttu-id="4f3a8-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f3a8-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f3a8-153">JSON representation</span></span>

<span data-ttu-id="4f3a8-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f3a8-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
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
