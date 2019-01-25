---
title: Тип ресурса synchronizationTaskExecution
description: Сводка результатов запустите задание синхронизации.
localization_priority: Normal
ms.openlocfilehash: 37a0fd57269cef6d3cb03c5cc5c38d3024fe198d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510556"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="d28a7-103">Тип ресурса synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="d28a7-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d28a7-104">Сводка результатов запустите задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d28a7-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="d28a7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d28a7-105">Properties</span></span>
| <span data-ttu-id="d28a7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d28a7-106">Property</span></span>     | <span data-ttu-id="d28a7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d28a7-107">Type</span></span>   |<span data-ttu-id="d28a7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d28a7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d28a7-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d28a7-109">activityIdentifier</span></span>           |<span data-ttu-id="d28a7-110">String</span><span class="sxs-lookup"><span data-stu-id="d28a7-110">String</span></span> |<span data-ttu-id="d28a7-111">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="d28a7-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="d28a7-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="d28a7-112">countEntitled</span></span>                |<span data-ttu-id="d28a7-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-113">Int64</span></span>  |<span data-ttu-id="d28a7-114">Число обработанных записей, которые были им назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="d28a7-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="d28a7-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="d28a7-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="d28a7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-116">Int64</span></span>  |<span data-ttu-id="d28a7-117">Число обработанных записей, которые были им назначены для подготовки.</span><span class="sxs-lookup"><span data-stu-id="d28a7-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="d28a7-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="d28a7-118">countEscrowed</span></span>                |<span data-ttu-id="d28a7-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-119">Int64</span></span>  |<span data-ttu-id="d28a7-120">Число записей, которые были депонированные (ошибки).</span><span class="sxs-lookup"><span data-stu-id="d28a7-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="d28a7-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="d28a7-121">countEscrowedRaw</span></span>             |<span data-ttu-id="d28a7-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-122">Int64</span></span>  |<span data-ttu-id="d28a7-123">Число записей, которые были депонированные, включая сгенерированное системой escrows.</span><span class="sxs-lookup"><span data-stu-id="d28a7-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="d28a7-124">countExported</span><span class="sxs-lookup"><span data-stu-id="d28a7-124">countExported</span></span>                |<span data-ttu-id="d28a7-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-125">Int64</span></span>  |<span data-ttu-id="d28a7-126">Число экспортированные операции.</span><span class="sxs-lookup"><span data-stu-id="d28a7-126">Count of exported entries.</span></span>|
|<span data-ttu-id="d28a7-127">countExports</span><span class="sxs-lookup"><span data-stu-id="d28a7-127">countExports</span></span>                 |<span data-ttu-id="d28a7-128">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-128">Int64</span></span>  |<span data-ttu-id="d28a7-129">Число записей, которые были им также экспортировать.</span><span class="sxs-lookup"><span data-stu-id="d28a7-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="d28a7-130">countImported</span><span class="sxs-lookup"><span data-stu-id="d28a7-130">countImported</span></span>                |<span data-ttu-id="d28a7-131">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-131">Int64</span></span>  |<span data-ttu-id="d28a7-132">Число импортированных записей.</span><span class="sxs-lookup"><span data-stu-id="d28a7-132">Count of imported entries.</span></span>|
|<span data-ttu-id="d28a7-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="d28a7-133">countImportedDeltas</span></span>          |<span data-ttu-id="d28a7-134">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-134">Int64</span></span>  |<span data-ttu-id="d28a7-135">Число импортированных дельта изменения.</span><span class="sxs-lookup"><span data-stu-id="d28a7-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="d28a7-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="d28a7-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="d28a7-137">Int64</span><span class="sxs-lookup"><span data-stu-id="d28a7-137">Int64</span></span>  |<span data-ttu-id="d28a7-138">Число импортированных дельта изменения, относящиеся к изменений ссылок.</span><span class="sxs-lookup"><span data-stu-id="d28a7-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="d28a7-139">error</span><span class="sxs-lookup"><span data-stu-id="d28a7-139">error</span></span>                        |[<span data-ttu-id="d28a7-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="d28a7-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="d28a7-141">Если произошла ошибка, содержит объект **synchronizationError** с подробностями.</span><span class="sxs-lookup"><span data-stu-id="d28a7-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="d28a7-142">state</span><span class="sxs-lookup"><span data-stu-id="d28a7-142">state</span></span>                        |<span data-ttu-id="d28a7-143">String</span><span class="sxs-lookup"><span data-stu-id="d28a7-143">String</span></span> |<span data-ttu-id="d28a7-144">Подведение итогов в результате выполнения кода.</span><span class="sxs-lookup"><span data-stu-id="d28a7-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="d28a7-145">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="d28a7-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="d28a7-146">timeBegan</span><span class="sxs-lookup"><span data-stu-id="d28a7-146">timeBegan</span></span>                    |<span data-ttu-id="d28a7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d28a7-147">DateTimeOffset</span></span>|<span data-ttu-id="d28a7-148">При выполнении этого задания времени начала.</span><span class="sxs-lookup"><span data-stu-id="d28a7-148">Time when this job run began.</span></span> <span data-ttu-id="d28a7-149">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d28a7-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d28a7-150">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d28a7-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d28a7-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="d28a7-151">timeEnded</span></span>                    |<span data-ttu-id="d28a7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d28a7-152">DateTimeOffset</span></span>|<span data-ttu-id="d28a7-153">При выполнении этого задания времени окончания.</span><span class="sxs-lookup"><span data-stu-id="d28a7-153">Time when this job run ended.</span></span> <span data-ttu-id="d28a7-154">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d28a7-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d28a7-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d28a7-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d28a7-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d28a7-156">JSON representation</span></span>

<span data-ttu-id="d28a7-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d28a7-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtaskexecution.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
