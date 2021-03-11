---
title: тип ресурса синхронизацииTaskExecution
description: Суммирует результаты работы синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d83092949e1f27c9dac9744d2b4b16be4bcbae0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722050"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="971f8-103">тип ресурса синхронизацииTaskExecution</span><span class="sxs-lookup"><span data-stu-id="971f8-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="971f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="971f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="971f8-105">Суммирует результаты работы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="971f8-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="971f8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="971f8-106">Properties</span></span>
| <span data-ttu-id="971f8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="971f8-107">Property</span></span>     | <span data-ttu-id="971f8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="971f8-108">Type</span></span>   |<span data-ttu-id="971f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="971f8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="971f8-110">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="971f8-110">activityIdentifier</span></span>           |<span data-ttu-id="971f8-111">String</span><span class="sxs-lookup"><span data-stu-id="971f8-111">String</span></span> |<span data-ttu-id="971f8-112">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="971f8-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="971f8-113">countEntitled</span><span class="sxs-lookup"><span data-stu-id="971f8-113">countEntitled</span></span>                |<span data-ttu-id="971f8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-114">Int64</span></span>  |<span data-ttu-id="971f8-115">Количество обработанных записей, которые были назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="971f8-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="971f8-116">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="971f8-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="971f8-117">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-117">Int64</span></span>  |<span data-ttu-id="971f8-118">Количество обработанных записей, которые были назначены для предварительной обработки.</span><span class="sxs-lookup"><span data-stu-id="971f8-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="971f8-119">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="971f8-119">countEscrowed</span></span>                |<span data-ttu-id="971f8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-120">Int64</span></span>  |<span data-ttu-id="971f8-121">Количество записей, которые были escrowed (ошибки).</span><span class="sxs-lookup"><span data-stu-id="971f8-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="971f8-122">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="971f8-122">countEscrowedRaw</span></span>             |<span data-ttu-id="971f8-123">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-123">Int64</span></span>  |<span data-ttu-id="971f8-124">Количество записей, которые были депонированы, включая системные эскроу-</span><span class="sxs-lookup"><span data-stu-id="971f8-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="971f8-125">countExported</span><span class="sxs-lookup"><span data-stu-id="971f8-125">countExported</span></span>                |<span data-ttu-id="971f8-126">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-126">Int64</span></span>  |<span data-ttu-id="971f8-127">Количество экспортных записей.</span><span class="sxs-lookup"><span data-stu-id="971f8-127">Count of exported entries.</span></span>|
|<span data-ttu-id="971f8-128">countExports</span><span class="sxs-lookup"><span data-stu-id="971f8-128">countExports</span></span>                 |<span data-ttu-id="971f8-129">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-129">Int64</span></span>  |<span data-ttu-id="971f8-130">Количество записей, которые должны были экспортироваться.</span><span class="sxs-lookup"><span data-stu-id="971f8-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="971f8-131">countImported</span><span class="sxs-lookup"><span data-stu-id="971f8-131">countImported</span></span>                |<span data-ttu-id="971f8-132">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-132">Int64</span></span>  |<span data-ttu-id="971f8-133">Количество импортных записей.</span><span class="sxs-lookup"><span data-stu-id="971f8-133">Count of imported entries.</span></span>|
|<span data-ttu-id="971f8-134">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="971f8-134">countImportedDeltas</span></span>          |<span data-ttu-id="971f8-135">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-135">Int64</span></span>  |<span data-ttu-id="971f8-136">Количество импортируемых изменений дельты.</span><span class="sxs-lookup"><span data-stu-id="971f8-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="971f8-137">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="971f8-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="971f8-138">Int64</span><span class="sxs-lookup"><span data-stu-id="971f8-138">Int64</span></span>  |<span data-ttu-id="971f8-139">Количество импортируемых изменений дельты, относящихся к эталонным изменениям.</span><span class="sxs-lookup"><span data-stu-id="971f8-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="971f8-140">error</span><span class="sxs-lookup"><span data-stu-id="971f8-140">error</span></span>                        |[<span data-ttu-id="971f8-141">синхронизацияError</span><span class="sxs-lookup"><span data-stu-id="971f8-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="971f8-142">В случае ошибки содержится объект **синхронизацииError** с подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="971f8-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="971f8-143">state</span><span class="sxs-lookup"><span data-stu-id="971f8-143">state</span></span>                        |<span data-ttu-id="971f8-144">String</span><span class="sxs-lookup"><span data-stu-id="971f8-144">String</span></span> |<span data-ttu-id="971f8-145">Код, подводя итоги этого запуска.</span><span class="sxs-lookup"><span data-stu-id="971f8-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="971f8-146">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="971f8-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="971f8-147">timeBegan</span><span class="sxs-lookup"><span data-stu-id="971f8-147">timeBegan</span></span>                    |<span data-ttu-id="971f8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="971f8-148">DateTimeOffset</span></span>|<span data-ttu-id="971f8-149">Время начала этого запуска задания.</span><span class="sxs-lookup"><span data-stu-id="971f8-149">Time when this job run began.</span></span> <span data-ttu-id="971f8-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="971f8-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="971f8-151">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="971f8-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="971f8-152">timeEnded</span><span class="sxs-lookup"><span data-stu-id="971f8-152">timeEnded</span></span>                    |<span data-ttu-id="971f8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="971f8-153">DateTimeOffset</span></span>|<span data-ttu-id="971f8-154">Время окончания этого задания.</span><span class="sxs-lookup"><span data-stu-id="971f8-154">Time when this job run ended.</span></span> <span data-ttu-id="971f8-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="971f8-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="971f8-156">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="971f8-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="971f8-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="971f8-157">JSON representation</span></span>

<span data-ttu-id="971f8-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="971f8-158">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


