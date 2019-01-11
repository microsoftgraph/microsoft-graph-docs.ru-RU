---
title: Тип ресурса synchronizationTaskExecution
description: Сводка результатов запустите задание синхронизации.
localization_priority: Normal
ms.openlocfilehash: 99b6c66b15577ee4c6cbbf5ffe44e17cf0672696
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851508"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="335f9-103">Тип ресурса synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="335f9-103">synchronizationTaskExecution resource type</span></span>

> <span data-ttu-id="335f9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="335f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="335f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="335f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="335f9-106">Сводка результатов запустите задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="335f9-106">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="335f9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="335f9-107">Properties</span></span>
| <span data-ttu-id="335f9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="335f9-108">Property</span></span>     | <span data-ttu-id="335f9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="335f9-109">Type</span></span>   |<span data-ttu-id="335f9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="335f9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="335f9-111">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="335f9-111">activityIdentifier</span></span>           |<span data-ttu-id="335f9-112">Строка</span><span class="sxs-lookup"><span data-stu-id="335f9-112">String</span></span> |<span data-ttu-id="335f9-113">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="335f9-113">Identifier of the job run.</span></span>|
|<span data-ttu-id="335f9-114">countEntitled</span><span class="sxs-lookup"><span data-stu-id="335f9-114">countEntitled</span></span>                |<span data-ttu-id="335f9-115">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-115">Int64</span></span>  |<span data-ttu-id="335f9-116">Число обработанных записей, которые были им назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="335f9-116">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="335f9-117">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="335f9-117">countEntitledForProvisioning</span></span> |<span data-ttu-id="335f9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-118">Int64</span></span>  |<span data-ttu-id="335f9-119">Число обработанных записей, которые были им назначены для подготовки.</span><span class="sxs-lookup"><span data-stu-id="335f9-119">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="335f9-120">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="335f9-120">countEscrowed</span></span>                |<span data-ttu-id="335f9-121">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-121">Int64</span></span>  |<span data-ttu-id="335f9-122">Число записей, которые были депонированные (ошибки).</span><span class="sxs-lookup"><span data-stu-id="335f9-122">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="335f9-123">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="335f9-123">countEscrowedRaw</span></span>             |<span data-ttu-id="335f9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-124">Int64</span></span>  |<span data-ttu-id="335f9-125">Число записей, которые были депонированные, включая сгенерированное системой escrows.</span><span class="sxs-lookup"><span data-stu-id="335f9-125">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="335f9-126">countExported</span><span class="sxs-lookup"><span data-stu-id="335f9-126">countExported</span></span>                |<span data-ttu-id="335f9-127">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-127">Int64</span></span>  |<span data-ttu-id="335f9-128">Число экспортированные операции.</span><span class="sxs-lookup"><span data-stu-id="335f9-128">Count of exported entries.</span></span>|
|<span data-ttu-id="335f9-129">countExports</span><span class="sxs-lookup"><span data-stu-id="335f9-129">countExports</span></span>                 |<span data-ttu-id="335f9-130">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-130">Int64</span></span>  |<span data-ttu-id="335f9-131">Число записей, которые были им также экспортировать.</span><span class="sxs-lookup"><span data-stu-id="335f9-131">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="335f9-132">countImported</span><span class="sxs-lookup"><span data-stu-id="335f9-132">countImported</span></span>                |<span data-ttu-id="335f9-133">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-133">Int64</span></span>  |<span data-ttu-id="335f9-134">Число импортированных записей.</span><span class="sxs-lookup"><span data-stu-id="335f9-134">Count of imported entries.</span></span>|
|<span data-ttu-id="335f9-135">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="335f9-135">countImportedDeltas</span></span>          |<span data-ttu-id="335f9-136">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-136">Int64</span></span>  |<span data-ttu-id="335f9-137">Число импортированных дельта изменения.</span><span class="sxs-lookup"><span data-stu-id="335f9-137">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="335f9-138">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="335f9-138">countImportedReferenceDeltas</span></span> |<span data-ttu-id="335f9-139">Int64</span><span class="sxs-lookup"><span data-stu-id="335f9-139">Int64</span></span>  |<span data-ttu-id="335f9-140">Число импортированных дельта изменения, относящиеся к изменений ссылок.</span><span class="sxs-lookup"><span data-stu-id="335f9-140">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="335f9-141">error</span><span class="sxs-lookup"><span data-stu-id="335f9-141">error</span></span>                        |[<span data-ttu-id="335f9-142">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="335f9-142">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="335f9-143">Если произошла ошибка, содержит объект **synchronizationError** с подробностями.</span><span class="sxs-lookup"><span data-stu-id="335f9-143">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="335f9-144">state</span><span class="sxs-lookup"><span data-stu-id="335f9-144">state</span></span>                        |<span data-ttu-id="335f9-145">Строка</span><span class="sxs-lookup"><span data-stu-id="335f9-145">String</span></span> |<span data-ttu-id="335f9-146">Подведение итогов в результате выполнения кода.</span><span class="sxs-lookup"><span data-stu-id="335f9-146">Code summarizing the result of this run.</span></span> <span data-ttu-id="335f9-147">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="335f9-147">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="335f9-148">timeBegan</span><span class="sxs-lookup"><span data-stu-id="335f9-148">timeBegan</span></span>                    |<span data-ttu-id="335f9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="335f9-149">DateTimeOffset</span></span>|<span data-ttu-id="335f9-150">При выполнении этого задания времени начала.</span><span class="sxs-lookup"><span data-stu-id="335f9-150">Time when this job run began.</span></span> <span data-ttu-id="335f9-151">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="335f9-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="335f9-152">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="335f9-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="335f9-153">timeEnded</span><span class="sxs-lookup"><span data-stu-id="335f9-153">timeEnded</span></span>                    |<span data-ttu-id="335f9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="335f9-154">DateTimeOffset</span></span>|<span data-ttu-id="335f9-155">При выполнении этого задания времени окончания.</span><span class="sxs-lookup"><span data-stu-id="335f9-155">Time when this job run ended.</span></span> <span data-ttu-id="335f9-156">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="335f9-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="335f9-157">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="335f9-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="335f9-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="335f9-158">JSON representation</span></span>

<span data-ttu-id="335f9-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="335f9-159">The following is a JSON representation of the resource.</span></span>

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
