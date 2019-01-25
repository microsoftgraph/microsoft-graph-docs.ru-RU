---
title: Тип ресурса synchronizationRule
description: Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517927"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="8115e-103">Тип ресурса synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="8115e-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8115e-104">Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="8115e-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="8115e-105">**Примечание:** Правила синхронизации определение синхронизации в одном направлении - из исходного каталога в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="8115e-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="8115e-106">Исходный и целевой каталоги определены как часть свойств правила.</span><span class="sxs-lookup"><span data-stu-id="8115e-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="8115e-107">Правила синхронизации обновляются в процессе [синхронизации схемы](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8115e-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8115e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8115e-108">Properties</span></span>

| <span data-ttu-id="8115e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8115e-109">Property</span></span>      | <span data-ttu-id="8115e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8115e-110">Type</span></span>      | <span data-ttu-id="8115e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8115e-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="8115e-112">изменения</span><span class="sxs-lookup"><span data-stu-id="8115e-112">editable</span></span>       |<span data-ttu-id="8115e-113">Логическое</span><span class="sxs-lookup"><span data-stu-id="8115e-113">Boolean</span></span>    |<span data-ttu-id="8115e-114">`true`Если можно настроить правила синхронизации; `false` Если это правило доступно только для чтения и не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="8115e-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="8115e-115">id</span><span class="sxs-lookup"><span data-stu-id="8115e-115">id</span></span>             |<span data-ttu-id="8115e-116">String</span><span class="sxs-lookup"><span data-stu-id="8115e-116">String</span></span>     |<span data-ttu-id="8115e-117">Идентификатор правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8115e-117">Synchronization rule identifier.</span></span> <span data-ttu-id="8115e-118">Должен быть один из идентификаторов, распознаваемых обработчик синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8115e-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="8115e-119">Поддерживается правило, которое идентификаторы можно найти в шаблоне синхронизации, возвращаемых API.</span><span class="sxs-lookup"><span data-stu-id="8115e-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="8115e-120">Метаданные</span><span class="sxs-lookup"><span data-stu-id="8115e-120">metadata</span></span>       |<span data-ttu-id="8115e-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8115e-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="8115e-122">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="8115e-122">Additional extension properties.</span></span> <span data-ttu-id="8115e-123">Если не указано явно группой поддержки, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="8115e-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="8115e-124">name</span><span class="sxs-lookup"><span data-stu-id="8115e-124">name</span></span>           |<span data-ttu-id="8115e-125">String</span><span class="sxs-lookup"><span data-stu-id="8115e-125">String</span></span>     |<span data-ttu-id="8115e-126">Понятное имя правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8115e-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="8115e-127">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="8115e-127">Not nullable.</span></span>|
|<span data-ttu-id="8115e-128">objectMappings</span><span class="sxs-lookup"><span data-stu-id="8115e-128">objectMappings</span></span> |<span data-ttu-id="8115e-129">[objectMapping](synchronization-objectmapping.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8115e-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="8115e-130">Коллекция сопоставления объектов, поддерживаемых правило.</span><span class="sxs-lookup"><span data-stu-id="8115e-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="8115e-131">Указывает обработчик синхронизации объектов, которые должны быть синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="8115e-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="8115e-132">priority</span><span class="sxs-lookup"><span data-stu-id="8115e-132">priority</span></span>       |<span data-ttu-id="8115e-133">Целое число</span><span class="sxs-lookup"><span data-stu-id="8115e-133">Integer</span></span>    |<span data-ttu-id="8115e-134">Приоритет относительно других правил в [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8115e-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="8115e-135">Правила с наименьшим номером приоритет будут обрабатываться в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="8115e-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="8115e-136">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="8115e-136">sourceDirectoryName</span></span>       |<span data-ttu-id="8115e-137">String</span><span class="sxs-lookup"><span data-stu-id="8115e-137">String</span></span>    |<span data-ttu-id="8115e-138">Имя исходного каталога.</span><span class="sxs-lookup"><span data-stu-id="8115e-138">Name of the source directory.</span></span> <span data-ttu-id="8115e-139">Должно соответствовать одному из определений каталога в [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8115e-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="8115e-140">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="8115e-140">targetDirectoryName</span></span>       |<span data-ttu-id="8115e-141">String</span><span class="sxs-lookup"><span data-stu-id="8115e-141">String</span></span>    |<span data-ttu-id="8115e-142">Имя в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="8115e-142">Name of the target directory.</span></span> <span data-ttu-id="8115e-143">Должно соответствовать одному из определений каталога в [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8115e-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8115e-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8115e-144">JSON representation</span></span>

<span data-ttu-id="8115e-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8115e-145">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationrule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
