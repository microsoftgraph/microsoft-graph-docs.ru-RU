---
title: Тип ресурса Синчронизатионстатус
description: Представляет текущее состояние Синчронизатионжоб.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5019c506d2ef27a645deb0d24580892403dbdb2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052525"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="aa8b3-103">Тип ресурса Синчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="aa8b3-103">synchronizationStatus resource type</span></span>

<span data-ttu-id="aa8b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa8b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa8b3-105">Представляет текущее состояние [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="aa8b3-105">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aa8b3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa8b3-106">Properties</span></span>

| <span data-ttu-id="aa8b3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa8b3-107">Property</span></span>                              | <span data-ttu-id="aa8b3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aa8b3-108">Type</span></span>      | <span data-ttu-id="aa8b3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aa8b3-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="aa8b3-110">code</span><span class="sxs-lookup"><span data-stu-id="aa8b3-110">code</span></span>|<span data-ttu-id="aa8b3-111">Строка</span><span class="sxs-lookup"><span data-stu-id="aa8b3-111">String</span></span>|<span data-ttu-id="aa8b3-112">Высокий уровень кода состояния задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-112">High-level status code of the synchronization job.</span></span> <span data-ttu-id="aa8b3-113">Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-113">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="aa8b3-114">каунтсукцессивекомплетефаилурес</span><span class="sxs-lookup"><span data-stu-id="aa8b3-114">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="aa8b3-115">Int64</span><span class="sxs-lookup"><span data-stu-id="aa8b3-115">Int64</span></span>|<span data-ttu-id="aa8b3-116">Количество последовательных попыток выполнения этого задания.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-116">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="aa8b3-117">ескровспрунед</span><span class="sxs-lookup"><span data-stu-id="aa8b3-117">escrowsPruned</span></span>|<span data-ttu-id="aa8b3-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa8b3-118">Boolean</span></span>|<span data-ttu-id="aa8b3-119">`true` значение, которое было удаляться из-за ошибок на уровне объектов во время первоначальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-119">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="aa8b3-120">Если во время первоначальной синхронизации вы повлияете на пороговое значение, то получится пороговое значение ошибок, которые обычно помещают в карантин.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-120">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="aa8b3-121">Вместо того чтобы переходить в карантин, процесс синхронизации очищает ошибки задания и продолжается до завершения первоначальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-121">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="aa8b3-122">После завершения первоначальной синхронизации задание будет приостановлено и ждать, пока клиент очистит ошибки.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-122">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="aa8b3-123">ластексекутион</span><span class="sxs-lookup"><span data-stu-id="aa8b3-123">lastExecution</span></span>|[<span data-ttu-id="aa8b3-124">синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="aa8b3-124">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="aa8b3-125">Сведения о последнем выполнении задания.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-125">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="aa8b3-126">ластсукцессфулексекутион</span><span class="sxs-lookup"><span data-stu-id="aa8b3-126">lastSuccessfulExecution</span></span>|[<span data-ttu-id="aa8b3-127">синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="aa8b3-127">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="aa8b3-128">Сведения о последнем выполнении задания, у которого нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-128">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="aa8b3-129">ластсукцессфулексекутионвисекспортс</span><span class="sxs-lookup"><span data-stu-id="aa8b3-129">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="aa8b3-130">синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="aa8b3-130">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="aa8b3-131">Сведения о последнем выполнении задания, экспортируемые объекты в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-131">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="aa8b3-132">progress</span><span class="sxs-lookup"><span data-stu-id="aa8b3-132">progress</span></span>|<span data-ttu-id="aa8b3-133">Коллекция [синчронизатионпрогресс](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="aa8b3-133">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="aa8b3-134">Сведения о ходе выполнения задания в направлении завершения.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-134">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="aa8b3-135">папку</span><span class="sxs-lookup"><span data-stu-id="aa8b3-135">quarantine</span></span>|[<span data-ttu-id="aa8b3-136">синчронизатионкуарантине</span><span class="sxs-lookup"><span data-stu-id="aa8b3-136">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="aa8b3-137">Если задание находится в карантине, сведения о карантине.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-137">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="aa8b3-138">стеадистатефирстачиеведтиме</span><span class="sxs-lookup"><span data-stu-id="aa8b3-138">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="aa8b3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa8b3-139">DateTimeOffset</span></span>|<span data-ttu-id="aa8b3-140">Время, в течение которого было выполнено стабильное состояние (больше изменений процесса).</span><span class="sxs-lookup"><span data-stu-id="aa8b3-140">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="aa8b3-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aa8b3-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa8b3-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aa8b3-143">стеадистателастачиеведтиме</span><span class="sxs-lookup"><span data-stu-id="aa8b3-143">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="aa8b3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa8b3-144">DateTimeOffset</span></span>|<span data-ttu-id="aa8b3-145">Время, в течение которого было последнее время последнего изменения процесса (без дополнительных изменений).</span><span class="sxs-lookup"><span data-stu-id="aa8b3-145">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="aa8b3-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aa8b3-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa8b3-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aa8b3-148">синчронизедентрикаунтбитипе</span><span class="sxs-lookup"><span data-stu-id="aa8b3-148">synchronizedEntryCountByType</span></span>|<span data-ttu-id="aa8b3-149">Коллекция [стрингкэйлонгвалуепаир](synchronization-stringkeylongvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="aa8b3-149">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="aa8b3-150">Число синхронизированных объектов, перечисленных по типу объекта.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-150">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="aa8b3-151">траублешутингурл</span><span class="sxs-lookup"><span data-stu-id="aa8b3-151">troubleshootingUrl</span></span>|<span data-ttu-id="aa8b3-152">Строка</span><span class="sxs-lookup"><span data-stu-id="aa8b3-152">String</span></span>|<span data-ttu-id="aa8b3-153">В случае ошибки URL-адрес с действиями по устранению неполадок для проблемы.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-153">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="aa8b3-154">Сведения о коде состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="aa8b3-154">Synchronization status code details</span></span>

| <span data-ttu-id="aa8b3-155">Значение</span><span class="sxs-lookup"><span data-stu-id="aa8b3-155">Value</span></span>                              | <span data-ttu-id="aa8b3-156">Описание</span><span class="sxs-lookup"><span data-stu-id="aa8b3-156">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="aa8b3-157">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="aa8b3-157">NotConfigured</span></span>                       |<span data-ttu-id="aa8b3-158">Задание не настроено и никогда не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-158">Job was not configured and never run.</span></span> <span data-ttu-id="aa8b3-159">Авторизация не предоставлена.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-159">No authorization was provided.</span></span> |
|<span data-ttu-id="aa8b3-160">нотрун</span><span class="sxs-lookup"><span data-stu-id="aa8b3-160">NotRun</span></span>                              |<span data-ttu-id="aa8b3-161">Задание было настроено и, возможно, начато, но не завершило свое первое выполнение.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-161">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="aa8b3-162">Активное</span><span class="sxs-lookup"><span data-stu-id="aa8b3-162">Active</span></span>                              |<span data-ttu-id="aa8b3-163">Задание выполняется периодически.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-163">Job is running periodically.</span></span>|
|<span data-ttu-id="aa8b3-164">Приостановлено</span><span class="sxs-lookup"><span data-stu-id="aa8b3-164">Paused</span></span>                              |<span data-ttu-id="aa8b3-165">Задание было приостановлено (обычно администратором), но в настоящее время оно не запущено, но состояние задания сохраняется.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-165">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="aa8b3-166">Карантин</span><span class="sxs-lookup"><span data-stu-id="aa8b3-166">Quarantine</span></span>                          |<span data-ttu-id="aa8b3-167">Задание находится в карантине.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-167">Job is in quarantine.</span></span> <span data-ttu-id="aa8b3-168">Это может произойти при большом объеме ошибок или критических ошибках, таких как отозванные или просроченные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-168">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="aa8b3-169">Во время карантина процесс синхронизации будет пытаться запустить задание с ограниченной частотой.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-169">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa8b3-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa8b3-170">JSON representation</span></span>

<span data-ttu-id="aa8b3-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-171">The following is a JSON representation of the resource.</span></span>

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


