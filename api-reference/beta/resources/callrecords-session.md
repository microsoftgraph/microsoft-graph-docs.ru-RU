---
title: Тип ресурса Session
description: Тип сеанса
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 91683b4bd9568d14a7049a74d997564b570e4f26
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48600973"
---
# <a name="session-resource-type"></a><span data-ttu-id="6246e-103">Тип ресурса Session</span><span class="sxs-lookup"><span data-stu-id="6246e-103">session resource type</span></span>

<span data-ttu-id="6246e-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="6246e-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6246e-105">Представляет User-User связь или User-Meeting связь в случае вызова конференции.</span><span class="sxs-lookup"><span data-stu-id="6246e-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="6246e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6246e-106">Methods</span></span>

| <span data-ttu-id="6246e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6246e-107">Method</span></span>       | <span data-ttu-id="6246e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6246e-108">Return Type</span></span> | <span data-ttu-id="6246e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6246e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6246e-110">Перечисление сеансов</span><span class="sxs-lookup"><span data-stu-id="6246e-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="6246e-111">Коллекция [Microsoft. Graph. каллрекордс. Session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="6246e-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="6246e-112">Получение списка сеансов, связанных с объектом [каллрекорд](callrecords-callrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="6246e-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="6246e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="6246e-113">Properties</span></span>

| <span data-ttu-id="6246e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="6246e-114">Property</span></span>     | <span data-ttu-id="6246e-115">Тип</span><span class="sxs-lookup"><span data-stu-id="6246e-115">Type</span></span>        | <span data-ttu-id="6246e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="6246e-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6246e-117">id</span><span class="sxs-lookup"><span data-stu-id="6246e-117">id</span></span>|<span data-ttu-id="6246e-118">строка</span><span class="sxs-lookup"><span data-stu-id="6246e-118">string</span></span>|<span data-ttu-id="6246e-119">Уникальный идентификатор сеанса.</span><span class="sxs-lookup"><span data-stu-id="6246e-119">Unique identifier for the session.</span></span> <span data-ttu-id="6246e-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6246e-120">Read-only.</span></span>|
|<span data-ttu-id="6246e-121">объекта</span><span class="sxs-lookup"><span data-stu-id="6246e-121">caller</span></span>|[<span data-ttu-id="6246e-122">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="6246e-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="6246e-123">Конечная точка, которая инициировала сеанс.</span><span class="sxs-lookup"><span data-stu-id="6246e-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="6246e-124">вызываемого абонента</span><span class="sxs-lookup"><span data-stu-id="6246e-124">callee</span></span>|[<span data-ttu-id="6246e-125">Microsoft. Graph. Каллрекордс. Endpoint</span><span class="sxs-lookup"><span data-stu-id="6246e-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="6246e-126">Конечная точка, которая ответила на сеанс.</span><span class="sxs-lookup"><span data-stu-id="6246e-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="6246e-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="6246e-127">failureInfo</span></span>|[<span data-ttu-id="6246e-128">Microsoft. Graph. Каллрекордс. Фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="6246e-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="6246e-129">Сведения о сбое, связанные с сеансом в случае сбоя сеанса.</span><span class="sxs-lookup"><span data-stu-id="6246e-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="6246e-130">модальности</span><span class="sxs-lookup"><span data-stu-id="6246e-130">modalities</span></span>|<span data-ttu-id="6246e-131">коллекция Microsoft. Graph. Каллрекордс. Modal</span><span class="sxs-lookup"><span data-stu-id="6246e-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="6246e-132">Список модальности, присутствующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="6246e-132">List of modalities present in the session.</span></span> <span data-ttu-id="6246e-133">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6246e-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6246e-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6246e-134">startDateTime</span></span>|<span data-ttu-id="6246e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6246e-135">DateTimeOffset</span></span>|<span data-ttu-id="6246e-136">UTC Фиме, когда первый пользователь присоединился к сеансу.</span><span class="sxs-lookup"><span data-stu-id="6246e-136">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="6246e-137">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6246e-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6246e-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6246e-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6246e-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6246e-139">endDateTime</span></span>|<span data-ttu-id="6246e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6246e-140">DateTimeOffset</span></span>|<span data-ttu-id="6246e-141">Время в формате UTC, когда последний пользователь оставил сеанс.</span><span class="sxs-lookup"><span data-stu-id="6246e-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="6246e-142">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6246e-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6246e-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6246e-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="6246e-144">Связи</span><span class="sxs-lookup"><span data-stu-id="6246e-144">Relationships</span></span>

| <span data-ttu-id="6246e-145">Связь</span><span class="sxs-lookup"><span data-stu-id="6246e-145">Relationship</span></span> | <span data-ttu-id="6246e-146">Тип</span><span class="sxs-lookup"><span data-stu-id="6246e-146">Type</span></span>        | <span data-ttu-id="6246e-147">Описание</span><span class="sxs-lookup"><span data-stu-id="6246e-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6246e-148">segments</span><span class="sxs-lookup"><span data-stu-id="6246e-148">segments</span></span>|<span data-ttu-id="6246e-149">Коллекция [Microsoft. Graph. каллрекордс. segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="6246e-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="6246e-150">Список сегментов, участвующих в сеансе.</span><span class="sxs-lookup"><span data-stu-id="6246e-150">The list of segments involved in the session.</span></span> <span data-ttu-id="6246e-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6246e-151">Read-only.</span></span> <span data-ttu-id="6246e-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6246e-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6246e-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6246e-153">JSON representation</span></span>

<span data-ttu-id="6246e-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6246e-154">The following is a JSON representation of the resource.</span></span>

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

