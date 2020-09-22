---
title: Тип ресурса Каллрекорд
description: Представляет один одноранговый вызов или групповой вызов между несколькими участниками, которые иногда называют собранием по сети.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a119b95daf651ca5a91c269210a81a9a9a3cc1f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071585"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="bcdff-103">Тип ресурса Каллрекорд</span><span class="sxs-lookup"><span data-stu-id="bcdff-103">callRecord resource type</span></span>

<span data-ttu-id="bcdff-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="bcdff-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcdff-105">Представляет один одноранговый вызов или групповой вызов между несколькими участниками, которые иногда называют собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="bcdff-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="bcdff-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bcdff-106">Methods</span></span>

| <span data-ttu-id="bcdff-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bcdff-107">Method</span></span>       | <span data-ttu-id="bcdff-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bcdff-108">Return Type</span></span> | <span data-ttu-id="bcdff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bcdff-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bcdff-110">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="bcdff-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="bcdff-111">Microsoft. Graph. Каллрекордс. Каллрекорд</span><span class="sxs-lookup"><span data-stu-id="bcdff-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="bcdff-112">Чтение свойств и связей объекта **каллрекорд** .</span><span class="sxs-lookup"><span data-stu-id="bcdff-112">Read the properties and relationships of a **callRecord** object.</span></span> |
| [<span data-ttu-id="bcdff-113">Получение звонков PSTN</span><span class="sxs-lookup"><span data-stu-id="bcdff-113">Get PSTN calls</span></span>](../api/callrecords-callrecord-getpstncalls.md) | [<span data-ttu-id="bcdff-114">Microsoft. Graph. Каллрекордс. Пстнкалллогров</span><span class="sxs-lookup"><span data-stu-id="bcdff-114">microsoft.graph.callRecords.pstnCallLogRow</span></span>](callrecords-pstncalllogrow.md)| <span data-ttu-id="bcdff-115">Чтение свойств объекта **пстнкалллогров** .</span><span class="sxs-lookup"><span data-stu-id="bcdff-115">Read the properties of a **pstnCallLogRow** object.</span></span> |
| [<span data-ttu-id="bcdff-116">Получение прямых вызовов маршрутизации</span><span class="sxs-lookup"><span data-stu-id="bcdff-116">Get direct routing calls</span></span>](../api/callrecords-callrecord-getdirectroutingcalls.md) | [<span data-ttu-id="bcdff-117">Microsoft. Graph. Каллрекордс. Директраутинглогров</span><span class="sxs-lookup"><span data-stu-id="bcdff-117">microsoft.graph.callRecords.directRoutingLogRow</span></span>](callrecords-directroutinglogrow.md)| <span data-ttu-id="bcdff-118">Чтение свойств объекта **директраутинглогров** .</span><span class="sxs-lookup"><span data-stu-id="bcdff-118">Read the properties of a **directRoutingLogRow** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bcdff-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="bcdff-119">Properties</span></span>

| <span data-ttu-id="bcdff-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcdff-120">Property</span></span>     | <span data-ttu-id="bcdff-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bcdff-121">Type</span></span>        | <span data-ttu-id="bcdff-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bcdff-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bcdff-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bcdff-123">endDateTime</span></span>|<span data-ttu-id="bcdff-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcdff-124">DateTimeOffset</span></span>|<span data-ttu-id="bcdff-125">Время в формате UTC, когда последний пользователь оставил вызов.</span><span class="sxs-lookup"><span data-stu-id="bcdff-125">UTC time when the last user left the call.</span></span> <span data-ttu-id="bcdff-126">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bcdff-126">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bcdff-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bcdff-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bcdff-128">id</span><span class="sxs-lookup"><span data-stu-id="bcdff-128">id</span></span>|<span data-ttu-id="bcdff-129">String</span><span class="sxs-lookup"><span data-stu-id="bcdff-129">String</span></span>|<span data-ttu-id="bcdff-130">Уникальный идентификатор для записи вызова.</span><span class="sxs-lookup"><span data-stu-id="bcdff-130">Unique identifier for the call record.</span></span> <span data-ttu-id="bcdff-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bcdff-131">Read-only.</span></span>|
|<span data-ttu-id="bcdff-132">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="bcdff-132">joinWebUrl</span></span>|<span data-ttu-id="bcdff-133">String</span><span class="sxs-lookup"><span data-stu-id="bcdff-133">String</span></span>|<span data-ttu-id="bcdff-134">URL-адрес собрания, связанный с вызовом.</span><span class="sxs-lookup"><span data-stu-id="bcdff-134">Meeting URL associated to the call.</span></span> <span data-ttu-id="bcdff-135">Может быть недоступен для типа записи вызовов Пиртопир.</span><span class="sxs-lookup"><span data-stu-id="bcdff-135">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="bcdff-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcdff-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bcdff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcdff-137">DateTimeOffset</span></span>|<span data-ttu-id="bcdff-138">Время в формате UTC при создании записи вызова.</span><span class="sxs-lookup"><span data-stu-id="bcdff-138">UTC time when the call record was created.</span></span> <span data-ttu-id="bcdff-139">Тип DatetimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается как время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bcdff-139">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bcdff-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bcdff-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bcdff-141">модальности</span><span class="sxs-lookup"><span data-stu-id="bcdff-141">modalities</span></span>|<span data-ttu-id="bcdff-142">коллекция Microsoft. Graph. Каллрекордс. Modal</span><span class="sxs-lookup"><span data-stu-id="bcdff-142">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="bcdff-143">Список всех модальности, используемых в вызове.</span><span class="sxs-lookup"><span data-stu-id="bcdff-143">List of all the modalities used in the call.</span></span> <span data-ttu-id="bcdff-144">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bcdff-144">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bcdff-145">organizer</span><span class="sxs-lookup"><span data-stu-id="bcdff-145">organizer</span></span>|[<span data-ttu-id="bcdff-146">identitySet</span><span class="sxs-lookup"><span data-stu-id="bcdff-146">identitySet</span></span>](identityset.md)|<span data-ttu-id="bcdff-147">Удостоверение субъекта Организации.</span><span class="sxs-lookup"><span data-stu-id="bcdff-147">The organizing party's identity.</span></span>|
|<span data-ttu-id="bcdff-148">participants</span><span class="sxs-lookup"><span data-stu-id="bcdff-148">participants</span></span>|<span data-ttu-id="bcdff-149">Коллекция [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="bcdff-149">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="bcdff-150">Список уникальных удостоверений, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="bcdff-150">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="bcdff-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bcdff-151">startDateTime</span></span>|<span data-ttu-id="bcdff-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcdff-152">DateTimeOffset</span></span>|<span data-ttu-id="bcdff-153">Время в формате UTC, когда первый пользователь присоединился к вызову.</span><span class="sxs-lookup"><span data-stu-id="bcdff-153">UTC time when the first user joined the call.</span></span> <span data-ttu-id="bcdff-154">Тип DatetimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается как время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bcdff-154">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bcdff-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bcdff-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bcdff-156">type</span><span class="sxs-lookup"><span data-stu-id="bcdff-156">type</span></span>|<span data-ttu-id="bcdff-157">Microsoft. Graph. Каллрекордс. callType</span><span class="sxs-lookup"><span data-stu-id="bcdff-157">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="bcdff-158">Указывает тип вызова.</span><span class="sxs-lookup"><span data-stu-id="bcdff-158">Indicates the type of the call.</span></span> <span data-ttu-id="bcdff-159">Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bcdff-159">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bcdff-160">version</span><span class="sxs-lookup"><span data-stu-id="bcdff-160">version</span></span>|<span data-ttu-id="bcdff-161">Int64</span><span class="sxs-lookup"><span data-stu-id="bcdff-161">Int64</span></span>|<span data-ttu-id="bcdff-162">Монотонно увеличивающаяся версия записи вызова.</span><span class="sxs-lookup"><span data-stu-id="bcdff-162">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="bcdff-163">Более высокие записи вызовов с одинаковым ИДЕНТИФИКАТОРом содержат дополнительные данные по сравнению с более низкой версией.</span><span class="sxs-lookup"><span data-stu-id="bcdff-163">Higher version call records with the same ID includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcdff-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="bcdff-164">Relationships</span></span>

| <span data-ttu-id="bcdff-165">Связь</span><span class="sxs-lookup"><span data-stu-id="bcdff-165">Relationship</span></span> | <span data-ttu-id="bcdff-166">Тип</span><span class="sxs-lookup"><span data-stu-id="bcdff-166">Type</span></span>        | <span data-ttu-id="bcdff-167">Описание</span><span class="sxs-lookup"><span data-stu-id="bcdff-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bcdff-168">сеансов</span><span class="sxs-lookup"><span data-stu-id="bcdff-168">sessions</span></span>|<span data-ttu-id="bcdff-169">Коллекция [Microsoft. Graph. каллрекордс. Session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="bcdff-169">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="bcdff-170">Список сеансов, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="bcdff-170">List of sessions involved in the call.</span></span> <span data-ttu-id="bcdff-171">Одноранговые вызовы обычно имеют только один сеанс, в то время как для групповых вызовов обычно используется по крайней мере один сеанс на каждый участник.</span><span class="sxs-lookup"><span data-stu-id="bcdff-171">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="bcdff-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bcdff-172">Read-only.</span></span> <span data-ttu-id="bcdff-173">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bcdff-173">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcdff-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bcdff-174">JSON representation</span></span>

<span data-ttu-id="bcdff-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcdff-175">The following is a JSON representation of the resource.</span></span>

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


