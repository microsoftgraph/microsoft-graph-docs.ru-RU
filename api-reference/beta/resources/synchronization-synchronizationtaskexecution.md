---
title: Тип ресурса Синчронизатионтаскексекутион
description: Сводка результатов выполнения задания синхронизации.
localization_priority: Normal
ms.openlocfilehash: 37a0fd57269cef6d3cb03c5cc5c38d3024fe198d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453865"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="ce74c-103">Тип ресурса Синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="ce74c-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce74c-104">Сводка результатов выполнения задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ce74c-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="ce74c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce74c-105">Properties</span></span>
| <span data-ttu-id="ce74c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce74c-106">Property</span></span>     | <span data-ttu-id="ce74c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ce74c-107">Type</span></span>   |<span data-ttu-id="ce74c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ce74c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce74c-109">Активитидентифиер</span><span class="sxs-lookup"><span data-stu-id="ce74c-109">activityIdentifier</span></span>           |<span data-ttu-id="ce74c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="ce74c-110">String</span></span> |<span data-ttu-id="ce74c-111">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="ce74c-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="ce74c-112">Каунтентитлед</span><span class="sxs-lookup"><span data-stu-id="ce74c-112">countEntitled</span></span>                |<span data-ttu-id="ce74c-113">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-113">Int64</span></span>  |<span data-ttu-id="ce74c-114">Количество обработанных элементов, которые были назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="ce74c-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="ce74c-115">Каунтентитледфорпровисионинг</span><span class="sxs-lookup"><span data-stu-id="ce74c-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="ce74c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-116">Int64</span></span>  |<span data-ttu-id="ce74c-117">Количество обработанных записей, которые были назначены для подготовки.</span><span class="sxs-lookup"><span data-stu-id="ce74c-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="ce74c-118">Каунтескровед</span><span class="sxs-lookup"><span data-stu-id="ce74c-118">countEscrowed</span></span>                |<span data-ttu-id="ce74c-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-119">Int64</span></span>  |<span data-ttu-id="ce74c-120">Количество условных (ошибочных) записей.</span><span class="sxs-lookup"><span data-stu-id="ce74c-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="ce74c-121">Каунтескроведрав</span><span class="sxs-lookup"><span data-stu-id="ce74c-121">countEscrowedRaw</span></span>             |<span data-ttu-id="ce74c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-122">Int64</span></span>  |<span data-ttu-id="ce74c-123">Количество условных записей, включая созданные системой.</span><span class="sxs-lookup"><span data-stu-id="ce74c-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="ce74c-124">Каунтекспортед</span><span class="sxs-lookup"><span data-stu-id="ce74c-124">countExported</span></span>                |<span data-ttu-id="ce74c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-125">Int64</span></span>  |<span data-ttu-id="ce74c-126">Количество экспортированных записей.</span><span class="sxs-lookup"><span data-stu-id="ce74c-126">Count of exported entries.</span></span>|
|<span data-ttu-id="ce74c-127">Каунтекспортс</span><span class="sxs-lookup"><span data-stu-id="ce74c-127">countExports</span></span>                 |<span data-ttu-id="ce74c-128">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-128">Int64</span></span>  |<span data-ttu-id="ce74c-129">Количество записей, которые ожидались экспортировать.</span><span class="sxs-lookup"><span data-stu-id="ce74c-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="ce74c-130">Каунтимпортед</span><span class="sxs-lookup"><span data-stu-id="ce74c-130">countImported</span></span>                |<span data-ttu-id="ce74c-131">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-131">Int64</span></span>  |<span data-ttu-id="ce74c-132">Количество импортированных записей.</span><span class="sxs-lookup"><span data-stu-id="ce74c-132">Count of imported entries.</span></span>|
|<span data-ttu-id="ce74c-133">Каунтимпортедделтас</span><span class="sxs-lookup"><span data-stu-id="ce74c-133">countImportedDeltas</span></span>          |<span data-ttu-id="ce74c-134">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-134">Int64</span></span>  |<span data-ttu-id="ce74c-135">Количество импортированных изменений изменений.</span><span class="sxs-lookup"><span data-stu-id="ce74c-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="ce74c-136">Каунтимпортедреференцеделтас</span><span class="sxs-lookup"><span data-stu-id="ce74c-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="ce74c-137">Int64</span><span class="sxs-lookup"><span data-stu-id="ce74c-137">Int64</span></span>  |<span data-ttu-id="ce74c-138">Количество импортированных изменений изменений, относящихся к изменениям ссылок.</span><span class="sxs-lookup"><span data-stu-id="ce74c-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="ce74c-139">error</span><span class="sxs-lookup"><span data-stu-id="ce74c-139">error</span></span>                        |[<span data-ttu-id="ce74c-140">Синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="ce74c-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="ce74c-141">Если обнаружена ошибка, содержит объект **синчронизатионеррор** со сведениями.</span><span class="sxs-lookup"><span data-stu-id="ce74c-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="ce74c-142">state</span><span class="sxs-lookup"><span data-stu-id="ce74c-142">state</span></span>                        |<span data-ttu-id="ce74c-143">String</span><span class="sxs-lookup"><span data-stu-id="ce74c-143">String</span></span> |<span data-ttu-id="ce74c-144">Код, суммирующий результат этого запуска.</span><span class="sxs-lookup"><span data-stu-id="ce74c-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="ce74c-145">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="ce74c-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="ce74c-146">Тимебеган</span><span class="sxs-lookup"><span data-stu-id="ce74c-146">timeBegan</span></span>                    |<span data-ttu-id="ce74c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce74c-147">DateTimeOffset</span></span>|<span data-ttu-id="ce74c-148">Время начала выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="ce74c-148">Time when this job run began.</span></span> <span data-ttu-id="ce74c-149">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ce74c-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce74c-150">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ce74c-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ce74c-151">Тиминдед</span><span class="sxs-lookup"><span data-stu-id="ce74c-151">timeEnded</span></span>                    |<span data-ttu-id="ce74c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce74c-152">DateTimeOffset</span></span>|<span data-ttu-id="ce74c-153">Время окончания выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="ce74c-153">Time when this job run ended.</span></span> <span data-ttu-id="ce74c-154">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ce74c-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce74c-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ce74c-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce74c-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce74c-156">JSON representation</span></span>

<span data-ttu-id="ce74c-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce74c-157">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtaskexecution.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
