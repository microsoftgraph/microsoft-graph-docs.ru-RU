---
title: Тип ресурса synchronizationTaskExecution
description: Сводка результатов запустите задание синхронизации.
ms.openlocfilehash: 4aefba4bdf9ab850892344e6e34683e81d1a1afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078579"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="00490-103">Тип ресурса synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="00490-103">synchronizationTaskExecution resource type</span></span>

> <span data-ttu-id="00490-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00490-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00490-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00490-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00490-106">Сводка результатов запустите задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="00490-106">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="00490-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="00490-107">Properties</span></span>
| <span data-ttu-id="00490-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="00490-108">Property</span></span>     | <span data-ttu-id="00490-109">Тип</span><span class="sxs-lookup"><span data-stu-id="00490-109">Type</span></span>   |<span data-ttu-id="00490-110">Description</span><span class="sxs-lookup"><span data-stu-id="00490-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00490-111">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="00490-111">activityIdentifier</span></span>           |<span data-ttu-id="00490-112">String</span><span class="sxs-lookup"><span data-stu-id="00490-112">String</span></span> |<span data-ttu-id="00490-113">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="00490-113">Identifier of the job run.</span></span>|
|<span data-ttu-id="00490-114">countEntitled</span><span class="sxs-lookup"><span data-stu-id="00490-114">countEntitled</span></span>                |<span data-ttu-id="00490-115">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-115">Int64</span></span>  |<span data-ttu-id="00490-116">Число обработанных записей, которые были им назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="00490-116">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="00490-117">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="00490-117">countEntitledForProvisioning</span></span> |<span data-ttu-id="00490-118">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-118">Int64</span></span>  |<span data-ttu-id="00490-119">Число обработанных записей, которые были им назначены для подготовки.</span><span class="sxs-lookup"><span data-stu-id="00490-119">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="00490-120">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="00490-120">countEscrowed</span></span>                |<span data-ttu-id="00490-121">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-121">Int64</span></span>  |<span data-ttu-id="00490-122">Число записей, которые были депонированные (ошибки).</span><span class="sxs-lookup"><span data-stu-id="00490-122">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="00490-123">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="00490-123">countEscrowedRaw</span></span>             |<span data-ttu-id="00490-124">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-124">Int64</span></span>  |<span data-ttu-id="00490-125">Число записей, которые были депонированные, включая сгенерированное системой escrows.</span><span class="sxs-lookup"><span data-stu-id="00490-125">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="00490-126">countExported</span><span class="sxs-lookup"><span data-stu-id="00490-126">countExported</span></span>                |<span data-ttu-id="00490-127">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-127">Int64</span></span>  |<span data-ttu-id="00490-128">Число экспортированные операции.</span><span class="sxs-lookup"><span data-stu-id="00490-128">Count of exported entries.</span></span>|
|<span data-ttu-id="00490-129">countExports</span><span class="sxs-lookup"><span data-stu-id="00490-129">countExports</span></span>                 |<span data-ttu-id="00490-130">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-130">Int64</span></span>  |<span data-ttu-id="00490-131">Число записей, которые были им также экспортировать.</span><span class="sxs-lookup"><span data-stu-id="00490-131">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="00490-132">countImported</span><span class="sxs-lookup"><span data-stu-id="00490-132">countImported</span></span>                |<span data-ttu-id="00490-133">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-133">Int64</span></span>  |<span data-ttu-id="00490-134">Число импортированных записей.</span><span class="sxs-lookup"><span data-stu-id="00490-134">Count of imported entries.</span></span>|
|<span data-ttu-id="00490-135">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="00490-135">countImportedDeltas</span></span>          |<span data-ttu-id="00490-136">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-136">Int64</span></span>  |<span data-ttu-id="00490-137">Число импортированных дельта изменения.</span><span class="sxs-lookup"><span data-stu-id="00490-137">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="00490-138">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="00490-138">countImportedReferenceDeltas</span></span> |<span data-ttu-id="00490-139">Int64</span><span class="sxs-lookup"><span data-stu-id="00490-139">Int64</span></span>  |<span data-ttu-id="00490-140">Число импортированных дельта изменения, относящиеся к изменений ссылок.</span><span class="sxs-lookup"><span data-stu-id="00490-140">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="00490-141">error</span><span class="sxs-lookup"><span data-stu-id="00490-141">error</span></span>                        |[<span data-ttu-id="00490-142">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="00490-142">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="00490-143">Если произошла ошибка, содержит объект **synchronizationError** с подробностями.</span><span class="sxs-lookup"><span data-stu-id="00490-143">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="00490-144">state</span><span class="sxs-lookup"><span data-stu-id="00490-144">state</span></span>                        |<span data-ttu-id="00490-145">String</span><span class="sxs-lookup"><span data-stu-id="00490-145">String</span></span> |<span data-ttu-id="00490-146">Подведение итогов в результате выполнения кода.</span><span class="sxs-lookup"><span data-stu-id="00490-146">Code summarizing the result of this run.</span></span> <span data-ttu-id="00490-147">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="00490-147">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="00490-148">timeBegan</span><span class="sxs-lookup"><span data-stu-id="00490-148">timeBegan</span></span>                    |<span data-ttu-id="00490-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00490-149">DateTimeOffset</span></span>|<span data-ttu-id="00490-150">При выполнении этого задания времени начала.</span><span class="sxs-lookup"><span data-stu-id="00490-150">Time when this job run began.</span></span> <span data-ttu-id="00490-151">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="00490-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="00490-152">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="00490-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="00490-153">timeEnded</span><span class="sxs-lookup"><span data-stu-id="00490-153">timeEnded</span></span>                    |<span data-ttu-id="00490-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00490-154">DateTimeOffset</span></span>|<span data-ttu-id="00490-155">При выполнении этого задания времени окончания.</span><span class="sxs-lookup"><span data-stu-id="00490-155">Time when this job run ended.</span></span> <span data-ttu-id="00490-156">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="00490-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="00490-157">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="00490-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00490-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00490-158">JSON representation</span></span>

<span data-ttu-id="00490-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00490-159">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->