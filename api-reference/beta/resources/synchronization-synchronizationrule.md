---
title: Тип ресурса synchronizationRule
description: Определяет, как должна выполняться синхронизация для обдвижки синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 94697fede9ab9055b1a477cfd94edea88f207331
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135999"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="d3b6f-103">Тип ресурса synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="d3b6f-103">synchronizationRule resource type</span></span>

<span data-ttu-id="d3b6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3b6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3b6f-105">Определяет, как должна выполняться синхронизация для обдвижка синхронизации, включая объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходных каталогов должны быть соединяются с объектами в целевом каталоге и как атрибуты должны преобразовываться при их синхронизации из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-105">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="d3b6f-106">**Примечание.** Правила синхронизации определяют синхронизацию в одном направлении — от каталога источника к целевому.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-106">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="d3b6f-107">Исходный и целевой каталоги определяются как часть свойств правила.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-107">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="d3b6f-108">Правила синхронизации обновляются в рамках [схемы синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="d3b6f-108">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d3b6f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3b6f-109">Properties</span></span>

| <span data-ttu-id="d3b6f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3b6f-110">Property</span></span>      | <span data-ttu-id="d3b6f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d3b6f-111">Type</span></span>      | <span data-ttu-id="d3b6f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d3b6f-112">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="d3b6f-113">редактируемый</span><span class="sxs-lookup"><span data-stu-id="d3b6f-113">editable</span></span>       |<span data-ttu-id="d3b6f-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3b6f-114">Boolean</span></span>    |<span data-ttu-id="d3b6f-115">`true` если правило синхронизации можно настроить; `false` если это правило является только для чтения и не должно быть изменено.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-115">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="d3b6f-116">id</span><span class="sxs-lookup"><span data-stu-id="d3b6f-116">id</span></span>             |<span data-ttu-id="d3b6f-117">Строка</span><span class="sxs-lookup"><span data-stu-id="d3b6f-117">String</span></span>     |<span data-ttu-id="d3b6f-118">Идентификатор правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-118">Synchronization rule identifier.</span></span> <span data-ttu-id="d3b6f-119">Должен быть одним из идентификаторов, распознается механизмом синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-119">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="d3b6f-120">Поддерживаемые идентификаторы правил можно найти в шаблоне синхронизации, возвращаемом API.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-120">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="d3b6f-121">метаданные</span><span class="sxs-lookup"><span data-stu-id="d3b6f-121">metadata</span></span>       |<span data-ttu-id="d3b6f-122">[Коллекция stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d3b6f-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="d3b6f-123">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-123">Additional extension properties.</span></span> <span data-ttu-id="d3b6f-124">Если группа поддержки явно не проинструктировали ее, значения метаданных не следует менять.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-124">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="d3b6f-125">name</span><span class="sxs-lookup"><span data-stu-id="d3b6f-125">name</span></span>           |<span data-ttu-id="d3b6f-126">String</span><span class="sxs-lookup"><span data-stu-id="d3b6f-126">String</span></span>     |<span data-ttu-id="d3b6f-127">Понятное для человека имя правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-127">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="d3b6f-128">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-128">Not nullable.</span></span>|
|<span data-ttu-id="d3b6f-129">objectMappings</span><span class="sxs-lookup"><span data-stu-id="d3b6f-129">objectMappings</span></span> |<span data-ttu-id="d3b6f-130">[Коллекция objectMapping](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="d3b6f-130">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="d3b6f-131">Коллекция сопоставлений объектов, поддерживаемых правилом.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-131">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="d3b6f-132">Сообщает механизму синхронизации, какие объекты следует синхронизировать.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-132">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="d3b6f-133">priority</span><span class="sxs-lookup"><span data-stu-id="d3b6f-133">priority</span></span>       |<span data-ttu-id="d3b6f-134">Целое число</span><span class="sxs-lookup"><span data-stu-id="d3b6f-134">Integer</span></span>    |<span data-ttu-id="d3b6f-135">Приоритет относительно других правил в [synchronizationSchema.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="d3b6f-135">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="d3b6f-136">Правила с наименьшим номером приоритета будут обрабатываться в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-136">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="d3b6f-137">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="d3b6f-137">sourceDirectoryName</span></span>       |<span data-ttu-id="d3b6f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="d3b6f-138">String</span></span>    |<span data-ttu-id="d3b6f-139">Имя каталога источника.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-139">Name of the source directory.</span></span> <span data-ttu-id="d3b6f-140">Должно соответствовать одному из определений каталогов в [synchronizationSchema.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="d3b6f-140">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="d3b6f-141">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="d3b6f-141">targetDirectoryName</span></span>       |<span data-ttu-id="d3b6f-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d3b6f-142">String</span></span>    |<span data-ttu-id="d3b6f-143">Имя целевого каталога.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-143">Name of the target directory.</span></span> <span data-ttu-id="d3b6f-144">Должно соответствовать одному из определений каталогов в [synchronizationSchema.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="d3b6f-144">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3b6f-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d3b6f-145">JSON representation</span></span>

<span data-ttu-id="d3b6f-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3b6f-146">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


