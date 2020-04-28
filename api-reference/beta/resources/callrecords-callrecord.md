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
# <a name="callrecord-resource-type"></a><span data-ttu-id="4beda-103">Тип ресурса Каллрекорд</span><span class="sxs-lookup"><span data-stu-id="4beda-103">callRecord resource type</span></span>

<span data-ttu-id="4beda-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="4beda-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4beda-105">Представляет один одноранговый вызов или групповой вызов между несколькими участниками, которые иногда называют собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="4beda-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="4beda-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4beda-106">Methods</span></span>

| <span data-ttu-id="4beda-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4beda-107">Method</span></span>       | <span data-ttu-id="4beda-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4beda-108">Return Type</span></span> | <span data-ttu-id="4beda-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4beda-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4beda-110">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="4beda-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="4beda-111">Microsoft. Graph. Каллрекордс. Каллрекорд</span><span class="sxs-lookup"><span data-stu-id="4beda-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="4beda-112">Чтение свойств и связей объекта Каллрекорд.</span><span class="sxs-lookup"><span data-stu-id="4beda-112">Read properties and relationships of callRecord object.</span></span> |
## <a name="properties"></a><span data-ttu-id="4beda-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="4beda-113">Properties</span></span>

| <span data-ttu-id="4beda-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="4beda-114">Property</span></span>     | <span data-ttu-id="4beda-115">Тип</span><span class="sxs-lookup"><span data-stu-id="4beda-115">Type</span></span>        | <span data-ttu-id="4beda-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4beda-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4beda-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4beda-117">endDateTime</span></span>|<span data-ttu-id="4beda-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4beda-118">DateTimeOffset</span></span>|<span data-ttu-id="4beda-119">Время в формате UTC, когда последний пользователь оставил вызов.</span><span class="sxs-lookup"><span data-stu-id="4beda-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="4beda-120">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4beda-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4beda-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4beda-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4beda-122">id</span><span class="sxs-lookup"><span data-stu-id="4beda-122">id</span></span>|<span data-ttu-id="4beda-123">Строка</span><span class="sxs-lookup"><span data-stu-id="4beda-123">String</span></span>|<span data-ttu-id="4beda-124">Уникальный идентификатор для записи вызова.</span><span class="sxs-lookup"><span data-stu-id="4beda-124">Unique identifier for the call record.</span></span> <span data-ttu-id="4beda-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4beda-125">Read-only.</span></span>|
|<span data-ttu-id="4beda-126">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="4beda-126">joinWebUrl</span></span>|<span data-ttu-id="4beda-127">String</span><span class="sxs-lookup"><span data-stu-id="4beda-127">String</span></span>|<span data-ttu-id="4beda-128">URL-адрес собрания, связанный с вызовом.</span><span class="sxs-lookup"><span data-stu-id="4beda-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="4beda-129">Может быть недоступен для типа записи вызовов Пиртопир.</span><span class="sxs-lookup"><span data-stu-id="4beda-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="4beda-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4beda-130">lastModifiedDateTime</span></span>|<span data-ttu-id="4beda-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4beda-131">DateTimeOffset</span></span>|<span data-ttu-id="4beda-132">Время в формате UTC при создании записи вызова.</span><span class="sxs-lookup"><span data-stu-id="4beda-132">UTC time when the call record was created.</span></span> <span data-ttu-id="4beda-133">Тип DatetimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается как время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4beda-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4beda-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4beda-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4beda-135">модальности</span><span class="sxs-lookup"><span data-stu-id="4beda-135">modalities</span></span>|<span data-ttu-id="4beda-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4beda-136">string collection</span></span>|<span data-ttu-id="4beda-137">Список всех модальности, используемых в вызове.</span><span class="sxs-lookup"><span data-stu-id="4beda-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="4beda-138">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4beda-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4beda-139">organizer</span><span class="sxs-lookup"><span data-stu-id="4beda-139">organizer</span></span>|[<span data-ttu-id="4beda-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="4beda-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="4beda-141">Удостоверение субъекта Организации.</span><span class="sxs-lookup"><span data-stu-id="4beda-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="4beda-142">participants</span><span class="sxs-lookup"><span data-stu-id="4beda-142">participants</span></span>|<span data-ttu-id="4beda-143">Коллекция [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="4beda-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="4beda-144">Список уникальных удостоверений, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="4beda-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="4beda-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4beda-145">startDateTime</span></span>|<span data-ttu-id="4beda-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4beda-146">DateTimeOffset</span></span>|<span data-ttu-id="4beda-147">Время в формате UTC, когда первый пользователь присоединился к вызову.</span><span class="sxs-lookup"><span data-stu-id="4beda-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="4beda-148">Тип DatetimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается как время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4beda-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4beda-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4beda-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4beda-150">type</span><span class="sxs-lookup"><span data-stu-id="4beda-150">type</span></span>|<span data-ttu-id="4beda-151">string</span><span class="sxs-lookup"><span data-stu-id="4beda-151">string</span></span>|<span data-ttu-id="4beda-152">Указывает тип вызова.</span><span class="sxs-lookup"><span data-stu-id="4beda-152">Indicates the type of the call.</span></span> <span data-ttu-id="4beda-153">Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4beda-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4beda-154">version</span><span class="sxs-lookup"><span data-stu-id="4beda-154">version</span></span>|<span data-ttu-id="4beda-155">Int64</span><span class="sxs-lookup"><span data-stu-id="4beda-155">Int64</span></span>|<span data-ttu-id="4beda-156">Монотонно увеличивающаяся версия записи вызова.</span><span class="sxs-lookup"><span data-stu-id="4beda-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="4beda-157">Более высокие записи вызовов с одинаковым идентификатором содержат дополнительные данные по сравнению с более низкой версией.</span><span class="sxs-lookup"><span data-stu-id="4beda-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4beda-158">Связи</span><span class="sxs-lookup"><span data-stu-id="4beda-158">Relationships</span></span>

| <span data-ttu-id="4beda-159">Связь</span><span class="sxs-lookup"><span data-stu-id="4beda-159">Relationship</span></span> | <span data-ttu-id="4beda-160">Тип</span><span class="sxs-lookup"><span data-stu-id="4beda-160">Type</span></span>        | <span data-ttu-id="4beda-161">Описание</span><span class="sxs-lookup"><span data-stu-id="4beda-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4beda-162">сеансов</span><span class="sxs-lookup"><span data-stu-id="4beda-162">sessions</span></span>|<span data-ttu-id="4beda-163">Коллекция [Microsoft. Graph. каллрекордс. Session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="4beda-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="4beda-164">Список сеансов, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="4beda-164">List of sessions involved in the call.</span></span> <span data-ttu-id="4beda-165">Одноранговые вызовы обычно имеют только один сеанс, в то время как для групповых вызовов обычно используется по крайней мере один сеанс на каждый участник.</span><span class="sxs-lookup"><span data-stu-id="4beda-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="4beda-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4beda-166">Read-only.</span></span> <span data-ttu-id="4beda-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4beda-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4beda-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4beda-168">JSON representation</span></span>

<span data-ttu-id="4beda-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4beda-169">The following is a JSON representation of the resource.</span></span>

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