---
title: Тип ресурса synchronizationRule
description: Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.
ms.openlocfilehash: c860228637a6cc3ad9137851408379bd7f779c75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076746"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="c0099-103">Тип ресурса synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="c0099-103">synchronizationRule resource type</span></span>

> <span data-ttu-id="c0099-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0099-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0099-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0099-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0099-106">Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="c0099-106">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="c0099-107">**Примечание:** Правила синхронизации определение синхронизации в одном направлении - из исходного каталога в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="c0099-107">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="c0099-108">Исходный и целевой каталоги определены как часть свойств правила.</span><span class="sxs-lookup"><span data-stu-id="c0099-108">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="c0099-109">Правила синхронизации обновляются в процессе [синхронизации схемы](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c0099-109">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c0099-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0099-110">Properties</span></span>

| <span data-ttu-id="c0099-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0099-111">Property</span></span>      | <span data-ttu-id="c0099-112">Тип</span><span class="sxs-lookup"><span data-stu-id="c0099-112">Type</span></span>      | <span data-ttu-id="c0099-113">Description</span><span class="sxs-lookup"><span data-stu-id="c0099-113">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c0099-114">изменения</span><span class="sxs-lookup"><span data-stu-id="c0099-114">editable</span></span>       |<span data-ttu-id="c0099-115">Логический</span><span class="sxs-lookup"><span data-stu-id="c0099-115">Boolean</span></span>    |<span data-ttu-id="c0099-116">`true`Если можно настроить правила синхронизации; `false` Если это правило доступно только для чтения и не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="c0099-116">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="c0099-117">id</span><span class="sxs-lookup"><span data-stu-id="c0099-117">id</span></span>             |<span data-ttu-id="c0099-118">String</span><span class="sxs-lookup"><span data-stu-id="c0099-118">String</span></span>     |<span data-ttu-id="c0099-119">Идентификатор правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c0099-119">Synchronization rule identifier.</span></span> <span data-ttu-id="c0099-120">Должен быть один из идентификаторов, распознаваемых обработчик синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c0099-120">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="c0099-121">Поддерживается правило, которое идентификаторы можно найти в шаблоне синхронизации, возвращаемых API.</span><span class="sxs-lookup"><span data-stu-id="c0099-121">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="c0099-122">метаданные</span><span class="sxs-lookup"><span data-stu-id="c0099-122">metadata</span></span>       |<span data-ttu-id="c0099-123">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c0099-123">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="c0099-124">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="c0099-124">Additional extension properties.</span></span> <span data-ttu-id="c0099-125">Если не указано явно группой поддержки, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="c0099-125">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c0099-126">name</span><span class="sxs-lookup"><span data-stu-id="c0099-126">name</span></span>           |<span data-ttu-id="c0099-127">String</span><span class="sxs-lookup"><span data-stu-id="c0099-127">String</span></span>     |<span data-ttu-id="c0099-128">Понятное имя правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c0099-128">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="c0099-129">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c0099-129">Not nullable.</span></span>|
|<span data-ttu-id="c0099-130">objectMappings</span><span class="sxs-lookup"><span data-stu-id="c0099-130">objectMappings</span></span> |<span data-ttu-id="c0099-131">[objectMapping](synchronization-objectmapping.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c0099-131">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="c0099-132">Коллекция сопоставления объектов, поддерживаемых правило.</span><span class="sxs-lookup"><span data-stu-id="c0099-132">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="c0099-133">Указывает обработчик синхронизации объектов, которые должны быть синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="c0099-133">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="c0099-134">priority</span><span class="sxs-lookup"><span data-stu-id="c0099-134">priority</span></span>       |<span data-ttu-id="c0099-135">Целое число</span><span class="sxs-lookup"><span data-stu-id="c0099-135">Integer</span></span>    |<span data-ttu-id="c0099-136">Приоритет относительно других правил в [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c0099-136">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="c0099-137">Правила с наименьшим номером приоритет будут обрабатываться в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="c0099-137">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="c0099-138">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="c0099-138">sourceDirectoryName</span></span>       |<span data-ttu-id="c0099-139">String</span><span class="sxs-lookup"><span data-stu-id="c0099-139">String</span></span>    |<span data-ttu-id="c0099-140">Имя исходного каталога.</span><span class="sxs-lookup"><span data-stu-id="c0099-140">Name of the source directory.</span></span> <span data-ttu-id="c0099-141">Должно соответствовать одному из определений каталога в [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c0099-141">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="c0099-142">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="c0099-142">targetDirectoryName</span></span>       |<span data-ttu-id="c0099-143">String</span><span class="sxs-lookup"><span data-stu-id="c0099-143">String</span></span>    |<span data-ttu-id="c0099-144">Имя в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="c0099-144">Name of the target directory.</span></span> <span data-ttu-id="c0099-145">Должно соответствовать одному из определений каталога в [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c0099-145">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0099-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0099-146">JSON representation</span></span>

<span data-ttu-id="c0099-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0099-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->