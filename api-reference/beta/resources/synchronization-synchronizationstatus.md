---
title: Тип ресурса synchronizationStatus
description: Представляет текущее состояние synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bb832fa8d62f2c666b430c242a49bd9138de1b57
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135053"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="e9a16-103">Тип ресурса synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="e9a16-103">synchronizationStatus resource type</span></span>

<span data-ttu-id="e9a16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9a16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9a16-105">Представляет текущее состояние [synchronizationJob.](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="e9a16-105">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e9a16-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9a16-106">Properties</span></span>

| <span data-ttu-id="e9a16-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9a16-107">Property</span></span>                              | <span data-ttu-id="e9a16-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e9a16-108">Type</span></span>      | <span data-ttu-id="e9a16-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e9a16-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="e9a16-110">code</span><span class="sxs-lookup"><span data-stu-id="e9a16-110">code</span></span>|<span data-ttu-id="e9a16-111">Строка</span><span class="sxs-lookup"><span data-stu-id="e9a16-111">String</span></span>|<span data-ttu-id="e9a16-112">Высокоуровневый код состояния задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e9a16-112">High-level status code of the synchronization job.</span></span> <span data-ttu-id="e9a16-113">Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="e9a16-113">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="e9a16-114">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="e9a16-114">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="e9a16-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e9a16-115">Int64</span></span>|<span data-ttu-id="e9a16-116">Количество последовательных сбойов этого задания.</span><span class="sxs-lookup"><span data-stu-id="e9a16-116">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="e9a16-117">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="e9a16-117">escrowsPruned</span></span>|<span data-ttu-id="e9a16-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9a16-118">Boolean</span></span>|<span data-ttu-id="e9a16-119">`true` если объектные объекты задания (ошибки на уровне объекта) были обрезаются во время начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e9a16-119">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="e9a16-120">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span><span class="sxs-lookup"><span data-stu-id="e9a16-120">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="e9a16-121">Вместо того чтобы ходить в карантин, процесс синхронизации очищает ошибки задания и продолжается до завершения начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e9a16-121">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="e9a16-122">После завершения начальной синхронизации задание будет приостановлено и будет ждать, пока клиент очистит ошибки.</span><span class="sxs-lookup"><span data-stu-id="e9a16-122">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="e9a16-123">lastExecution</span><span class="sxs-lookup"><span data-stu-id="e9a16-123">lastExecution</span></span>|[<span data-ttu-id="e9a16-124">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="e9a16-124">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="e9a16-125">Сведения о последнем выполнении задания.</span><span class="sxs-lookup"><span data-stu-id="e9a16-125">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="e9a16-126">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="e9a16-126">lastSuccessfulExecution</span></span>|[<span data-ttu-id="e9a16-127">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="e9a16-127">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="e9a16-128">Сведения о последнем выполнении этого задания без ошибок.</span><span class="sxs-lookup"><span data-stu-id="e9a16-128">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="e9a16-129">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="e9a16-129">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="e9a16-130">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="e9a16-130">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="e9a16-131">Сведения о последнем выполнении задания, которое экспортирует объекты в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="e9a16-131">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="e9a16-132">progress</span><span class="sxs-lookup"><span data-stu-id="e9a16-132">progress</span></span>|<span data-ttu-id="e9a16-133">[Коллекция synchronizationProgress](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="e9a16-133">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="e9a16-134">Сведения о ходе выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="e9a16-134">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="e9a16-135">карантин</span><span class="sxs-lookup"><span data-stu-id="e9a16-135">quarantine</span></span>|[<span data-ttu-id="e9a16-136">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="e9a16-136">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="e9a16-137">Если задание находится в карантине, сведения о карантине.</span><span class="sxs-lookup"><span data-stu-id="e9a16-137">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="e9a16-138">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="e9a16-138">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="e9a16-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9a16-139">DateTimeOffset</span></span>|<span data-ttu-id="e9a16-140">Время, когда было достигнуто стабильное состояние (больше не внося изменений в процесс).</span><span class="sxs-lookup"><span data-stu-id="e9a16-140">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="e9a16-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e9a16-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9a16-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e9a16-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e9a16-143">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="e9a16-143">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="e9a16-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9a16-144">DateTimeOffset</span></span>|<span data-ttu-id="e9a16-145">Время последнего достижения устойчивого состояния (без изменений в процессе).</span><span class="sxs-lookup"><span data-stu-id="e9a16-145">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="e9a16-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e9a16-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9a16-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e9a16-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e9a16-148">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="e9a16-148">synchronizedEntryCountByType</span></span>|<span data-ttu-id="e9a16-149">[Коллекция stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e9a16-149">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="e9a16-150">Количество синхронизированных объектов, перечисленных по типу объекта.</span><span class="sxs-lookup"><span data-stu-id="e9a16-150">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="e9a16-151">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="e9a16-151">troubleshootingUrl</span></span>|<span data-ttu-id="e9a16-152">Строка</span><span class="sxs-lookup"><span data-stu-id="e9a16-152">String</span></span>|<span data-ttu-id="e9a16-153">В случае ошибки URL-адрес с действиями по устранению неполадок для проблемы.</span><span class="sxs-lookup"><span data-stu-id="e9a16-153">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="e9a16-154">Сведения о коде состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="e9a16-154">Synchronization status code details</span></span>

| <span data-ttu-id="e9a16-155">Значение</span><span class="sxs-lookup"><span data-stu-id="e9a16-155">Value</span></span>                              | <span data-ttu-id="e9a16-156">Описание</span><span class="sxs-lookup"><span data-stu-id="e9a16-156">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="e9a16-157">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="e9a16-157">NotConfigured</span></span>                       |<span data-ttu-id="e9a16-158">Задание не было настроено и никогда не запускалось.</span><span class="sxs-lookup"><span data-stu-id="e9a16-158">Job was not configured and never run.</span></span> <span data-ttu-id="e9a16-159">Авторизация не предоставлена.</span><span class="sxs-lookup"><span data-stu-id="e9a16-159">No authorization was provided.</span></span> |
|<span data-ttu-id="e9a16-160">NotRun</span><span class="sxs-lookup"><span data-stu-id="e9a16-160">NotRun</span></span>                              |<span data-ttu-id="e9a16-161">Задание было настроено и, возможно, запущено, но не завершило свой первый запуск.</span><span class="sxs-lookup"><span data-stu-id="e9a16-161">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="e9a16-162">Активное</span><span class="sxs-lookup"><span data-stu-id="e9a16-162">Active</span></span>                              |<span data-ttu-id="e9a16-163">Задание работает периодически.</span><span class="sxs-lookup"><span data-stu-id="e9a16-163">Job is running periodically.</span></span>|
|<span data-ttu-id="e9a16-164">Приостановлено</span><span class="sxs-lookup"><span data-stu-id="e9a16-164">Paused</span></span>                              |<span data-ttu-id="e9a16-165">Задание было приостановлено (обычно администратором) и в настоящее время не запущено, но состояние задания сохраняется.</span><span class="sxs-lookup"><span data-stu-id="e9a16-165">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="e9a16-166">Карантин</span><span class="sxs-lookup"><span data-stu-id="e9a16-166">Quarantine</span></span>                          |<span data-ttu-id="e9a16-167">Задание находится в карантине.</span><span class="sxs-lookup"><span data-stu-id="e9a16-167">Job is in quarantine.</span></span> <span data-ttu-id="e9a16-168">Это может произойти в случае большого объема ошибок или критических ошибок, таких как отозванные или просроченные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="e9a16-168">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="e9a16-169">В карантине процесс синхронизации попытается выполнить задание с уменьшенной частотой.</span><span class="sxs-lookup"><span data-stu-id="e9a16-169">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9a16-170">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e9a16-170">JSON representation</span></span>

<span data-ttu-id="e9a16-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9a16-171">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


