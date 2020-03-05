---
title: Тип ресурса Синчронизатионтаскексекутион
description: Сводка результатов выполнения задания синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 936201202a36d85f8b7a0caa5cfb1cebb002bbb1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520025"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="07c5a-103">Тип ресурса Синчронизатионтаскексекутион</span><span class="sxs-lookup"><span data-stu-id="07c5a-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="07c5a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="07c5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07c5a-105">Сводка результатов выполнения задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="07c5a-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="07c5a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="07c5a-106">Properties</span></span>
| <span data-ttu-id="07c5a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="07c5a-107">Property</span></span>     | <span data-ttu-id="07c5a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="07c5a-108">Type</span></span>   |<span data-ttu-id="07c5a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="07c5a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07c5a-110">активитидентифиер</span><span class="sxs-lookup"><span data-stu-id="07c5a-110">activityIdentifier</span></span>           |<span data-ttu-id="07c5a-111">String</span><span class="sxs-lookup"><span data-stu-id="07c5a-111">String</span></span> |<span data-ttu-id="07c5a-112">Идентификатор запуска задания.</span><span class="sxs-lookup"><span data-stu-id="07c5a-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="07c5a-113">каунтентитлед</span><span class="sxs-lookup"><span data-stu-id="07c5a-113">countEntitled</span></span>                |<span data-ttu-id="07c5a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-114">Int64</span></span>  |<span data-ttu-id="07c5a-115">Количество обработанных элементов, которые были назначены для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="07c5a-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="07c5a-116">каунтентитледфорпровисионинг</span><span class="sxs-lookup"><span data-stu-id="07c5a-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="07c5a-117">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-117">Int64</span></span>  |<span data-ttu-id="07c5a-118">Количество обработанных записей, которые были назначены для подготовки.</span><span class="sxs-lookup"><span data-stu-id="07c5a-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="07c5a-119">каунтескровед</span><span class="sxs-lookup"><span data-stu-id="07c5a-119">countEscrowed</span></span>                |<span data-ttu-id="07c5a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-120">Int64</span></span>  |<span data-ttu-id="07c5a-121">Количество условных (ошибочных) записей.</span><span class="sxs-lookup"><span data-stu-id="07c5a-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="07c5a-122">каунтескроведрав</span><span class="sxs-lookup"><span data-stu-id="07c5a-122">countEscrowedRaw</span></span>             |<span data-ttu-id="07c5a-123">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-123">Int64</span></span>  |<span data-ttu-id="07c5a-124">Количество условных записей, включая созданные системой.</span><span class="sxs-lookup"><span data-stu-id="07c5a-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="07c5a-125">каунтекспортед</span><span class="sxs-lookup"><span data-stu-id="07c5a-125">countExported</span></span>                |<span data-ttu-id="07c5a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-126">Int64</span></span>  |<span data-ttu-id="07c5a-127">Количество экспортированных записей.</span><span class="sxs-lookup"><span data-stu-id="07c5a-127">Count of exported entries.</span></span>|
|<span data-ttu-id="07c5a-128">каунтекспортс</span><span class="sxs-lookup"><span data-stu-id="07c5a-128">countExports</span></span>                 |<span data-ttu-id="07c5a-129">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-129">Int64</span></span>  |<span data-ttu-id="07c5a-130">Количество записей, которые ожидались экспортировать.</span><span class="sxs-lookup"><span data-stu-id="07c5a-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="07c5a-131">каунтимпортед</span><span class="sxs-lookup"><span data-stu-id="07c5a-131">countImported</span></span>                |<span data-ttu-id="07c5a-132">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-132">Int64</span></span>  |<span data-ttu-id="07c5a-133">Количество импортированных записей.</span><span class="sxs-lookup"><span data-stu-id="07c5a-133">Count of imported entries.</span></span>|
|<span data-ttu-id="07c5a-134">каунтимпортедделтас</span><span class="sxs-lookup"><span data-stu-id="07c5a-134">countImportedDeltas</span></span>          |<span data-ttu-id="07c5a-135">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-135">Int64</span></span>  |<span data-ttu-id="07c5a-136">Количество импортированных изменений изменений.</span><span class="sxs-lookup"><span data-stu-id="07c5a-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="07c5a-137">каунтимпортедреференцеделтас</span><span class="sxs-lookup"><span data-stu-id="07c5a-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="07c5a-138">Int64</span><span class="sxs-lookup"><span data-stu-id="07c5a-138">Int64</span></span>  |<span data-ttu-id="07c5a-139">Количество импортированных изменений изменений, относящихся к изменениям ссылок.</span><span class="sxs-lookup"><span data-stu-id="07c5a-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="07c5a-140">error</span><span class="sxs-lookup"><span data-stu-id="07c5a-140">error</span></span>                        |[<span data-ttu-id="07c5a-141">синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="07c5a-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="07c5a-142">Если обнаружена ошибка, содержит объект **синчронизатионеррор** со сведениями.</span><span class="sxs-lookup"><span data-stu-id="07c5a-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="07c5a-143">state</span><span class="sxs-lookup"><span data-stu-id="07c5a-143">state</span></span>                        |<span data-ttu-id="07c5a-144">String</span><span class="sxs-lookup"><span data-stu-id="07c5a-144">String</span></span> |<span data-ttu-id="07c5a-145">Код, суммирующий результат этого запуска.</span><span class="sxs-lookup"><span data-stu-id="07c5a-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="07c5a-146">Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="07c5a-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="07c5a-147">тимебеган</span><span class="sxs-lookup"><span data-stu-id="07c5a-147">timeBegan</span></span>                    |<span data-ttu-id="07c5a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07c5a-148">DateTimeOffset</span></span>|<span data-ttu-id="07c5a-149">Время начала выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="07c5a-149">Time when this job run began.</span></span> <span data-ttu-id="07c5a-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="07c5a-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07c5a-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="07c5a-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="07c5a-152">тиминдед</span><span class="sxs-lookup"><span data-stu-id="07c5a-152">timeEnded</span></span>                    |<span data-ttu-id="07c5a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07c5a-153">DateTimeOffset</span></span>|<span data-ttu-id="07c5a-154">Время окончания выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="07c5a-154">Time when this job run ended.</span></span> <span data-ttu-id="07c5a-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="07c5a-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07c5a-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="07c5a-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07c5a-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07c5a-157">JSON representation</span></span>

<span data-ttu-id="07c5a-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07c5a-158">The following is a JSON representation of the resource.</span></span>

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
