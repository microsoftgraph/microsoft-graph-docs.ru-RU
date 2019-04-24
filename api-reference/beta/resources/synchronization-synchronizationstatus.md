---
title: Тип ресурса Синчронизатионстатус
description: Представляет текущее состояние Синчронизатионжоб.
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453872"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="d803c-103">Тип ресурса Синчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="d803c-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d803c-104">Представляет текущее состояние [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="d803c-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d803c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d803c-105">Properties</span></span>

| <span data-ttu-id="d803c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d803c-106">Property</span></span>                              | <span data-ttu-id="d803c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d803c-107">Type</span></span>      | <span data-ttu-id="d803c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d803c-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="d803c-109">code</span><span class="sxs-lookup"><span data-stu-id="d803c-109">code</span></span>|<span data-ttu-id="d803c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="d803c-110">String</span></span>|<span data-ttu-id="d803c-111">Высокий уровень кода состояния задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d803c-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="d803c-112">Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="d803c-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="d803c-113">Каунтсукцессивекомплетефаилурес</span><span class="sxs-lookup"><span data-stu-id="d803c-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="d803c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d803c-114">Int64</span></span>|<span data-ttu-id="d803c-115">Количество последовательных попыток выполнения этого задания.</span><span class="sxs-lookup"><span data-stu-id="d803c-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="d803c-116">Ескровспрунед</span><span class="sxs-lookup"><span data-stu-id="d803c-116">escrowsPruned</span></span>|<span data-ttu-id="d803c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d803c-117">Boolean</span></span>|<span data-ttu-id="d803c-118">`true`значение, которое было удаляться из-за ошибок на уровне объектов во время первоначальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d803c-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="d803c-119">Если во время первоначальной синхронизации вы повлияете на пороговое значение, то получится пороговое значение ошибок, которые обычно помещают в карантин.</span><span class="sxs-lookup"><span data-stu-id="d803c-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="d803c-120">Вместо того чтобы переходить в карантин, процесс синхронизации очищает ошибки задания и продолжается до завершения первоначальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d803c-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="d803c-121">После завершения первоначальной синхронизации задание будет приостановлено и ждать, пока клиент очистит ошибки.</span><span class="sxs-lookup"><span data-stu-id="d803c-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="d803c-122">Ластексекутион</span><span class="sxs-lookup"><span data-stu-id="d803c-122">lastExecution</span></span>|[<span data-ttu-id="d803c-123">Синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="d803c-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="d803c-124">Сведения о последнем выполнении задания.</span><span class="sxs-lookup"><span data-stu-id="d803c-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="d803c-125">Ластсукцессфулексекутион</span><span class="sxs-lookup"><span data-stu-id="d803c-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="d803c-126">Синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="d803c-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="d803c-127">Сведения о последнем выполнении задания, у которого нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="d803c-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="d803c-128">Ластсукцессфулексекутионвисекспортс</span><span class="sxs-lookup"><span data-stu-id="d803c-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="d803c-129">Синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="d803c-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="d803c-130">Сведения о последнем выполнении задания, экспортируемые объекты в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="d803c-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="d803c-131">progress</span><span class="sxs-lookup"><span data-stu-id="d803c-131">progress</span></span>|<span data-ttu-id="d803c-132">Коллекция [синчронизатионпрогресс](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="d803c-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="d803c-133">Сведения о ходе выполнения задания в направлении завершения.</span><span class="sxs-lookup"><span data-stu-id="d803c-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="d803c-134">папку</span><span class="sxs-lookup"><span data-stu-id="d803c-134">quarantine</span></span>|[<span data-ttu-id="d803c-135">Синчронизатионкуарантине</span><span class="sxs-lookup"><span data-stu-id="d803c-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="d803c-136">Если задание находится в карантине, сведения о карантине.</span><span class="sxs-lookup"><span data-stu-id="d803c-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="d803c-137">Стеадистатефирстачиеведтиме</span><span class="sxs-lookup"><span data-stu-id="d803c-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="d803c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d803c-138">DateTimeOffset</span></span>|<span data-ttu-id="d803c-139">Время, в течение которого было выполнено стабильное состояние (больше изменений процесса).</span><span class="sxs-lookup"><span data-stu-id="d803c-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="d803c-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d803c-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d803c-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d803c-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d803c-142">Стеадистателастачиеведтиме</span><span class="sxs-lookup"><span data-stu-id="d803c-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="d803c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d803c-143">DateTimeOffset</span></span>|<span data-ttu-id="d803c-144">Время, в течение которого было последнее время последнего изменения процесса (без дополнительных изменений).</span><span class="sxs-lookup"><span data-stu-id="d803c-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="d803c-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d803c-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d803c-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d803c-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d803c-147">Синчронизедентрикаунтбитипе</span><span class="sxs-lookup"><span data-stu-id="d803c-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="d803c-148">Коллекция [стрингкэйлонгвалуепаир](synchronization-stringkeylongvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d803c-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="d803c-149">Число синхронизированных объектов, перечисленных по типу объекта.</span><span class="sxs-lookup"><span data-stu-id="d803c-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="d803c-150">Траублешутингурл</span><span class="sxs-lookup"><span data-stu-id="d803c-150">troubleshootingUrl</span></span>|<span data-ttu-id="d803c-151">Строка</span><span class="sxs-lookup"><span data-stu-id="d803c-151">String</span></span>|<span data-ttu-id="d803c-152">В случае ошибки URL-адрес с действиями по устранению неполадок для проблемы.</span><span class="sxs-lookup"><span data-stu-id="d803c-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="d803c-153">Сведения о коде состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="d803c-153">Synchronization status code details</span></span>

| <span data-ttu-id="d803c-154">Значение</span><span class="sxs-lookup"><span data-stu-id="d803c-154">Value</span></span>                              | <span data-ttu-id="d803c-155">Описание</span><span class="sxs-lookup"><span data-stu-id="d803c-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="d803c-156">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="d803c-156">NotConfigured</span></span>                       |<span data-ttu-id="d803c-157">Задание не настроено и никогда не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="d803c-157">Job was not configured and never run.</span></span> <span data-ttu-id="d803c-158">Авторизация не предоставлена.</span><span class="sxs-lookup"><span data-stu-id="d803c-158">No authorization was provided.</span></span> |
|<span data-ttu-id="d803c-159">Нотрун</span><span class="sxs-lookup"><span data-stu-id="d803c-159">NotRun</span></span>                              |<span data-ttu-id="d803c-160">Задание было настроено и, возможно, начато, но не завершило свое первое выполнение.</span><span class="sxs-lookup"><span data-stu-id="d803c-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="d803c-161">Активное</span><span class="sxs-lookup"><span data-stu-id="d803c-161">Active</span></span>                              |<span data-ttu-id="d803c-162">Задание выполняется периодически.</span><span class="sxs-lookup"><span data-stu-id="d803c-162">Job is running periodically.</span></span>|
|<span data-ttu-id="d803c-163">Приостановлено</span><span class="sxs-lookup"><span data-stu-id="d803c-163">Paused</span></span>                              |<span data-ttu-id="d803c-164">Задание было приостановлено (обычно администратором), но в настоящее время оно не запущено, но состояние задания сохраняется.</span><span class="sxs-lookup"><span data-stu-id="d803c-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="d803c-165">Карантин</span><span class="sxs-lookup"><span data-stu-id="d803c-165">Quarantine</span></span>                          |<span data-ttu-id="d803c-166">Задание находится в карантине.</span><span class="sxs-lookup"><span data-stu-id="d803c-166">Job is in quarantine.</span></span> <span data-ttu-id="d803c-167">Это может произойти при большом объеме ошибок или критических ошибках, таких как отозванные или просроченные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="d803c-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="d803c-168">Во время карантина процесс синхронизации будет пытаться запустить задание с ограниченной частотой.</span><span class="sxs-lookup"><span data-stu-id="d803c-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d803c-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d803c-169">JSON representation</span></span>

<span data-ttu-id="d803c-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d803c-170">The following is a JSON representation of the resource.</span></span>

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
