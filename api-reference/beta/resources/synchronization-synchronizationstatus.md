---
title: Тип ресурса synchronizationStatus
description: Представляет текущее состояние synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523766"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="829c7-103">Тип ресурса synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="829c7-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="829c7-104">Представляет текущее состояние [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="829c7-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="829c7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="829c7-105">Properties</span></span>

| <span data-ttu-id="829c7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="829c7-106">Property</span></span>                              | <span data-ttu-id="829c7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="829c7-107">Type</span></span>      | <span data-ttu-id="829c7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="829c7-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="829c7-109">code</span><span class="sxs-lookup"><span data-stu-id="829c7-109">code</span></span>|<span data-ttu-id="829c7-110">String</span><span class="sxs-lookup"><span data-stu-id="829c7-110">String</span></span>|<span data-ttu-id="829c7-111">Код высокого уровня состояния заданий синхронизации.</span><span class="sxs-lookup"><span data-stu-id="829c7-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="829c7-112">Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="829c7-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="829c7-113">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="829c7-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="829c7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="829c7-114">Int64</span></span>|<span data-ttu-id="829c7-115">Последовательные время это задание не удалось.</span><span class="sxs-lookup"><span data-stu-id="829c7-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="829c7-116">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="829c7-116">escrowsPruned</span></span>|<span data-ttu-id="829c7-117">Логическое</span><span class="sxs-lookup"><span data-stu-id="829c7-117">Boolean</span></span>|<span data-ttu-id="829c7-118">`true`Если задание escrows (ошибки уровня объекта) удаляются во время начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="829c7-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="829c7-119">Escrows можно удаляются при достижении порогового значения ошибок, которые обычно находится в карантине задание во время начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="829c7-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="829c7-120">Вдаваясь в карантин, процесс синхронизации очищает ошибок заданий и продолжает вплоть до завершения начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="829c7-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="829c7-121">После завершения начальной синхронизации задание приостановить и дождитесь клиента для очистки ошибки.</span><span class="sxs-lookup"><span data-stu-id="829c7-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="829c7-122">lastExecution</span><span class="sxs-lookup"><span data-stu-id="829c7-122">lastExecution</span></span>|[<span data-ttu-id="829c7-123">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="829c7-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="829c7-124">Подробные сведения о последнего выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="829c7-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="829c7-125">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="829c7-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="829c7-126">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="829c7-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="829c7-127">Подробные сведения о последнего выполнения этого задания, не пришлось возникновения ошибок.</span><span class="sxs-lookup"><span data-stu-id="829c7-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="829c7-128">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="829c7-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="829c7-129">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="829c7-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="829c7-130">Подробные сведения о последнего выполнения задания, которое экспортированных объектов в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="829c7-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="829c7-131">Progress</span><span class="sxs-lookup"><span data-stu-id="829c7-131">progress</span></span>|<span data-ttu-id="829c7-132">[synchronizationProgress](synchronization-synchronizationprogress.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="829c7-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="829c7-133">Подробные сведения о ходе выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="829c7-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="829c7-134">карантин</span><span class="sxs-lookup"><span data-stu-id="829c7-134">quarantine</span></span>|[<span data-ttu-id="829c7-135">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="829c7-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="829c7-136">Если задание находится в карантине, сведения о карантине.</span><span class="sxs-lookup"><span data-stu-id="829c7-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="829c7-137">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="829c7-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="829c7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="829c7-138">DateTimeOffset</span></span>|<span data-ttu-id="829c7-139">Время, когда сначала достигнутым в стабильном состоянии (больше нет изменений для процесса).</span><span class="sxs-lookup"><span data-stu-id="829c7-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="829c7-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="829c7-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="829c7-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="829c7-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="829c7-142">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="829c7-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="829c7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="829c7-143">DateTimeOffset</span></span>|<span data-ttu-id="829c7-144">Время, когда последнего достигнуть стабильном состоянии (больше нет изменений для процесса).</span><span class="sxs-lookup"><span data-stu-id="829c7-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="829c7-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="829c7-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="829c7-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="829c7-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="829c7-147">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="829c7-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="829c7-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="829c7-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="829c7-149">Количество синхронизированных объектов, перечисленные по типу объекта.</span><span class="sxs-lookup"><span data-stu-id="829c7-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="829c7-150">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="829c7-150">troubleshootingUrl</span></span>|<span data-ttu-id="829c7-151">String</span><span class="sxs-lookup"><span data-stu-id="829c7-151">String</span></span>|<span data-ttu-id="829c7-152">В случае ошибки, URL-адрес с помощью действия по устранению неполадок для проблему.</span><span class="sxs-lookup"><span data-stu-id="829c7-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="829c7-153">Сведения о коде состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="829c7-153">Synchronization status code details</span></span>

| <span data-ttu-id="829c7-154">Значение</span><span class="sxs-lookup"><span data-stu-id="829c7-154">Value</span></span>                              | <span data-ttu-id="829c7-155">Описание</span><span class="sxs-lookup"><span data-stu-id="829c7-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="829c7-156">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="829c7-156">NotConfigured</span></span>                       |<span data-ttu-id="829c7-157">Задание не настроен и ни разу.</span><span class="sxs-lookup"><span data-stu-id="829c7-157">Job was not configured and never run.</span></span> <span data-ttu-id="829c7-158">Не было указано.</span><span class="sxs-lookup"><span data-stu-id="829c7-158">No authorization was provided.</span></span> |
|<span data-ttu-id="829c7-159">NotRun</span><span class="sxs-lookup"><span data-stu-id="829c7-159">NotRun</span></span>                              |<span data-ttu-id="829c7-160">Задание был настроен и возможно работы, но еще не завершено его первого потока.</span><span class="sxs-lookup"><span data-stu-id="829c7-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="829c7-161">Активное</span><span class="sxs-lookup"><span data-stu-id="829c7-161">Active</span></span>                              |<span data-ttu-id="829c7-162">Задание выполняется периодически.</span><span class="sxs-lookup"><span data-stu-id="829c7-162">Job is running periodically.</span></span>|
|<span data-ttu-id="829c7-163">Приостановлена работа</span><span class="sxs-lookup"><span data-stu-id="829c7-163">Paused</span></span>                              |<span data-ttu-id="829c7-164">Задание приостановлено (обычно администратором) и в настоящее время не работает, но сохранять состояние задания.</span><span class="sxs-lookup"><span data-stu-id="829c7-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="829c7-165">Карантин</span><span class="sxs-lookup"><span data-stu-id="829c7-165">Quarantine</span></span>                          |<span data-ttu-id="829c7-166">Задание находится в карантине.</span><span class="sxs-lookup"><span data-stu-id="829c7-166">Job is in quarantine.</span></span> <span data-ttu-id="829c7-167">Это может произойти при наличии большое количество ошибок или критические ошибки, такие как отозван Просроченные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="829c7-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="829c7-168">Находясь в карантин, процесс синхронизации будет пытаться с ограниченной частоту выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="829c7-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="829c7-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="829c7-169">JSON representation</span></span>

<span data-ttu-id="829c7-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="829c7-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
