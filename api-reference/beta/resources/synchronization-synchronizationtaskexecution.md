---
title: Тип ресурса Синчронизатионтаскексекутион
description: Сводка результатов выполнения задания синхронизации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2aeb64d0ef08d25a8be9b2ed711d6deabfe522a1
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620663"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="8fc25-103">Тип ресурса Синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="8fc25-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fc25-104">Сводка результатов выполнения задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8fc25-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="8fc25-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fc25-105">Properties</span></span>
| <span data-ttu-id="8fc25-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fc25-106">Property</span></span>     | <span data-ttu-id="8fc25-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8fc25-107">Type</span></span>   |<span data-ttu-id="8fc25-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8fc25-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fc25-109">Активитидентифиер</span><span class="sxs-lookup"><span data-stu-id="8fc25-109">activityIdentifier</span></span>           |<span data-ttu-id="8fc25-110">String</span><span class="sxs-lookup"><span data-stu-id="8fc25-110">String</span></span> |<span data-ttu-id="8fc25-111">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="8fc25-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="8fc25-112">Каунтентитлед</span><span class="sxs-lookup"><span data-stu-id="8fc25-112">countEntitled</span></span>                |<span data-ttu-id="8fc25-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-113">Int64</span></span>  |<span data-ttu-id="8fc25-114">Количество обработанных элементов, которые были назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8fc25-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="8fc25-115">Каунтентитледфорпровисионинг</span><span class="sxs-lookup"><span data-stu-id="8fc25-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="8fc25-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-116">Int64</span></span>  |<span data-ttu-id="8fc25-117">Количество обработанных записей, которые были назначены для подготовки.</span><span class="sxs-lookup"><span data-stu-id="8fc25-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="8fc25-118">Каунтескровед</span><span class="sxs-lookup"><span data-stu-id="8fc25-118">countEscrowed</span></span>                |<span data-ttu-id="8fc25-119">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-119">Int64</span></span>  |<span data-ttu-id="8fc25-120">Количество условных (ошибочных) записей.</span><span class="sxs-lookup"><span data-stu-id="8fc25-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="8fc25-121">Каунтескроведрав</span><span class="sxs-lookup"><span data-stu-id="8fc25-121">countEscrowedRaw</span></span>             |<span data-ttu-id="8fc25-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-122">Int64</span></span>  |<span data-ttu-id="8fc25-123">Количество условных записей, включая созданные системой.</span><span class="sxs-lookup"><span data-stu-id="8fc25-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="8fc25-124">Каунтекспортед</span><span class="sxs-lookup"><span data-stu-id="8fc25-124">countExported</span></span>                |<span data-ttu-id="8fc25-125">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-125">Int64</span></span>  |<span data-ttu-id="8fc25-126">Количество экспортированных записей.</span><span class="sxs-lookup"><span data-stu-id="8fc25-126">Count of exported entries.</span></span>|
|<span data-ttu-id="8fc25-127">Каунтекспортс</span><span class="sxs-lookup"><span data-stu-id="8fc25-127">countExports</span></span>                 |<span data-ttu-id="8fc25-128">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-128">Int64</span></span>  |<span data-ttu-id="8fc25-129">Количество записей, которые ожидались экспортировать.</span><span class="sxs-lookup"><span data-stu-id="8fc25-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="8fc25-130">Каунтимпортед</span><span class="sxs-lookup"><span data-stu-id="8fc25-130">countImported</span></span>                |<span data-ttu-id="8fc25-131">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-131">Int64</span></span>  |<span data-ttu-id="8fc25-132">Количество импортированных записей.</span><span class="sxs-lookup"><span data-stu-id="8fc25-132">Count of imported entries.</span></span>|
|<span data-ttu-id="8fc25-133">Каунтимпортедделтас</span><span class="sxs-lookup"><span data-stu-id="8fc25-133">countImportedDeltas</span></span>          |<span data-ttu-id="8fc25-134">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-134">Int64</span></span>  |<span data-ttu-id="8fc25-135">Количество импортированных изменений изменений.</span><span class="sxs-lookup"><span data-stu-id="8fc25-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="8fc25-136">Каунтимпортедреференцеделтас</span><span class="sxs-lookup"><span data-stu-id="8fc25-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="8fc25-137">Int64</span><span class="sxs-lookup"><span data-stu-id="8fc25-137">Int64</span></span>  |<span data-ttu-id="8fc25-138">Количество импортированных изменений изменений, относящихся к изменениям ссылок.</span><span class="sxs-lookup"><span data-stu-id="8fc25-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="8fc25-139">error</span><span class="sxs-lookup"><span data-stu-id="8fc25-139">error</span></span>                        |[<span data-ttu-id="8fc25-140">Синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="8fc25-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="8fc25-141">Если обнаружена ошибка, содержит объект **синчронизатионеррор** со сведениями.</span><span class="sxs-lookup"><span data-stu-id="8fc25-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="8fc25-142">state</span><span class="sxs-lookup"><span data-stu-id="8fc25-142">state</span></span>                        |<span data-ttu-id="8fc25-143">String</span><span class="sxs-lookup"><span data-stu-id="8fc25-143">String</span></span> |<span data-ttu-id="8fc25-144">Код, суммирующий результат этого запуска.</span><span class="sxs-lookup"><span data-stu-id="8fc25-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="8fc25-145">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="8fc25-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="8fc25-146">Тимебеган</span><span class="sxs-lookup"><span data-stu-id="8fc25-146">timeBegan</span></span>                    |<span data-ttu-id="8fc25-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fc25-147">DateTimeOffset</span></span>|<span data-ttu-id="8fc25-148">Время начала выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="8fc25-148">Time when this job run began.</span></span> <span data-ttu-id="8fc25-149">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8fc25-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fc25-150">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8fc25-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8fc25-151">Тиминдед</span><span class="sxs-lookup"><span data-stu-id="8fc25-151">timeEnded</span></span>                    |<span data-ttu-id="8fc25-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fc25-152">DateTimeOffset</span></span>|<span data-ttu-id="8fc25-153">Время окончания выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="8fc25-153">Time when this job run ended.</span></span> <span data-ttu-id="8fc25-154">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8fc25-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fc25-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8fc25-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fc25-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fc25-156">JSON representation</span></span>

<span data-ttu-id="8fc25-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fc25-157">The following is a JSON representation of the resource.</span></span>

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
