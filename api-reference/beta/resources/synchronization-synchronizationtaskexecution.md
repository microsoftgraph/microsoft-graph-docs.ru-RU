---
title: Тип ресурса Синчронизатионтаскексекутион
description: Сводка результатов выполнения задания синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d777a575290699c2a936902614aa8ef0e8b042d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094920"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="23c32-103">Тип ресурса Синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="23c32-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="23c32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23c32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23c32-105">Сводка результатов выполнения задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="23c32-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="23c32-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="23c32-106">Properties</span></span>
| <span data-ttu-id="23c32-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="23c32-107">Property</span></span>     | <span data-ttu-id="23c32-108">Тип</span><span class="sxs-lookup"><span data-stu-id="23c32-108">Type</span></span>   |<span data-ttu-id="23c32-109">Описание</span><span class="sxs-lookup"><span data-stu-id="23c32-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23c32-110">активитидентифиер</span><span class="sxs-lookup"><span data-stu-id="23c32-110">activityIdentifier</span></span>           |<span data-ttu-id="23c32-111">Строка</span><span class="sxs-lookup"><span data-stu-id="23c32-111">String</span></span> |<span data-ttu-id="23c32-112">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="23c32-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="23c32-113">каунтентитлед</span><span class="sxs-lookup"><span data-stu-id="23c32-113">countEntitled</span></span>                |<span data-ttu-id="23c32-114">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-114">Int64</span></span>  |<span data-ttu-id="23c32-115">Количество обработанных элементов, которые были назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="23c32-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="23c32-116">каунтентитледфорпровисионинг</span><span class="sxs-lookup"><span data-stu-id="23c32-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="23c32-117">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-117">Int64</span></span>  |<span data-ttu-id="23c32-118">Количество обработанных записей, которые были назначены для подготовки.</span><span class="sxs-lookup"><span data-stu-id="23c32-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="23c32-119">каунтескровед</span><span class="sxs-lookup"><span data-stu-id="23c32-119">countEscrowed</span></span>                |<span data-ttu-id="23c32-120">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-120">Int64</span></span>  |<span data-ttu-id="23c32-121">Количество условных (ошибочных) записей.</span><span class="sxs-lookup"><span data-stu-id="23c32-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="23c32-122">каунтескроведрав</span><span class="sxs-lookup"><span data-stu-id="23c32-122">countEscrowedRaw</span></span>             |<span data-ttu-id="23c32-123">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-123">Int64</span></span>  |<span data-ttu-id="23c32-124">Количество условных записей, включая созданные системой.</span><span class="sxs-lookup"><span data-stu-id="23c32-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="23c32-125">каунтекспортед</span><span class="sxs-lookup"><span data-stu-id="23c32-125">countExported</span></span>                |<span data-ttu-id="23c32-126">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-126">Int64</span></span>  |<span data-ttu-id="23c32-127">Количество экспортированных записей.</span><span class="sxs-lookup"><span data-stu-id="23c32-127">Count of exported entries.</span></span>|
|<span data-ttu-id="23c32-128">каунтекспортс</span><span class="sxs-lookup"><span data-stu-id="23c32-128">countExports</span></span>                 |<span data-ttu-id="23c32-129">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-129">Int64</span></span>  |<span data-ttu-id="23c32-130">Количество записей, которые ожидались экспортировать.</span><span class="sxs-lookup"><span data-stu-id="23c32-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="23c32-131">каунтимпортед</span><span class="sxs-lookup"><span data-stu-id="23c32-131">countImported</span></span>                |<span data-ttu-id="23c32-132">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-132">Int64</span></span>  |<span data-ttu-id="23c32-133">Количество импортированных записей.</span><span class="sxs-lookup"><span data-stu-id="23c32-133">Count of imported entries.</span></span>|
|<span data-ttu-id="23c32-134">каунтимпортедделтас</span><span class="sxs-lookup"><span data-stu-id="23c32-134">countImportedDeltas</span></span>          |<span data-ttu-id="23c32-135">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-135">Int64</span></span>  |<span data-ttu-id="23c32-136">Количество импортированных изменений изменений.</span><span class="sxs-lookup"><span data-stu-id="23c32-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="23c32-137">каунтимпортедреференцеделтас</span><span class="sxs-lookup"><span data-stu-id="23c32-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="23c32-138">Int64</span><span class="sxs-lookup"><span data-stu-id="23c32-138">Int64</span></span>  |<span data-ttu-id="23c32-139">Количество импортированных изменений изменений, относящихся к изменениям ссылок.</span><span class="sxs-lookup"><span data-stu-id="23c32-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="23c32-140">error</span><span class="sxs-lookup"><span data-stu-id="23c32-140">error</span></span>                        |[<span data-ttu-id="23c32-141">синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="23c32-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="23c32-142">Если обнаружена ошибка, содержит объект **синчронизатионеррор** со сведениями.</span><span class="sxs-lookup"><span data-stu-id="23c32-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="23c32-143">state</span><span class="sxs-lookup"><span data-stu-id="23c32-143">state</span></span>                        |<span data-ttu-id="23c32-144">String</span><span class="sxs-lookup"><span data-stu-id="23c32-144">String</span></span> |<span data-ttu-id="23c32-145">Код, суммирующий результат этого запуска.</span><span class="sxs-lookup"><span data-stu-id="23c32-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="23c32-146">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="23c32-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="23c32-147">тимебеган</span><span class="sxs-lookup"><span data-stu-id="23c32-147">timeBegan</span></span>                    |<span data-ttu-id="23c32-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23c32-148">DateTimeOffset</span></span>|<span data-ttu-id="23c32-149">Время начала выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="23c32-149">Time when this job run began.</span></span> <span data-ttu-id="23c32-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="23c32-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="23c32-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="23c32-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="23c32-152">тиминдед</span><span class="sxs-lookup"><span data-stu-id="23c32-152">timeEnded</span></span>                    |<span data-ttu-id="23c32-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23c32-153">DateTimeOffset</span></span>|<span data-ttu-id="23c32-154">Время окончания выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="23c32-154">Time when this job run ended.</span></span> <span data-ttu-id="23c32-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="23c32-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="23c32-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="23c32-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23c32-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="23c32-157">JSON representation</span></span>

<span data-ttu-id="23c32-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23c32-158">The following is a JSON representation of the resource.</span></span>

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


