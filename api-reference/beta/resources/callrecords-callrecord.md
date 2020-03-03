---
title: Тип ресурса Каллрекорд
description: Тип Каллрекорд
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0eddc25f92c7043425ff63c46ce5fbba23f5a1be
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394880"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="fee57-103">Тип ресурса Каллрекорд</span><span class="sxs-lookup"><span data-stu-id="fee57-103">callRecord resource type</span></span>

<span data-ttu-id="fee57-104">Пространство имен: Microsoft. Graph. Каллрекордс</span><span class="sxs-lookup"><span data-stu-id="fee57-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fee57-105">Представляет один одноранговый вызов или групповой вызов между несколькими участниками, которые иногда называют собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="fee57-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="fee57-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fee57-106">Methods</span></span>

| <span data-ttu-id="fee57-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fee57-107">Method</span></span>       | <span data-ttu-id="fee57-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fee57-108">Return Type</span></span> | <span data-ttu-id="fee57-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fee57-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fee57-110">Получение Каллрекорд</span><span class="sxs-lookup"><span data-stu-id="fee57-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="fee57-111">Microsoft. Graph. Каллрекордс. Каллрекорд</span><span class="sxs-lookup"><span data-stu-id="fee57-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="fee57-112">Чтение свойств и связей объекта Каллрекорд.</span><span class="sxs-lookup"><span data-stu-id="fee57-112">Read properties and relationships of callRecord object.</span></span> |
## <a name="properties"></a><span data-ttu-id="fee57-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="fee57-113">Properties</span></span>

| <span data-ttu-id="fee57-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="fee57-114">Property</span></span>     | <span data-ttu-id="fee57-115">Тип</span><span class="sxs-lookup"><span data-stu-id="fee57-115">Type</span></span>        | <span data-ttu-id="fee57-116">Описание</span><span class="sxs-lookup"><span data-stu-id="fee57-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fee57-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fee57-117">endDateTime</span></span>|<span data-ttu-id="fee57-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fee57-118">DateTimeOffset</span></span>|<span data-ttu-id="fee57-119">Время в формате UTC, когда последний пользователь оставил вызов.</span><span class="sxs-lookup"><span data-stu-id="fee57-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="fee57-120">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fee57-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fee57-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fee57-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fee57-122">id</span><span class="sxs-lookup"><span data-stu-id="fee57-122">id</span></span>|<span data-ttu-id="fee57-123">Строка</span><span class="sxs-lookup"><span data-stu-id="fee57-123">String</span></span>|<span data-ttu-id="fee57-124">Уникальный идентификатор для записи вызова.</span><span class="sxs-lookup"><span data-stu-id="fee57-124">Unique identifier for the call record.</span></span> <span data-ttu-id="fee57-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fee57-125">Read-only.</span></span>|
|<span data-ttu-id="fee57-126">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="fee57-126">joinWebUrl</span></span>|<span data-ttu-id="fee57-127">String</span><span class="sxs-lookup"><span data-stu-id="fee57-127">String</span></span>|<span data-ttu-id="fee57-128">URL-адрес собрания, связанный с вызовом.</span><span class="sxs-lookup"><span data-stu-id="fee57-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="fee57-129">Может быть недоступен для типа записи вызовов Пиртопир.</span><span class="sxs-lookup"><span data-stu-id="fee57-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="fee57-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fee57-130">lastModifiedDateTime</span></span>|<span data-ttu-id="fee57-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fee57-131">DateTimeOffset</span></span>|<span data-ttu-id="fee57-132">Время в формате UTC при создании записи вызова.</span><span class="sxs-lookup"><span data-stu-id="fee57-132">UTC time when the call record was created.</span></span> <span data-ttu-id="fee57-133">Тип DatetimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается как время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fee57-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fee57-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fee57-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fee57-135">модальности</span><span class="sxs-lookup"><span data-stu-id="fee57-135">modalities</span></span>|<span data-ttu-id="fee57-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fee57-136">string collection</span></span>|<span data-ttu-id="fee57-137">Список всех модальности, используемых в вызове.</span><span class="sxs-lookup"><span data-stu-id="fee57-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="fee57-138">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fee57-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fee57-139">organizer</span><span class="sxs-lookup"><span data-stu-id="fee57-139">organizer</span></span>|[<span data-ttu-id="fee57-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="fee57-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="fee57-141">Удостоверение субъекта Организации.</span><span class="sxs-lookup"><span data-stu-id="fee57-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="fee57-142">participants</span><span class="sxs-lookup"><span data-stu-id="fee57-142">participants</span></span>|<span data-ttu-id="fee57-143">Коллекция [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="fee57-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="fee57-144">Список уникальных удостоверений, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="fee57-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="fee57-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fee57-145">startDateTime</span></span>|<span data-ttu-id="fee57-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fee57-146">DateTimeOffset</span></span>|<span data-ttu-id="fee57-147">Время в формате UTC, когда первый пользователь присоединился к вызову.</span><span class="sxs-lookup"><span data-stu-id="fee57-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="fee57-148">Тип DatetimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается как время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fee57-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fee57-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fee57-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fee57-150">type</span><span class="sxs-lookup"><span data-stu-id="fee57-150">type</span></span>|<span data-ttu-id="fee57-151">string</span><span class="sxs-lookup"><span data-stu-id="fee57-151">string</span></span>|<span data-ttu-id="fee57-152">Указывает тип вызова.</span><span class="sxs-lookup"><span data-stu-id="fee57-152">Indicates the type of the call.</span></span> <span data-ttu-id="fee57-153">Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fee57-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fee57-154">version</span><span class="sxs-lookup"><span data-stu-id="fee57-154">version</span></span>|<span data-ttu-id="fee57-155">Int64</span><span class="sxs-lookup"><span data-stu-id="fee57-155">Int64</span></span>|<span data-ttu-id="fee57-156">Монотонно увеличивающаяся версия записи вызова.</span><span class="sxs-lookup"><span data-stu-id="fee57-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="fee57-157">Более высокие записи вызовов с одинаковым идентификатором содержат дополнительные данные по сравнению с более низкой версией.</span><span class="sxs-lookup"><span data-stu-id="fee57-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fee57-158">Связи</span><span class="sxs-lookup"><span data-stu-id="fee57-158">Relationships</span></span>

| <span data-ttu-id="fee57-159">Связь</span><span class="sxs-lookup"><span data-stu-id="fee57-159">Relationship</span></span> | <span data-ttu-id="fee57-160">Тип</span><span class="sxs-lookup"><span data-stu-id="fee57-160">Type</span></span>        | <span data-ttu-id="fee57-161">Описание</span><span class="sxs-lookup"><span data-stu-id="fee57-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fee57-162">сеансов</span><span class="sxs-lookup"><span data-stu-id="fee57-162">sessions</span></span>|<span data-ttu-id="fee57-163">Коллекция [Microsoft. Graph. каллрекордс. Session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="fee57-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="fee57-164">Список сеансов, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="fee57-164">List of sessions involved in the call.</span></span> <span data-ttu-id="fee57-165">Одноранговые вызовы обычно имеют только один сеанс, в то время как для групповых вызовов обычно используется по крайней мере один сеанс на каждый участник.</span><span class="sxs-lookup"><span data-stu-id="fee57-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="fee57-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fee57-166">Read-only.</span></span> <span data-ttu-id="fee57-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fee57-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fee57-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fee57-168">JSON representation</span></span>

<span data-ttu-id="fee57-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fee57-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "modalities": ["string"],
  "organizer": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}],
  "startDateTime": "String (timestamp)",
  "type": "string",
  "version": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->