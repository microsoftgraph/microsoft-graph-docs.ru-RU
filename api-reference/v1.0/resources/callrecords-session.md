---
title: Тип ресурса session
description: Тип сеанса
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9a61fca17c8b04e9f5c236d0104b2b93f1a6704e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153497"
---
# <a name="session-resource-type"></a><span data-ttu-id="3caef-103">Тип ресурса session</span><span class="sxs-lookup"><span data-stu-id="3caef-103">session resource type</span></span>

<span data-ttu-id="3caef-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="3caef-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="3caef-105">Представляет User-User или User-Meeting в случае конференц-связи.</span><span class="sxs-lookup"><span data-stu-id="3caef-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="3caef-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3caef-106">Methods</span></span>

| <span data-ttu-id="3caef-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3caef-107">Method</span></span>       | <span data-ttu-id="3caef-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3caef-108">Return Type</span></span> | <span data-ttu-id="3caef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3caef-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3caef-110">Перечисление сеансов</span><span class="sxs-lookup"><span data-stu-id="3caef-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="3caef-111">[коллекция microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="3caef-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="3caef-112">Получить список сеансов, связанных с [объектом callRecord.](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="3caef-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="3caef-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="3caef-113">Properties</span></span>

| <span data-ttu-id="3caef-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="3caef-114">Property</span></span>     | <span data-ttu-id="3caef-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3caef-115">Type</span></span>        | <span data-ttu-id="3caef-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3caef-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3caef-117">id</span><span class="sxs-lookup"><span data-stu-id="3caef-117">id</span></span>|<span data-ttu-id="3caef-118">string</span><span class="sxs-lookup"><span data-stu-id="3caef-118">string</span></span>|<span data-ttu-id="3caef-119">Уникальный идентификатор сеанса.</span><span class="sxs-lookup"><span data-stu-id="3caef-119">Unique identifier for the session.</span></span> <span data-ttu-id="3caef-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3caef-120">Read-only.</span></span>|
|<span data-ttu-id="3caef-121">вызываемая</span><span class="sxs-lookup"><span data-stu-id="3caef-121">caller</span></span>|[<span data-ttu-id="3caef-122">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="3caef-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="3caef-123">Конечная точка, которая инициировала сеанс.</span><span class="sxs-lookup"><span data-stu-id="3caef-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="3caef-124">вызываемая</span><span class="sxs-lookup"><span data-stu-id="3caef-124">callee</span></span>|[<span data-ttu-id="3caef-125">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="3caef-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="3caef-126">Конечная точка, ответив на сеанс.</span><span class="sxs-lookup"><span data-stu-id="3caef-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="3caef-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="3caef-127">failureInfo</span></span>|[<span data-ttu-id="3caef-128">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="3caef-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="3caef-129">Сведения о сбое, связанном с сеансом, если сеанс не был сбой.</span><span class="sxs-lookup"><span data-stu-id="3caef-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="3caef-130">модальности</span><span class="sxs-lookup"><span data-stu-id="3caef-130">modalities</span></span>|<span data-ttu-id="3caef-131">Коллекция microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="3caef-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="3caef-132">Список модальных режимов, присутствующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="3caef-132">List of modalities present in the session.</span></span> <span data-ttu-id="3caef-133">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3caef-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3caef-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3caef-134">startDateTime</span></span>|<span data-ttu-id="3caef-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3caef-135">DateTimeOffset</span></span>|<span data-ttu-id="3caef-136">Время в UTC, когда первый пользователь присоединился к сеансу.</span><span class="sxs-lookup"><span data-stu-id="3caef-136">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="3caef-137">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3caef-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3caef-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3caef-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3caef-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3caef-139">endDateTime</span></span>|<span data-ttu-id="3caef-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3caef-140">DateTimeOffset</span></span>|<span data-ttu-id="3caef-141">Время в UTC, когда последний пользователь покинул сеанс.</span><span class="sxs-lookup"><span data-stu-id="3caef-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="3caef-142">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3caef-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3caef-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3caef-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="3caef-144">Связи</span><span class="sxs-lookup"><span data-stu-id="3caef-144">Relationships</span></span>

| <span data-ttu-id="3caef-145">Связь</span><span class="sxs-lookup"><span data-stu-id="3caef-145">Relationship</span></span> | <span data-ttu-id="3caef-146">Тип</span><span class="sxs-lookup"><span data-stu-id="3caef-146">Type</span></span>        | <span data-ttu-id="3caef-147">Описание</span><span class="sxs-lookup"><span data-stu-id="3caef-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3caef-148">segments</span><span class="sxs-lookup"><span data-stu-id="3caef-148">segments</span></span>|<span data-ttu-id="3caef-149">[Коллекция microsoft.graph.callRecords.segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="3caef-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="3caef-150">Список сегментов, участвующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="3caef-150">The list of segments involved in the session.</span></span> <span data-ttu-id="3caef-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3caef-151">Read-only.</span></span> <span data-ttu-id="3caef-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3caef-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3caef-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3caef-153">JSON representation</span></span>

<span data-ttu-id="3caef-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3caef-154">The following is a JSON representation of the resource.</span></span>

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
