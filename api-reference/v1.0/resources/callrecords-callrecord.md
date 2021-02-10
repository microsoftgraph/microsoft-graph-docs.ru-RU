---
title: Тип ресурса callRecord
description: Тип callRecord
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc1f6498abe52386ccf8aaa67a542adb891b60bb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159411"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="1f50e-103">Тип ресурса callRecord</span><span class="sxs-lookup"><span data-stu-id="1f50e-103">callRecord resource type</span></span>

<span data-ttu-id="1f50e-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="1f50e-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="1f50e-105">Представляет один одноранговой звонок или групповой звонок между несколькими участниками, которые иногда называют собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="1f50e-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="1f50e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1f50e-106">Methods</span></span>

| <span data-ttu-id="1f50e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1f50e-107">Method</span></span>       | <span data-ttu-id="1f50e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f50e-108">Return Type</span></span> | <span data-ttu-id="1f50e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1f50e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1f50e-110">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="1f50e-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="1f50e-111">microsoft.graph.callRecords.callRecord</span><span class="sxs-lookup"><span data-stu-id="1f50e-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="1f50e-112">Чтение свойств и связей объекта callRecord.</span><span class="sxs-lookup"><span data-stu-id="1f50e-112">Read properties and relationships of callRecord object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1f50e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f50e-113">Properties</span></span>

| <span data-ttu-id="1f50e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f50e-114">Property</span></span>     | <span data-ttu-id="1f50e-115">Тип</span><span class="sxs-lookup"><span data-stu-id="1f50e-115">Type</span></span>        | <span data-ttu-id="1f50e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="1f50e-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f50e-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1f50e-117">endDateTime</span></span>|<span data-ttu-id="1f50e-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f50e-118">DateTimeOffset</span></span>|<span data-ttu-id="1f50e-119">Время в UTC, когда последний пользователь оставил вызов.</span><span class="sxs-lookup"><span data-stu-id="1f50e-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="1f50e-120">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1f50e-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f50e-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1f50e-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1f50e-122">id</span><span class="sxs-lookup"><span data-stu-id="1f50e-122">id</span></span>|<span data-ttu-id="1f50e-123">String</span><span class="sxs-lookup"><span data-stu-id="1f50e-123">String</span></span>|<span data-ttu-id="1f50e-124">Уникальный идентификатор записи вызова.</span><span class="sxs-lookup"><span data-stu-id="1f50e-124">Unique identifier for the call record.</span></span> <span data-ttu-id="1f50e-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f50e-125">Read-only.</span></span>|
|<span data-ttu-id="1f50e-126">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="1f50e-126">joinWebUrl</span></span>|<span data-ttu-id="1f50e-127">String</span><span class="sxs-lookup"><span data-stu-id="1f50e-127">String</span></span>|<span data-ttu-id="1f50e-128">URL-адрес собрания, связанный с вызовом.</span><span class="sxs-lookup"><span data-stu-id="1f50e-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="1f50e-129">Может быть не доступен для типа записи вызова peerToPeer.</span><span class="sxs-lookup"><span data-stu-id="1f50e-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="1f50e-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f50e-130">lastModifiedDateTime</span></span>|<span data-ttu-id="1f50e-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f50e-131">DateTimeOffset</span></span>|<span data-ttu-id="1f50e-132">Время создания записи вызова в UTC.</span><span class="sxs-lookup"><span data-stu-id="1f50e-132">UTC time when the call record was created.</span></span> <span data-ttu-id="1f50e-133">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1f50e-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f50e-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1f50e-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1f50e-135">модальности</span><span class="sxs-lookup"><span data-stu-id="1f50e-135">modalities</span></span>|<span data-ttu-id="1f50e-136">Коллекция microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="1f50e-136">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="1f50e-137">Список всех модальных режимов, используемых в вызове.</span><span class="sxs-lookup"><span data-stu-id="1f50e-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="1f50e-138">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1f50e-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1f50e-139">organizer</span><span class="sxs-lookup"><span data-stu-id="1f50e-139">organizer</span></span>|[<span data-ttu-id="1f50e-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="1f50e-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="1f50e-141">Удостоверение организатора.</span><span class="sxs-lookup"><span data-stu-id="1f50e-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="1f50e-142">participants</span><span class="sxs-lookup"><span data-stu-id="1f50e-142">participants</span></span>|<span data-ttu-id="1f50e-143">Коллекция [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="1f50e-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="1f50e-144">Список отдельных удостоверений, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="1f50e-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="1f50e-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1f50e-145">startDateTime</span></span>|<span data-ttu-id="1f50e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f50e-146">DateTimeOffset</span></span>|<span data-ttu-id="1f50e-147">Время в UTC, когда первый пользователь присоединился к вызову.</span><span class="sxs-lookup"><span data-stu-id="1f50e-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="1f50e-148">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1f50e-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f50e-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1f50e-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1f50e-150">type</span><span class="sxs-lookup"><span data-stu-id="1f50e-150">type</span></span>|<span data-ttu-id="1f50e-151">microsoft.graph.callRecords.callType</span><span class="sxs-lookup"><span data-stu-id="1f50e-151">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="1f50e-152">Указывает тип вызова.</span><span class="sxs-lookup"><span data-stu-id="1f50e-152">Indicates the type of the call.</span></span> <span data-ttu-id="1f50e-153">Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1f50e-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1f50e-154">version</span><span class="sxs-lookup"><span data-stu-id="1f50e-154">version</span></span>|<span data-ttu-id="1f50e-155">Int64</span><span class="sxs-lookup"><span data-stu-id="1f50e-155">Int64</span></span>|<span data-ttu-id="1f50e-156">Монотонно увеличивающаяся версия записи вызова.</span><span class="sxs-lookup"><span data-stu-id="1f50e-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="1f50e-157">Записи вызовов более высокой версии с таким же идом включают дополнительные данные по сравнению с более низкой версией.</span><span class="sxs-lookup"><span data-stu-id="1f50e-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f50e-158">Связи</span><span class="sxs-lookup"><span data-stu-id="1f50e-158">Relationships</span></span>

| <span data-ttu-id="1f50e-159">Связь</span><span class="sxs-lookup"><span data-stu-id="1f50e-159">Relationship</span></span> | <span data-ttu-id="1f50e-160">Тип</span><span class="sxs-lookup"><span data-stu-id="1f50e-160">Type</span></span>        | <span data-ttu-id="1f50e-161">Описание</span><span class="sxs-lookup"><span data-stu-id="1f50e-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f50e-162">sessions</span><span class="sxs-lookup"><span data-stu-id="1f50e-162">sessions</span></span>|<span data-ttu-id="1f50e-163">[коллекция microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="1f50e-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="1f50e-164">Список сеансов, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="1f50e-164">List of sessions involved in the call.</span></span> <span data-ttu-id="1f50e-165">Одноранговые вызовы обычно имеют только один сеанс, тогда как групповые вызовы обычно имеют по крайней мере один сеанс на участника.</span><span class="sxs-lookup"><span data-stu-id="1f50e-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="1f50e-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f50e-166">Read-only.</span></span> <span data-ttu-id="1f50e-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1f50e-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f50e-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f50e-168">JSON representation</span></span>

<span data-ttu-id="1f50e-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f50e-169">The following is a JSON representation of the resource.</span></span>

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
