---
title: Тип ресурса session
description: Тип сеанса
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 263ad4d249535fc9255507e398b29d69b34bbb7d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155575"
---
# <a name="session-resource-type"></a><span data-ttu-id="3ebe9-103">Тип ресурса session</span><span class="sxs-lookup"><span data-stu-id="3ebe9-103">session resource type</span></span>

<span data-ttu-id="3ebe9-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="3ebe9-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ebe9-105">Представляет User-User или User-Meeting в случае конференц-связи.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="3ebe9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3ebe9-106">Methods</span></span>

| <span data-ttu-id="3ebe9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3ebe9-107">Method</span></span>       | <span data-ttu-id="3ebe9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ebe9-108">Return Type</span></span> | <span data-ttu-id="3ebe9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3ebe9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3ebe9-110">Перечисление сеансов</span><span class="sxs-lookup"><span data-stu-id="3ebe9-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="3ebe9-111">[коллекция microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="3ebe9-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="3ebe9-112">Получить список сеансов, связанных с [объектом callRecord.](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="3ebe9-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="3ebe9-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ebe9-113">Properties</span></span>

| <span data-ttu-id="3ebe9-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ebe9-114">Property</span></span>     | <span data-ttu-id="3ebe9-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3ebe9-115">Type</span></span>        | <span data-ttu-id="3ebe9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3ebe9-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ebe9-117">id</span><span class="sxs-lookup"><span data-stu-id="3ebe9-117">id</span></span>|<span data-ttu-id="3ebe9-118">string</span><span class="sxs-lookup"><span data-stu-id="3ebe9-118">string</span></span>|<span data-ttu-id="3ebe9-119">Уникальный идентификатор сеанса.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-119">Unique identifier for the session.</span></span> <span data-ttu-id="3ebe9-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-120">Read-only.</span></span>|
|<span data-ttu-id="3ebe9-121">вызываемая</span><span class="sxs-lookup"><span data-stu-id="3ebe9-121">caller</span></span>|[<span data-ttu-id="3ebe9-122">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="3ebe9-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="3ebe9-123">Конечная точка, которая инициировала сеанс.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="3ebe9-124">вызываемая</span><span class="sxs-lookup"><span data-stu-id="3ebe9-124">callee</span></span>|[<span data-ttu-id="3ebe9-125">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="3ebe9-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="3ebe9-126">Конечная точка, ответив на сеанс.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="3ebe9-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="3ebe9-127">failureInfo</span></span>|[<span data-ttu-id="3ebe9-128">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="3ebe9-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="3ebe9-129">Сведения о сбое, связанном с сеансом, если сеанс не был сбой.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="3ebe9-130">модальности</span><span class="sxs-lookup"><span data-stu-id="3ebe9-130">modalities</span></span>|<span data-ttu-id="3ebe9-131">Коллекция microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="3ebe9-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="3ebe9-132">Список модальных режимов, присутствующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-132">List of modalities present in the session.</span></span> <span data-ttu-id="3ebe9-133">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3ebe9-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3ebe9-134">startDateTime</span></span>|<span data-ttu-id="3ebe9-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ebe9-135">DateTimeOffset</span></span>|<span data-ttu-id="3ebe9-136">Fime в UTC, когда первый пользователь присоединился к сеансу.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-136">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="3ebe9-137">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3ebe9-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3ebe9-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3ebe9-139">endDateTime</span></span>|<span data-ttu-id="3ebe9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ebe9-140">DateTimeOffset</span></span>|<span data-ttu-id="3ebe9-141">Время в UTC, когда последний пользователь покинул сеанс.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="3ebe9-142">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3ebe9-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="3ebe9-144">Связи</span><span class="sxs-lookup"><span data-stu-id="3ebe9-144">Relationships</span></span>

| <span data-ttu-id="3ebe9-145">Связь</span><span class="sxs-lookup"><span data-stu-id="3ebe9-145">Relationship</span></span> | <span data-ttu-id="3ebe9-146">Тип</span><span class="sxs-lookup"><span data-stu-id="3ebe9-146">Type</span></span>        | <span data-ttu-id="3ebe9-147">Описание</span><span class="sxs-lookup"><span data-stu-id="3ebe9-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ebe9-148">segments</span><span class="sxs-lookup"><span data-stu-id="3ebe9-148">segments</span></span>|<span data-ttu-id="3ebe9-149">[Коллекция microsoft.graph.callRecords.segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="3ebe9-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="3ebe9-150">Список сегментов, участвующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-150">The list of segments involved in the session.</span></span> <span data-ttu-id="3ebe9-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-151">Read-only.</span></span> <span data-ttu-id="3ebe9-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ebe9-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ebe9-153">JSON representation</span></span>

<span data-ttu-id="3ebe9-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ebe9-154">The following is a JSON representation of the resource.</span></span>

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

