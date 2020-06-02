---
title: Тип ресурса Session
description: Тип сеанса
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f661f77ad381c61a3e27ba7edb5372b4f3bcbb5
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492128"
---
# <a name="session-resource-type"></a><span data-ttu-id="33808-103">Тип ресурса Session</span><span class="sxs-lookup"><span data-stu-id="33808-103">session resource type</span></span>

<span data-ttu-id="33808-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="33808-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="33808-105">Представляет пользовательское взаимодействие с пользователем или собрание пользователя в случае вызова конференции.</span><span class="sxs-lookup"><span data-stu-id="33808-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="33808-106">Методы</span><span class="sxs-lookup"><span data-stu-id="33808-106">Methods</span></span>

| <span data-ttu-id="33808-107">Метод</span><span class="sxs-lookup"><span data-stu-id="33808-107">Method</span></span>       | <span data-ttu-id="33808-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="33808-108">Return Type</span></span> | <span data-ttu-id="33808-109">Описание</span><span class="sxs-lookup"><span data-stu-id="33808-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="33808-110">Список сеансов</span><span class="sxs-lookup"><span data-stu-id="33808-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="33808-111">Коллекция [Microsoft. Graph. каллрекордс. Session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="33808-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="33808-112">Получение списка сеансов, связанных с объектом [каллрекорд](callrecords-callrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="33808-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="33808-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="33808-113">Properties</span></span>

| <span data-ttu-id="33808-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="33808-114">Property</span></span>     | <span data-ttu-id="33808-115">Тип</span><span class="sxs-lookup"><span data-stu-id="33808-115">Type</span></span>        | <span data-ttu-id="33808-116">Описание</span><span class="sxs-lookup"><span data-stu-id="33808-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33808-117">id</span><span class="sxs-lookup"><span data-stu-id="33808-117">id</span></span>|<span data-ttu-id="33808-118">string</span><span class="sxs-lookup"><span data-stu-id="33808-118">string</span></span>|<span data-ttu-id="33808-119">Уникальный идентификатор сеанса.</span><span class="sxs-lookup"><span data-stu-id="33808-119">Unique identifier for the session.</span></span> <span data-ttu-id="33808-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33808-120">Read-only.</span></span>|
|<span data-ttu-id="33808-121">объекта</span><span class="sxs-lookup"><span data-stu-id="33808-121">caller</span></span>|[<span data-ttu-id="33808-122">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="33808-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="33808-123">Конечная точка, которая инициировала сеанс.</span><span class="sxs-lookup"><span data-stu-id="33808-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="33808-124">вызываемого абонента</span><span class="sxs-lookup"><span data-stu-id="33808-124">callee</span></span>|[<span data-ttu-id="33808-125">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="33808-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="33808-126">Конечная точка, которая ответила на сеанс.</span><span class="sxs-lookup"><span data-stu-id="33808-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="33808-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="33808-127">failureInfo</span></span>|[<span data-ttu-id="33808-128">Microsoft. Graph. Каллрекордс. Фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="33808-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="33808-129">Сведения о сбое, связанные с сеансом в случае сбоя сеанса.</span><span class="sxs-lookup"><span data-stu-id="33808-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="33808-130">модальности</span><span class="sxs-lookup"><span data-stu-id="33808-130">modalities</span></span>|<span data-ttu-id="33808-131">коллекция Microsoft. Graph. Каллрекордс. Modal</span><span class="sxs-lookup"><span data-stu-id="33808-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="33808-132">Список модальности, присутствующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="33808-132">List of modalities present in the session.</span></span> <span data-ttu-id="33808-133">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="33808-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="33808-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="33808-134">startDateTime</span></span>|<span data-ttu-id="33808-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33808-135">DateTimeOffset</span></span>|<span data-ttu-id="33808-136">UTC Фиме, когда первый пользователь присоединился к сеансу.</span><span class="sxs-lookup"><span data-stu-id="33808-136">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="33808-137">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="33808-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="33808-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="33808-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="33808-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="33808-139">endDateTime</span></span>|<span data-ttu-id="33808-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33808-140">DateTimeOffset</span></span>|<span data-ttu-id="33808-141">Время в формате UTC, когда последний пользователь оставил сеанс.</span><span class="sxs-lookup"><span data-stu-id="33808-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="33808-142">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="33808-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="33808-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="33808-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="33808-144">Связи</span><span class="sxs-lookup"><span data-stu-id="33808-144">Relationships</span></span>

| <span data-ttu-id="33808-145">Связь</span><span class="sxs-lookup"><span data-stu-id="33808-145">Relationship</span></span> | <span data-ttu-id="33808-146">Тип</span><span class="sxs-lookup"><span data-stu-id="33808-146">Type</span></span>        | <span data-ttu-id="33808-147">Описание</span><span class="sxs-lookup"><span data-stu-id="33808-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33808-148">segments</span><span class="sxs-lookup"><span data-stu-id="33808-148">segments</span></span>|<span data-ttu-id="33808-149">Коллекция [Microsoft. Graph. каллрекордс. segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="33808-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="33808-150">Список сегментов, участвующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="33808-150">The list of segments involved in the session.</span></span> <span data-ttu-id="33808-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33808-151">Read-only.</span></span> <span data-ttu-id="33808-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="33808-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33808-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33808-153">JSON representation</span></span>

<span data-ttu-id="33808-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33808-154">The following is a JSON representation of the resource.</span></span>

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