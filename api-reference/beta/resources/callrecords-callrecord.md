---
title: Тип ресурса callRecord
description: Представляет один одноранговой звонок или групповой звонок между несколькими участниками, которые иногда называют собранием по сети.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 04335e2d804a0d1f824cfc70982e3c138812f8ce
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159684"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="6fb71-103">Тип ресурса callRecord</span><span class="sxs-lookup"><span data-stu-id="6fb71-103">callRecord resource type</span></span>

<span data-ttu-id="6fb71-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="6fb71-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb71-105">Представляет один одноранговой звонок или групповой звонок между несколькими участниками, которые иногда называют собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="6fb71-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="6fb71-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6fb71-106">Methods</span></span>

| <span data-ttu-id="6fb71-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6fb71-107">Method</span></span>       | <span data-ttu-id="6fb71-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6fb71-108">Return Type</span></span> | <span data-ttu-id="6fb71-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6fb71-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6fb71-110">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="6fb71-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="6fb71-111">microsoft.graph.callRecords.callRecord</span><span class="sxs-lookup"><span data-stu-id="6fb71-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="6fb71-112">Чтение свойств и связей объекта **callRecord.**</span><span class="sxs-lookup"><span data-stu-id="6fb71-112">Read the properties and relationships of a **callRecord** object.</span></span> |
| [<span data-ttu-id="6fb71-113">Получить вызовы STN</span><span class="sxs-lookup"><span data-stu-id="6fb71-113">Get PSTN calls</span></span>](../api/callrecords-callrecord-getpstncalls.md) | [<span data-ttu-id="6fb71-114">microsoft.graph.callRecords.pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="6fb71-114">microsoft.graph.callRecords.pstnCallLogRow</span></span>](callrecords-pstncalllogrow.md)| <span data-ttu-id="6fb71-115">Чтение свойств объекта **pstnCallLogRow.**</span><span class="sxs-lookup"><span data-stu-id="6fb71-115">Read the properties of a **pstnCallLogRow** object.</span></span> |
| [<span data-ttu-id="6fb71-116">Get direct routing calls</span><span class="sxs-lookup"><span data-stu-id="6fb71-116">Get direct routing calls</span></span>](../api/callrecords-callrecord-getdirectroutingcalls.md) | [<span data-ttu-id="6fb71-117">microsoft.graph.callRecords.directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="6fb71-117">microsoft.graph.callRecords.directRoutingLogRow</span></span>](callrecords-directroutinglogrow.md)| <span data-ttu-id="6fb71-118">Чтение свойств объекта **directRoutingLogRow.**</span><span class="sxs-lookup"><span data-stu-id="6fb71-118">Read the properties of a **directRoutingLogRow** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6fb71-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fb71-119">Properties</span></span>

| <span data-ttu-id="6fb71-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fb71-120">Property</span></span>     | <span data-ttu-id="6fb71-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6fb71-121">Type</span></span>        | <span data-ttu-id="6fb71-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6fb71-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6fb71-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb71-123">endDateTime</span></span>|<span data-ttu-id="6fb71-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb71-124">DateTimeOffset</span></span>|<span data-ttu-id="6fb71-125">Время в UTC, когда последний пользователь оставил вызов.</span><span class="sxs-lookup"><span data-stu-id="6fb71-125">UTC time when the last user left the call.</span></span> <span data-ttu-id="6fb71-126">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6fb71-126">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6fb71-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6fb71-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6fb71-128">id</span><span class="sxs-lookup"><span data-stu-id="6fb71-128">id</span></span>|<span data-ttu-id="6fb71-129">String</span><span class="sxs-lookup"><span data-stu-id="6fb71-129">String</span></span>|<span data-ttu-id="6fb71-130">Уникальный идентификатор записи вызова.</span><span class="sxs-lookup"><span data-stu-id="6fb71-130">Unique identifier for the call record.</span></span> <span data-ttu-id="6fb71-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6fb71-131">Read-only.</span></span>|
|<span data-ttu-id="6fb71-132">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="6fb71-132">joinWebUrl</span></span>|<span data-ttu-id="6fb71-133">String</span><span class="sxs-lookup"><span data-stu-id="6fb71-133">String</span></span>|<span data-ttu-id="6fb71-134">URL-адрес собрания, связанный с вызовом.</span><span class="sxs-lookup"><span data-stu-id="6fb71-134">Meeting URL associated to the call.</span></span> <span data-ttu-id="6fb71-135">Может быть не доступен для типа записи вызова peerToPeer.</span><span class="sxs-lookup"><span data-stu-id="6fb71-135">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="6fb71-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb71-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6fb71-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb71-137">DateTimeOffset</span></span>|<span data-ttu-id="6fb71-138">Время создания записи вызова в UTC.</span><span class="sxs-lookup"><span data-stu-id="6fb71-138">UTC time when the call record was created.</span></span> <span data-ttu-id="6fb71-139">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6fb71-139">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6fb71-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6fb71-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6fb71-141">модальности</span><span class="sxs-lookup"><span data-stu-id="6fb71-141">modalities</span></span>|<span data-ttu-id="6fb71-142">Коллекция microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="6fb71-142">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="6fb71-143">Список всех модальных режимов, используемых в вызове.</span><span class="sxs-lookup"><span data-stu-id="6fb71-143">List of all the modalities used in the call.</span></span> <span data-ttu-id="6fb71-144">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6fb71-144">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6fb71-145">organizer</span><span class="sxs-lookup"><span data-stu-id="6fb71-145">organizer</span></span>|[<span data-ttu-id="6fb71-146">identitySet</span><span class="sxs-lookup"><span data-stu-id="6fb71-146">identitySet</span></span>](identityset.md)|<span data-ttu-id="6fb71-147">Удостоверение организатора.</span><span class="sxs-lookup"><span data-stu-id="6fb71-147">The organizing party's identity.</span></span>|
|<span data-ttu-id="6fb71-148">participants</span><span class="sxs-lookup"><span data-stu-id="6fb71-148">participants</span></span>|<span data-ttu-id="6fb71-149">Коллекция [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="6fb71-149">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="6fb71-150">Список отдельных удостоверений, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="6fb71-150">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="6fb71-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb71-151">startDateTime</span></span>|<span data-ttu-id="6fb71-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb71-152">DateTimeOffset</span></span>|<span data-ttu-id="6fb71-153">Время в UTC, когда первый пользователь присоединился к вызову.</span><span class="sxs-lookup"><span data-stu-id="6fb71-153">UTC time when the first user joined the call.</span></span> <span data-ttu-id="6fb71-154">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6fb71-154">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6fb71-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6fb71-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6fb71-156">type</span><span class="sxs-lookup"><span data-stu-id="6fb71-156">type</span></span>|<span data-ttu-id="6fb71-157">microsoft.graph.callRecords.callType</span><span class="sxs-lookup"><span data-stu-id="6fb71-157">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="6fb71-158">Указывает тип вызова.</span><span class="sxs-lookup"><span data-stu-id="6fb71-158">Indicates the type of the call.</span></span> <span data-ttu-id="6fb71-159">Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6fb71-159">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6fb71-160">version</span><span class="sxs-lookup"><span data-stu-id="6fb71-160">version</span></span>|<span data-ttu-id="6fb71-161">Int64</span><span class="sxs-lookup"><span data-stu-id="6fb71-161">Int64</span></span>|<span data-ttu-id="6fb71-162">Монотонно увеличивающаяся версия записи вызова.</span><span class="sxs-lookup"><span data-stu-id="6fb71-162">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="6fb71-163">Записи вызовов более высокой версии с тем же ИД включают дополнительные данные по сравнению с более низкой версией.</span><span class="sxs-lookup"><span data-stu-id="6fb71-163">Higher version call records with the same ID includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fb71-164">Связи</span><span class="sxs-lookup"><span data-stu-id="6fb71-164">Relationships</span></span>

| <span data-ttu-id="6fb71-165">Связь</span><span class="sxs-lookup"><span data-stu-id="6fb71-165">Relationship</span></span> | <span data-ttu-id="6fb71-166">Тип</span><span class="sxs-lookup"><span data-stu-id="6fb71-166">Type</span></span>        | <span data-ttu-id="6fb71-167">Описание</span><span class="sxs-lookup"><span data-stu-id="6fb71-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6fb71-168">sessions</span><span class="sxs-lookup"><span data-stu-id="6fb71-168">sessions</span></span>|<span data-ttu-id="6fb71-169">[Коллекция microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="6fb71-169">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="6fb71-170">Список сеансов, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="6fb71-170">List of sessions involved in the call.</span></span> <span data-ttu-id="6fb71-171">Одноранговые звонки обычно имеют только один сеанс, тогда как групповые вызовы обычно имеют по крайней мере один сеанс на участника.</span><span class="sxs-lookup"><span data-stu-id="6fb71-171">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="6fb71-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6fb71-172">Read-only.</span></span> <span data-ttu-id="6fb71-173">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6fb71-173">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fb71-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fb71-174">JSON representation</span></span>

<span data-ttu-id="6fb71-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fb71-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
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


