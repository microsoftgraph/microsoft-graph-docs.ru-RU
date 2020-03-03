---
title: Тип ресурса Session
description: Тип сеанса
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d72ddd8273088fb7b1401d93e686914a69d18ebd
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394788"
---
# <a name="session-resource-type"></a><span data-ttu-id="11baa-103">Тип ресурса Session</span><span class="sxs-lookup"><span data-stu-id="11baa-103">session resource type</span></span>

<span data-ttu-id="11baa-104">Пространство имен: Microsoft. Graph. Каллрекордс</span><span class="sxs-lookup"><span data-stu-id="11baa-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11baa-105">Представляет пользовательское взаимодействие с пользователем или собрание пользователя в случае вызова конференции.</span><span class="sxs-lookup"><span data-stu-id="11baa-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="11baa-106">Methods</span><span class="sxs-lookup"><span data-stu-id="11baa-106">Methods</span></span>

<span data-ttu-id="11baa-107">Не существует методов для прямого доступа к сеансам.</span><span class="sxs-lookup"><span data-stu-id="11baa-107">No methods exist to directly access sessions.</span></span> <span data-ttu-id="11baa-108">Используйте API [Get каллрекорд](../api/callrecords-callrecord-get.md) , `$expand=sessions` чтобы получить сеансы для [каллрекорд](callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="11baa-108">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions` to get the sessions for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="11baa-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="11baa-109">Properties</span></span>

| <span data-ttu-id="11baa-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="11baa-110">Property</span></span>     | <span data-ttu-id="11baa-111">Тип</span><span class="sxs-lookup"><span data-stu-id="11baa-111">Type</span></span>        | <span data-ttu-id="11baa-112">Описание</span><span class="sxs-lookup"><span data-stu-id="11baa-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11baa-113">id</span><span class="sxs-lookup"><span data-stu-id="11baa-113">id</span></span>|<span data-ttu-id="11baa-114">string</span><span class="sxs-lookup"><span data-stu-id="11baa-114">string</span></span>|<span data-ttu-id="11baa-115">Уникальный идентификатор сеанса.</span><span class="sxs-lookup"><span data-stu-id="11baa-115">Unique identifier for the session.</span></span> <span data-ttu-id="11baa-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11baa-116">Read-only.</span></span>|
|<span data-ttu-id="11baa-117">объекта</span><span class="sxs-lookup"><span data-stu-id="11baa-117">caller</span></span>|[<span data-ttu-id="11baa-118">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="11baa-118">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="11baa-119">Конечная точка, которая инициировала сеанс.</span><span class="sxs-lookup"><span data-stu-id="11baa-119">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="11baa-120">вызываемого абонента</span><span class="sxs-lookup"><span data-stu-id="11baa-120">callee</span></span>|[<span data-ttu-id="11baa-121">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="11baa-121">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="11baa-122">Конечная точка, которая ответила на сеанс.</span><span class="sxs-lookup"><span data-stu-id="11baa-122">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="11baa-123">фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="11baa-123">failureInfo</span></span>|[<span data-ttu-id="11baa-124">Microsoft. Graph. Каллрекордс. Фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="11baa-124">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="11baa-125">Сведения о сбое, связанные с сеансом в случае сбоя сеанса.</span><span class="sxs-lookup"><span data-stu-id="11baa-125">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="11baa-126">модальности</span><span class="sxs-lookup"><span data-stu-id="11baa-126">modalities</span></span>|<span data-ttu-id="11baa-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="11baa-127">string collection</span></span>|<span data-ttu-id="11baa-128">Список модальности, присутствующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="11baa-128">List of modalities present in the session.</span></span> <span data-ttu-id="11baa-129">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="11baa-129">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="11baa-130">startDateTime</span><span class="sxs-lookup"><span data-stu-id="11baa-130">startDateTime</span></span>|<span data-ttu-id="11baa-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11baa-131">DateTimeOffset</span></span>|<span data-ttu-id="11baa-132">UTC Фиме, когда первый пользователь присоединился к сеансу.</span><span class="sxs-lookup"><span data-stu-id="11baa-132">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="11baa-133">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="11baa-133">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11baa-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11baa-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="11baa-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="11baa-135">endDateTime</span></span>|<span data-ttu-id="11baa-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11baa-136">DateTimeOffset</span></span>|<span data-ttu-id="11baa-137">Время в формате UTC, когда последний пользователь оставил сеанс.</span><span class="sxs-lookup"><span data-stu-id="11baa-137">UTC time when the last user left the session.</span></span> <span data-ttu-id="11baa-138">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="11baa-138">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11baa-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11baa-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="11baa-140">Связи</span><span class="sxs-lookup"><span data-stu-id="11baa-140">Relationships</span></span>

| <span data-ttu-id="11baa-141">Связь</span><span class="sxs-lookup"><span data-stu-id="11baa-141">Relationship</span></span> | <span data-ttu-id="11baa-142">Тип</span><span class="sxs-lookup"><span data-stu-id="11baa-142">Type</span></span>        | <span data-ttu-id="11baa-143">Описание</span><span class="sxs-lookup"><span data-stu-id="11baa-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11baa-144">segments</span><span class="sxs-lookup"><span data-stu-id="11baa-144">segments</span></span>|<span data-ttu-id="11baa-145">Коллекция [Microsoft. Graph. каллрекордс. segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="11baa-145">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="11baa-146">Список сегментов, участвующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="11baa-146">The list of segments involved in the session.</span></span> <span data-ttu-id="11baa-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11baa-147">Read-only.</span></span> <span data-ttu-id="11baa-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="11baa-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11baa-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11baa-149">JSON representation</span></span>

<span data-ttu-id="11baa-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11baa-150">The following is a JSON representation of the resource.</span></span>

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