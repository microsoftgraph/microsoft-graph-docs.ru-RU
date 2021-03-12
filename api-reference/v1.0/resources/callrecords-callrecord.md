---
title: тип ресурса callRecord
description: Тип callRecord
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 23c66be2623d208482ce80ac60a66abf1bacfdc6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722253"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="e0f50-103">тип ресурса callRecord</span><span class="sxs-lookup"><span data-stu-id="e0f50-103">callRecord resource type</span></span>

<span data-ttu-id="e0f50-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="e0f50-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="e0f50-105">Представляет один одноранговой вызов или групповой вызов между несколькими участниками, иногда именуемого как онлайн-собрание.</span><span class="sxs-lookup"><span data-stu-id="e0f50-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="e0f50-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e0f50-106">Methods</span></span>

| <span data-ttu-id="e0f50-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e0f50-107">Method</span></span>       | <span data-ttu-id="e0f50-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e0f50-108">Return Type</span></span> | <span data-ttu-id="e0f50-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e0f50-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e0f50-110">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="e0f50-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="e0f50-111">microsoft.graph.callRecords.callRecord</span><span class="sxs-lookup"><span data-stu-id="e0f50-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="e0f50-112">Чтение свойств и связей объекта callRecord.</span><span class="sxs-lookup"><span data-stu-id="e0f50-112">Read properties and relationships of callRecord object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e0f50-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0f50-113">Properties</span></span>

| <span data-ttu-id="e0f50-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0f50-114">Property</span></span>     | <span data-ttu-id="e0f50-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e0f50-115">Type</span></span>        | <span data-ttu-id="e0f50-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e0f50-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0f50-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e0f50-117">endDateTime</span></span>|<span data-ttu-id="e0f50-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0f50-118">DateTimeOffset</span></span>|<span data-ttu-id="e0f50-119">Время UTC, когда последний пользователь покинул вызов.</span><span class="sxs-lookup"><span data-stu-id="e0f50-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="e0f50-120">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e0f50-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0f50-121">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e0f50-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e0f50-122">id</span><span class="sxs-lookup"><span data-stu-id="e0f50-122">id</span></span>|<span data-ttu-id="e0f50-123">String</span><span class="sxs-lookup"><span data-stu-id="e0f50-123">String</span></span>|<span data-ttu-id="e0f50-124">Уникальный идентификатор для записи вызовов.</span><span class="sxs-lookup"><span data-stu-id="e0f50-124">Unique identifier for the call record.</span></span> <span data-ttu-id="e0f50-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0f50-125">Read-only.</span></span>|
|<span data-ttu-id="e0f50-126">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="e0f50-126">joinWebUrl</span></span>|<span data-ttu-id="e0f50-127">String</span><span class="sxs-lookup"><span data-stu-id="e0f50-127">String</span></span>|<span data-ttu-id="e0f50-128">Собрание URL-адреса, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="e0f50-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="e0f50-129">Может быть недоступным для типа записи вызовов peerToPeer.</span><span class="sxs-lookup"><span data-stu-id="e0f50-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="e0f50-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0f50-130">lastModifiedDateTime</span></span>|<span data-ttu-id="e0f50-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0f50-131">DateTimeOffset</span></span>|<span data-ttu-id="e0f50-132">Время UTC при создания записи вызовов.</span><span class="sxs-lookup"><span data-stu-id="e0f50-132">UTC time when the call record was created.</span></span> <span data-ttu-id="e0f50-133">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="e0f50-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0f50-134">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e0f50-134">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e0f50-135">модальности</span><span class="sxs-lookup"><span data-stu-id="e0f50-135">modalities</span></span>|<span data-ttu-id="e0f50-136">коллекция microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="e0f50-136">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="e0f50-137">Список всех способов, используемых в вызове.</span><span class="sxs-lookup"><span data-stu-id="e0f50-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="e0f50-138">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e0f50-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e0f50-139">organizer</span><span class="sxs-lookup"><span data-stu-id="e0f50-139">organizer</span></span>|[<span data-ttu-id="e0f50-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="e0f50-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="e0f50-141">Удостоверение организатора.</span><span class="sxs-lookup"><span data-stu-id="e0f50-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="e0f50-142">participants</span><span class="sxs-lookup"><span data-stu-id="e0f50-142">participants</span></span>|<span data-ttu-id="e0f50-143">Коллекция [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="e0f50-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="e0f50-144">Список различных удостоверений, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="e0f50-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="e0f50-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e0f50-145">startDateTime</span></span>|<span data-ttu-id="e0f50-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0f50-146">DateTimeOffset</span></span>|<span data-ttu-id="e0f50-147">Время UTC, когда первый пользователь присоединился к вызову.</span><span class="sxs-lookup"><span data-stu-id="e0f50-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="e0f50-148">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="e0f50-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0f50-149">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e0f50-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e0f50-150">type</span><span class="sxs-lookup"><span data-stu-id="e0f50-150">type</span></span>|<span data-ttu-id="e0f50-151">microsoft.graph.callRecords.callType</span><span class="sxs-lookup"><span data-stu-id="e0f50-151">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="e0f50-152">Указывает тип вызова.</span><span class="sxs-lookup"><span data-stu-id="e0f50-152">Indicates the type of the call.</span></span> <span data-ttu-id="e0f50-153">Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e0f50-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e0f50-154">version</span><span class="sxs-lookup"><span data-stu-id="e0f50-154">version</span></span>|<span data-ttu-id="e0f50-155">Int64</span><span class="sxs-lookup"><span data-stu-id="e0f50-155">Int64</span></span>|<span data-ttu-id="e0f50-156">Монотонно увеличивающаяся версия записи вызовов.</span><span class="sxs-lookup"><span data-stu-id="e0f50-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="e0f50-157">Записи вызовов более высокой версии с тем же ид включают дополнительные данные по сравнению с более низкой версией.</span><span class="sxs-lookup"><span data-stu-id="e0f50-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0f50-158">Связи</span><span class="sxs-lookup"><span data-stu-id="e0f50-158">Relationships</span></span>

| <span data-ttu-id="e0f50-159">Связь</span><span class="sxs-lookup"><span data-stu-id="e0f50-159">Relationship</span></span> | <span data-ttu-id="e0f50-160">Тип</span><span class="sxs-lookup"><span data-stu-id="e0f50-160">Type</span></span>        | <span data-ttu-id="e0f50-161">Описание</span><span class="sxs-lookup"><span data-stu-id="e0f50-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0f50-162">сеансы</span><span class="sxs-lookup"><span data-stu-id="e0f50-162">sessions</span></span>|<span data-ttu-id="e0f50-163">[коллекция microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="e0f50-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="e0f50-164">Список сеансов, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="e0f50-164">List of sessions involved in the call.</span></span> <span data-ttu-id="e0f50-165">Одноранговые вызовы обычно имеют только один сеанс, в то время как групповые вызовы обычно имеют по крайней мере один сеанс на каждого участника.</span><span class="sxs-lookup"><span data-stu-id="e0f50-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="e0f50-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0f50-166">Read-only.</span></span> <span data-ttu-id="e0f50-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e0f50-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0f50-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0f50-168">JSON representation</span></span>

<span data-ttu-id="e0f50-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0f50-169">The following is a JSON representation of the resource.</span></span>

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
