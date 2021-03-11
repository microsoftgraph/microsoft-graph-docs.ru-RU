---
title: тип ресурсов synchronizationStatus
description: Представляет текущее состояние синхронизацииJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 86320e6af31dae39f86ebe87f8490e24c7c33f57
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722057"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="810cb-103">тип ресурсов synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="810cb-103">synchronizationStatus resource type</span></span>

<span data-ttu-id="810cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="810cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="810cb-105">Представляет текущее состояние [синхронизацииJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="810cb-105">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="810cb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="810cb-106">Properties</span></span>

| <span data-ttu-id="810cb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="810cb-107">Property</span></span>                              | <span data-ttu-id="810cb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="810cb-108">Type</span></span>      | <span data-ttu-id="810cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="810cb-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="810cb-110">code</span><span class="sxs-lookup"><span data-stu-id="810cb-110">code</span></span>|<span data-ttu-id="810cb-111">String</span><span class="sxs-lookup"><span data-stu-id="810cb-111">String</span></span>|<span data-ttu-id="810cb-112">Код состояния высокого уровня задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="810cb-112">High-level status code of the synchronization job.</span></span> <span data-ttu-id="810cb-113">Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="810cb-113">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="810cb-114">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="810cb-114">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="810cb-115">Int64</span><span class="sxs-lookup"><span data-stu-id="810cb-115">Int64</span></span>|<span data-ttu-id="810cb-116">Количество последовательных сбойных работ.</span><span class="sxs-lookup"><span data-stu-id="810cb-116">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="810cb-117">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="810cb-117">escrowsPruned</span></span>|<span data-ttu-id="810cb-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="810cb-118">Boolean</span></span>|<span data-ttu-id="810cb-119">`true` если эскроуы задания (ошибки на уровне объекта) были обрезки во время начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="810cb-119">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="810cb-120">Escrows можно обрезать, если во время начальной синхронизации вы достигнете порога ошибок, которые обычно помещали бы задание в карантин.</span><span class="sxs-lookup"><span data-stu-id="810cb-120">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="810cb-121">Вместо того чтобы ходить в карантин, процесс синхронизации очищает ошибки задания и продолжается до завершения начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="810cb-121">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="810cb-122">После завершения начальной синхронизации задание приостанавливется и будет ждать, пока клиент очистит ошибки.</span><span class="sxs-lookup"><span data-stu-id="810cb-122">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="810cb-123">lastExecution</span><span class="sxs-lookup"><span data-stu-id="810cb-123">lastExecution</span></span>|[<span data-ttu-id="810cb-124">синхронизацияTaskExecution</span><span class="sxs-lookup"><span data-stu-id="810cb-124">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="810cb-125">Сведения о последнем выполнении задания.</span><span class="sxs-lookup"><span data-stu-id="810cb-125">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="810cb-126">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="810cb-126">lastSuccessfulExecution</span></span>|[<span data-ttu-id="810cb-127">синхронизацияTaskExecution</span><span class="sxs-lookup"><span data-stu-id="810cb-127">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="810cb-128">Сведения о последнем выполнении этого задания, в котором не было никаких ошибок.</span><span class="sxs-lookup"><span data-stu-id="810cb-128">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="810cb-129">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="810cb-129">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="810cb-130">синхронизацияTaskExecution</span><span class="sxs-lookup"><span data-stu-id="810cb-130">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="810cb-131">Сведения о последнем выполнении задания, которое экспортирует объекты в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="810cb-131">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="810cb-132">progress</span><span class="sxs-lookup"><span data-stu-id="810cb-132">progress</span></span>|<span data-ttu-id="810cb-133">[коллекция synchronizationProgress](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="810cb-133">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="810cb-134">Сведения о ходе выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="810cb-134">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="810cb-135">карантин</span><span class="sxs-lookup"><span data-stu-id="810cb-135">quarantine</span></span>|[<span data-ttu-id="810cb-136">синхронизацияКварантин</span><span class="sxs-lookup"><span data-stu-id="810cb-136">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="810cb-137">Если задание находится в карантине, сведения о карантине.</span><span class="sxs-lookup"><span data-stu-id="810cb-137">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="810cb-138">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="810cb-138">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="810cb-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="810cb-139">DateTimeOffset</span></span>|<span data-ttu-id="810cb-140">Время, когда было достигнуто стабильное состояние (больше никаких изменений в процессе) было достигнуто.</span><span class="sxs-lookup"><span data-stu-id="810cb-140">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="810cb-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="810cb-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="810cb-142">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="810cb-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="810cb-143">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="810cb-143">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="810cb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="810cb-144">DateTimeOffset</span></span>|<span data-ttu-id="810cb-145">Время, когда стабильное состояние (больше не изменяется в процессе) было достигнуто в последний раз.</span><span class="sxs-lookup"><span data-stu-id="810cb-145">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="810cb-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="810cb-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="810cb-147">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="810cb-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="810cb-148">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="810cb-148">synchronizedEntryCountByType</span></span>|<span data-ttu-id="810cb-149">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span><span class="sxs-lookup"><span data-stu-id="810cb-149">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="810cb-150">Количество синхронизированных объектов, перечисленных по типу объекта.</span><span class="sxs-lookup"><span data-stu-id="810cb-150">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="810cb-151">устранение неполадокUrl</span><span class="sxs-lookup"><span data-stu-id="810cb-151">troubleshootingUrl</span></span>|<span data-ttu-id="810cb-152">String</span><span class="sxs-lookup"><span data-stu-id="810cb-152">String</span></span>|<span data-ttu-id="810cb-153">В случае ошибки URL-адрес с действиями по устранению неполадок для проблемы.</span><span class="sxs-lookup"><span data-stu-id="810cb-153">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="810cb-154">Сведения о коде состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="810cb-154">Synchronization status code details</span></span>

| <span data-ttu-id="810cb-155">Значение</span><span class="sxs-lookup"><span data-stu-id="810cb-155">Value</span></span>                              | <span data-ttu-id="810cb-156">Описание</span><span class="sxs-lookup"><span data-stu-id="810cb-156">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="810cb-157">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="810cb-157">NotConfigured</span></span>                       |<span data-ttu-id="810cb-158">Задание не было настроено и никогда не запускалось.</span><span class="sxs-lookup"><span data-stu-id="810cb-158">Job was not configured and never run.</span></span> <span data-ttu-id="810cb-159">Авторизация не была предоставлена.</span><span class="sxs-lookup"><span data-stu-id="810cb-159">No authorization was provided.</span></span> |
|<span data-ttu-id="810cb-160">NotRun</span><span class="sxs-lookup"><span data-stu-id="810cb-160">NotRun</span></span>                              |<span data-ttu-id="810cb-161">Задание было настроено и, возможно, запущено, но не завершило первый запуск.</span><span class="sxs-lookup"><span data-stu-id="810cb-161">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="810cb-162">Активное</span><span class="sxs-lookup"><span data-stu-id="810cb-162">Active</span></span>                              |<span data-ttu-id="810cb-163">Задание работает периодически.</span><span class="sxs-lookup"><span data-stu-id="810cb-163">Job is running periodically.</span></span>|
|<span data-ttu-id="810cb-164">Приостановка</span><span class="sxs-lookup"><span data-stu-id="810cb-164">Paused</span></span>                              |<span data-ttu-id="810cb-165">Задание было приостановлено (обычно администратором) и в настоящее время не запущено, но состояние задания сохранено.</span><span class="sxs-lookup"><span data-stu-id="810cb-165">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="810cb-166">Карантин</span><span class="sxs-lookup"><span data-stu-id="810cb-166">Quarantine</span></span>                          |<span data-ttu-id="810cb-167">Задание находится на карантине.</span><span class="sxs-lookup"><span data-stu-id="810cb-167">Job is in quarantine.</span></span> <span data-ttu-id="810cb-168">Это может произойти, когда существует большой объем ошибок или критически важных ошибок, таких как аннулированные или просроченные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="810cb-168">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="810cb-169">В карантине процесс синхронизации будет пытаться выполнить задание с пониженной частотой.</span><span class="sxs-lookup"><span data-stu-id="810cb-169">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="810cb-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="810cb-170">JSON representation</span></span>

<span data-ttu-id="810cb-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="810cb-171">The following is a JSON representation of the resource.</span></span>

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


