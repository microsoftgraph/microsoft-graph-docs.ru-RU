---
title: тип ресурса callRecord
description: Представляет один одноранговой вызов или групповой вызов между несколькими участниками, иногда именуемого как онлайн-собрание.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b981502fb1714a8a29436fcf8ab2b68150d8fcbd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955024"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="442ae-103">тип ресурса callRecord</span><span class="sxs-lookup"><span data-stu-id="442ae-103">callRecord resource type</span></span>

<span data-ttu-id="442ae-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="442ae-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="442ae-105">Представляет один одноранговой вызов или групповой вызов между несколькими участниками, иногда именуемого как онлайн-собрание.</span><span class="sxs-lookup"><span data-stu-id="442ae-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="442ae-106">Методы</span><span class="sxs-lookup"><span data-stu-id="442ae-106">Methods</span></span>

| <span data-ttu-id="442ae-107">Метод</span><span class="sxs-lookup"><span data-stu-id="442ae-107">Method</span></span>       | <span data-ttu-id="442ae-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="442ae-108">Return Type</span></span> | <span data-ttu-id="442ae-109">Описание</span><span class="sxs-lookup"><span data-stu-id="442ae-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="442ae-110">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="442ae-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="442ae-111">microsoft.graph.callRecords.callRecord</span><span class="sxs-lookup"><span data-stu-id="442ae-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="442ae-112">Ознакомьтесь с свойствами и отношениями объекта **callRecord.**</span><span class="sxs-lookup"><span data-stu-id="442ae-112">Read the properties and relationships of a **callRecord** object.</span></span> |
| [<span data-ttu-id="442ae-113">Получить вызовы PSTN</span><span class="sxs-lookup"><span data-stu-id="442ae-113">Get PSTN calls</span></span>](../api/callrecords-callrecord-getpstncalls.md) | [<span data-ttu-id="442ae-114">microsoft.graph.callRecords.pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="442ae-114">microsoft.graph.callRecords.pstnCallLogRow</span></span>](callrecords-pstncalllogrow.md)| <span data-ttu-id="442ae-115">Ознакомьтесь с свойствами объекта **pstnCallLogRow.**</span><span class="sxs-lookup"><span data-stu-id="442ae-115">Read the properties of a **pstnCallLogRow** object.</span></span> |
| [<span data-ttu-id="442ae-116">Получать прямые вызовы маршрутов</span><span class="sxs-lookup"><span data-stu-id="442ae-116">Get direct routing calls</span></span>](../api/callrecords-callrecord-getdirectroutingcalls.md) | [<span data-ttu-id="442ae-117">microsoft.graph.callRecords.directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="442ae-117">microsoft.graph.callRecords.directRoutingLogRow</span></span>](callrecords-directroutinglogrow.md)| <span data-ttu-id="442ae-118">Ознакомьтесь с свойствами **объекта directRoutingLogRow.**</span><span class="sxs-lookup"><span data-stu-id="442ae-118">Read the properties of a **directRoutingLogRow** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="442ae-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="442ae-119">Properties</span></span>

| <span data-ttu-id="442ae-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="442ae-120">Property</span></span>     | <span data-ttu-id="442ae-121">Тип</span><span class="sxs-lookup"><span data-stu-id="442ae-121">Type</span></span>        | <span data-ttu-id="442ae-122">Описание</span><span class="sxs-lookup"><span data-stu-id="442ae-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="442ae-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="442ae-123">endDateTime</span></span>|<span data-ttu-id="442ae-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="442ae-124">DateTimeOffset</span></span>|<span data-ttu-id="442ae-125">Время UTC, когда последний пользователь покинул вызов.</span><span class="sxs-lookup"><span data-stu-id="442ae-125">UTC time when the last user left the call.</span></span> <span data-ttu-id="442ae-126">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="442ae-126">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="442ae-127">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="442ae-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="442ae-128">id</span><span class="sxs-lookup"><span data-stu-id="442ae-128">id</span></span>|<span data-ttu-id="442ae-129">Строка</span><span class="sxs-lookup"><span data-stu-id="442ae-129">String</span></span>|<span data-ttu-id="442ae-130">Уникальный идентификатор для записи вызовов.</span><span class="sxs-lookup"><span data-stu-id="442ae-130">Unique identifier for the call record.</span></span> <span data-ttu-id="442ae-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="442ae-131">Read-only.</span></span>|
|<span data-ttu-id="442ae-132">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="442ae-132">joinWebUrl</span></span>|<span data-ttu-id="442ae-133">Строка</span><span class="sxs-lookup"><span data-stu-id="442ae-133">String</span></span>|<span data-ttu-id="442ae-134">Собрание URL-адреса, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="442ae-134">Meeting URL associated to the call.</span></span> <span data-ttu-id="442ae-135">Может быть недоступным для типа записи вызовов peerToPeer.</span><span class="sxs-lookup"><span data-stu-id="442ae-135">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="442ae-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="442ae-136">lastModifiedDateTime</span></span>|<span data-ttu-id="442ae-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="442ae-137">DateTimeOffset</span></span>|<span data-ttu-id="442ae-138">Время UTC при создания записи вызовов.</span><span class="sxs-lookup"><span data-stu-id="442ae-138">UTC time when the call record was created.</span></span> <span data-ttu-id="442ae-139">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="442ae-139">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="442ae-140">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="442ae-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="442ae-141">модальности</span><span class="sxs-lookup"><span data-stu-id="442ae-141">modalities</span></span>|<span data-ttu-id="442ae-142">коллекция modality</span><span class="sxs-lookup"><span data-stu-id="442ae-142">modality collection</span></span>|<span data-ttu-id="442ae-143">Список всех способов, используемых в вызове.</span><span class="sxs-lookup"><span data-stu-id="442ae-143">List of all the modalities used in the call.</span></span> <span data-ttu-id="442ae-144">Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="442ae-144">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="442ae-145">organizer</span><span class="sxs-lookup"><span data-stu-id="442ae-145">organizer</span></span>|[<span data-ttu-id="442ae-146">identitySet</span><span class="sxs-lookup"><span data-stu-id="442ae-146">identitySet</span></span>](identityset.md)|<span data-ttu-id="442ae-147">Удостоверение организатора.</span><span class="sxs-lookup"><span data-stu-id="442ae-147">The organizing party's identity.</span></span>|
|<span data-ttu-id="442ae-148">participants</span><span class="sxs-lookup"><span data-stu-id="442ae-148">participants</span></span>|<span data-ttu-id="442ae-149">Коллекция [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="442ae-149">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="442ae-150">Список различных удостоверений, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="442ae-150">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="442ae-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="442ae-151">startDateTime</span></span>|<span data-ttu-id="442ae-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="442ae-152">DateTimeOffset</span></span>|<span data-ttu-id="442ae-153">Время UTC, когда первый пользователь присоединился к вызову.</span><span class="sxs-lookup"><span data-stu-id="442ae-153">UTC time when the first user joined the call.</span></span> <span data-ttu-id="442ae-154">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="442ae-154">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="442ae-155">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="442ae-155">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="442ae-156">type</span><span class="sxs-lookup"><span data-stu-id="442ae-156">type</span></span>|<span data-ttu-id="442ae-157">callType</span><span class="sxs-lookup"><span data-stu-id="442ae-157">callType</span></span>|<span data-ttu-id="442ae-158">Указывает тип вызова.</span><span class="sxs-lookup"><span data-stu-id="442ae-158">Indicates the type of the call.</span></span> <span data-ttu-id="442ae-159">Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="442ae-159">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="442ae-160">version</span><span class="sxs-lookup"><span data-stu-id="442ae-160">version</span></span>|<span data-ttu-id="442ae-161">Int64</span><span class="sxs-lookup"><span data-stu-id="442ae-161">Int64</span></span>|<span data-ttu-id="442ae-162">Монотонно увеличивающаяся версия записи вызовов.</span><span class="sxs-lookup"><span data-stu-id="442ae-162">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="442ae-163">Записи вызовов более высокой версии с тем же ИД включают дополнительные данные по сравнению с более низкой версией.</span><span class="sxs-lookup"><span data-stu-id="442ae-163">Higher version call records with the same ID includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="442ae-164">Связи</span><span class="sxs-lookup"><span data-stu-id="442ae-164">Relationships</span></span>

| <span data-ttu-id="442ae-165">Связь</span><span class="sxs-lookup"><span data-stu-id="442ae-165">Relationship</span></span> | <span data-ttu-id="442ae-166">Тип</span><span class="sxs-lookup"><span data-stu-id="442ae-166">Type</span></span>        | <span data-ttu-id="442ae-167">Описание</span><span class="sxs-lookup"><span data-stu-id="442ae-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="442ae-168">сеансы</span><span class="sxs-lookup"><span data-stu-id="442ae-168">sessions</span></span>|<span data-ttu-id="442ae-169">[коллекция microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="442ae-169">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="442ae-170">Список сеансов, участвующих в вызове.</span><span class="sxs-lookup"><span data-stu-id="442ae-170">List of sessions involved in the call.</span></span> <span data-ttu-id="442ae-171">Одноранговые вызовы обычно имеют только один сеанс, в то время как групповые вызовы обычно имеют по крайней мере один сеанс на каждого участника.</span><span class="sxs-lookup"><span data-stu-id="442ae-171">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="442ae-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="442ae-172">Read-only.</span></span> <span data-ttu-id="442ae-173">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="442ae-173">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="442ae-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="442ae-174">JSON representation</span></span>

<span data-ttu-id="442ae-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="442ae-175">The following is a JSON representation of the resource.</span></span>

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


