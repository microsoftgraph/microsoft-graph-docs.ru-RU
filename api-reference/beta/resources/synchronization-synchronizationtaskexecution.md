---
title: Тип ресурса synchronizationTaskExecution
description: Суммирует результаты запуска задания синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ac42a91ec35c1d81d81efa52f4306bbd1cfb2f55
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135039"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="f148d-103">Тип ресурса synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="f148d-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="f148d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f148d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f148d-105">Суммирует результаты запуска задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f148d-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="f148d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f148d-106">Properties</span></span>
| <span data-ttu-id="f148d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f148d-107">Property</span></span>     | <span data-ttu-id="f148d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f148d-108">Type</span></span>   |<span data-ttu-id="f148d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f148d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f148d-110">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="f148d-110">activityIdentifier</span></span>           |<span data-ttu-id="f148d-111">Строка</span><span class="sxs-lookup"><span data-stu-id="f148d-111">String</span></span> |<span data-ttu-id="f148d-112">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="f148d-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="f148d-113">countEntitled</span><span class="sxs-lookup"><span data-stu-id="f148d-113">countEntitled</span></span>                |<span data-ttu-id="f148d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-114">Int64</span></span>  |<span data-ttu-id="f148d-115">Количество обработанных записей, которые были назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="f148d-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="f148d-116">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="f148d-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="f148d-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-117">Int64</span></span>  |<span data-ttu-id="f148d-118">Количество обработанных записей, которые были назначены для предоставления.</span><span class="sxs-lookup"><span data-stu-id="f148d-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="f148d-119">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="f148d-119">countEscrowed</span></span>                |<span data-ttu-id="f148d-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-120">Int64</span></span>  |<span data-ttu-id="f148d-121">Количество записей, которые были escrowed (ошибки).</span><span class="sxs-lookup"><span data-stu-id="f148d-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="f148d-122">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="f148d-122">countEscrowedRaw</span></span>             |<span data-ttu-id="f148d-123">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-123">Int64</span></span>  |<span data-ttu-id="f148d-124">Количество записей, которые были escrowed, включая созданные системой escrows.</span><span class="sxs-lookup"><span data-stu-id="f148d-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="f148d-125">countExported</span><span class="sxs-lookup"><span data-stu-id="f148d-125">countExported</span></span>                |<span data-ttu-id="f148d-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-126">Int64</span></span>  |<span data-ttu-id="f148d-127">Количество экспортных записей.</span><span class="sxs-lookup"><span data-stu-id="f148d-127">Count of exported entries.</span></span>|
|<span data-ttu-id="f148d-128">countExports</span><span class="sxs-lookup"><span data-stu-id="f148d-128">countExports</span></span>                 |<span data-ttu-id="f148d-129">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-129">Int64</span></span>  |<span data-ttu-id="f148d-130">Количество записей, которые должны были быть экспортироваться.</span><span class="sxs-lookup"><span data-stu-id="f148d-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="f148d-131">countImported</span><span class="sxs-lookup"><span data-stu-id="f148d-131">countImported</span></span>                |<span data-ttu-id="f148d-132">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-132">Int64</span></span>  |<span data-ttu-id="f148d-133">Количество импортируемых записей.</span><span class="sxs-lookup"><span data-stu-id="f148d-133">Count of imported entries.</span></span>|
|<span data-ttu-id="f148d-134">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="f148d-134">countImportedDeltas</span></span>          |<span data-ttu-id="f148d-135">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-135">Int64</span></span>  |<span data-ttu-id="f148d-136">Количество импортируемых изменений.</span><span class="sxs-lookup"><span data-stu-id="f148d-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="f148d-137">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="f148d-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="f148d-138">Int64</span><span class="sxs-lookup"><span data-stu-id="f148d-138">Int64</span></span>  |<span data-ttu-id="f148d-139">Количество импортируемых изменений, связанных с изменениями ссылок.</span><span class="sxs-lookup"><span data-stu-id="f148d-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="f148d-140">error</span><span class="sxs-lookup"><span data-stu-id="f148d-140">error</span></span>                        |[<span data-ttu-id="f148d-141">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="f148d-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="f148d-142">Если произошла ошибка, содержит объект **synchronizationError** с подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f148d-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="f148d-143">state</span><span class="sxs-lookup"><span data-stu-id="f148d-143">state</span></span>                        |<span data-ttu-id="f148d-144">String</span><span class="sxs-lookup"><span data-stu-id="f148d-144">String</span></span> |<span data-ttu-id="f148d-145">Код, суммарный результат этого запуска.</span><span class="sxs-lookup"><span data-stu-id="f148d-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="f148d-146">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="f148d-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="f148d-147">timeBegan</span><span class="sxs-lookup"><span data-stu-id="f148d-147">timeBegan</span></span>                    |<span data-ttu-id="f148d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f148d-148">DateTimeOffset</span></span>|<span data-ttu-id="f148d-149">Время начала этого задания.</span><span class="sxs-lookup"><span data-stu-id="f148d-149">Time when this job run began.</span></span> <span data-ttu-id="f148d-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f148d-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f148d-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f148d-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f148d-152">timeEnded</span><span class="sxs-lookup"><span data-stu-id="f148d-152">timeEnded</span></span>                    |<span data-ttu-id="f148d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f148d-153">DateTimeOffset</span></span>|<span data-ttu-id="f148d-154">Время окончания этого задания.</span><span class="sxs-lookup"><span data-stu-id="f148d-154">Time when this job run ended.</span></span> <span data-ttu-id="f148d-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f148d-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f148d-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f148d-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f148d-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f148d-157">JSON representation</span></span>

<span data-ttu-id="f148d-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f148d-158">The following is a JSON representation of the resource.</span></span>

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


