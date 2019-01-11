---
title: Тип ресурса synchronizationStatus
description: Представляет текущее состояние synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 01f30338d7f6d4388554df08bf91655136c24a12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817033"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="f63ab-103">Тип ресурса synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="f63ab-103">synchronizationStatus resource type</span></span>

> <span data-ttu-id="f63ab-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f63ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f63ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f63ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f63ab-106">Представляет текущее состояние [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="f63ab-106">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f63ab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f63ab-107">Properties</span></span>

| <span data-ttu-id="f63ab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f63ab-108">Property</span></span>                              | <span data-ttu-id="f63ab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f63ab-109">Type</span></span>      | <span data-ttu-id="f63ab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f63ab-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="f63ab-111">code</span><span class="sxs-lookup"><span data-stu-id="f63ab-111">code</span></span>|<span data-ttu-id="f63ab-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f63ab-112">String</span></span>|<span data-ttu-id="f63ab-113">Код высокого уровня состояния заданий синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f63ab-113">High-level status code of the synchronization job.</span></span> <span data-ttu-id="f63ab-114">Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="f63ab-114">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="f63ab-115">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="f63ab-115">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="f63ab-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f63ab-116">Int64</span></span>|<span data-ttu-id="f63ab-117">Последовательные время это задание не удалось.</span><span class="sxs-lookup"><span data-stu-id="f63ab-117">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="f63ab-118">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="f63ab-118">escrowsPruned</span></span>|<span data-ttu-id="f63ab-119">Логический</span><span class="sxs-lookup"><span data-stu-id="f63ab-119">Boolean</span></span>|<span data-ttu-id="f63ab-120">`true`Если задание escrows (ошибки уровня объекта) удаляются во время начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f63ab-120">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="f63ab-121">Escrows можно удаляются при достижении порогового значения ошибок, которые обычно находится в карантине задание во время начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f63ab-121">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="f63ab-122">Вдаваясь в карантин, процесс синхронизации очищает ошибок заданий и продолжает вплоть до завершения начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f63ab-122">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="f63ab-123">После завершения начальной синхронизации задание приостановить и дождитесь клиента для очистки ошибки.</span><span class="sxs-lookup"><span data-stu-id="f63ab-123">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="f63ab-124">lastExecution</span><span class="sxs-lookup"><span data-stu-id="f63ab-124">lastExecution</span></span>|[<span data-ttu-id="f63ab-125">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="f63ab-125">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="f63ab-126">Подробные сведения о последнего выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="f63ab-126">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="f63ab-127">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="f63ab-127">lastSuccessfulExecution</span></span>|[<span data-ttu-id="f63ab-128">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="f63ab-128">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="f63ab-129">Подробные сведения о последнего выполнения этого задания, не пришлось возникновения ошибок.</span><span class="sxs-lookup"><span data-stu-id="f63ab-129">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="f63ab-130">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="f63ab-130">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="f63ab-131">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="f63ab-131">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="f63ab-132">Подробные сведения о последнего выполнения задания, которое экспортированных объектов в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="f63ab-132">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="f63ab-133">progress</span><span class="sxs-lookup"><span data-stu-id="f63ab-133">progress</span></span>|<span data-ttu-id="f63ab-134">[synchronizationProgress](synchronization-synchronizationprogress.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f63ab-134">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="f63ab-135">Подробные сведения о ходе выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="f63ab-135">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="f63ab-136">карантин</span><span class="sxs-lookup"><span data-stu-id="f63ab-136">quarantine</span></span>|[<span data-ttu-id="f63ab-137">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="f63ab-137">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="f63ab-138">Если задание находится в карантине, сведения о карантине.</span><span class="sxs-lookup"><span data-stu-id="f63ab-138">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="f63ab-139">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="f63ab-139">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="f63ab-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f63ab-140">DateTimeOffset</span></span>|<span data-ttu-id="f63ab-141">Время, когда сначала достигнутым в стабильном состоянии (больше нет изменений для процесса).</span><span class="sxs-lookup"><span data-stu-id="f63ab-141">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="f63ab-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f63ab-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f63ab-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f63ab-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f63ab-144">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="f63ab-144">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="f63ab-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f63ab-145">DateTimeOffset</span></span>|<span data-ttu-id="f63ab-146">Время, когда последнего достигнуть стабильном состоянии (больше нет изменений для процесса).</span><span class="sxs-lookup"><span data-stu-id="f63ab-146">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="f63ab-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f63ab-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f63ab-148">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f63ab-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f63ab-149">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="f63ab-149">synchronizedEntryCountByType</span></span>|<span data-ttu-id="f63ab-150">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f63ab-150">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="f63ab-151">Количество синхронизированных объектов, перечисленные по типу объекта.</span><span class="sxs-lookup"><span data-stu-id="f63ab-151">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="f63ab-152">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="f63ab-152">troubleshootingUrl</span></span>|<span data-ttu-id="f63ab-153">Строка</span><span class="sxs-lookup"><span data-stu-id="f63ab-153">String</span></span>|<span data-ttu-id="f63ab-154">В случае ошибки, URL-адрес с помощью действия по устранению неполадок для проблему.</span><span class="sxs-lookup"><span data-stu-id="f63ab-154">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="f63ab-155">Сведения о коде состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="f63ab-155">Synchronization status code details</span></span>

| <span data-ttu-id="f63ab-156">Значение</span><span class="sxs-lookup"><span data-stu-id="f63ab-156">Value</span></span>                              | <span data-ttu-id="f63ab-157">Описание</span><span class="sxs-lookup"><span data-stu-id="f63ab-157">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="f63ab-158">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="f63ab-158">NotConfigured</span></span>                       |<span data-ttu-id="f63ab-159">Задание не настроен и ни разу.</span><span class="sxs-lookup"><span data-stu-id="f63ab-159">Job was not configured and never run.</span></span> <span data-ttu-id="f63ab-160">Не было указано.</span><span class="sxs-lookup"><span data-stu-id="f63ab-160">No authorization was provided.</span></span> |
|<span data-ttu-id="f63ab-161">NotRun</span><span class="sxs-lookup"><span data-stu-id="f63ab-161">NotRun</span></span>                              |<span data-ttu-id="f63ab-162">Задание был настроен и возможно работы, но еще не завершено его первого потока.</span><span class="sxs-lookup"><span data-stu-id="f63ab-162">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="f63ab-163">Активное</span><span class="sxs-lookup"><span data-stu-id="f63ab-163">Active</span></span>                              |<span data-ttu-id="f63ab-164">Задание выполняется периодически.</span><span class="sxs-lookup"><span data-stu-id="f63ab-164">Job is running periodically.</span></span>|
|<span data-ttu-id="f63ab-165">Приостановлена работа</span><span class="sxs-lookup"><span data-stu-id="f63ab-165">Paused</span></span>                              |<span data-ttu-id="f63ab-166">Задание приостановлено (обычно администратором) и в настоящее время не работает, но сохранять состояние задания.</span><span class="sxs-lookup"><span data-stu-id="f63ab-166">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="f63ab-167">Карантин</span><span class="sxs-lookup"><span data-stu-id="f63ab-167">Quarantine</span></span>                          |<span data-ttu-id="f63ab-168">Задание находится в карантине.</span><span class="sxs-lookup"><span data-stu-id="f63ab-168">Job is in quarantine.</span></span> <span data-ttu-id="f63ab-169">Это может произойти при наличии большое количество ошибок или критические ошибки, такие как отозван Просроченные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="f63ab-169">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="f63ab-170">Находясь в карантин, процесс синхронизации будет пытаться с ограниченной частоту выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="f63ab-170">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f63ab-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f63ab-171">JSON representation</span></span>

<span data-ttu-id="f63ab-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f63ab-172">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
