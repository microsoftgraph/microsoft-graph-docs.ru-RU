---
title: Тип ресурса Синчронизатионруле
description: Определяет способ выполнения синхронизации для обработчика синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0698afb7e3584aa1d4cd6697504138f6262e5141
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217369"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="2d5cb-103">Тип ресурса Синчронизатионруле</span><span class="sxs-lookup"><span data-stu-id="2d5cb-103">synchronizationRule resource type</span></span>

<span data-ttu-id="2d5cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d5cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d5cb-105">Определяет способ выполнения синхронизации для обработчика синхронизации, в том числе объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге и как должны быть преобразованы атрибуты при их синхронизации из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-105">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="2d5cb-106">**Примечание:** Правила синхронизации определяют синхронизацию в одном направлении — из исходного каталога в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-106">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="2d5cb-107">Исходные и целевые каталоги определяются как часть свойств правила.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-107">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="2d5cb-108">Правила синхронизации обновляются в рамках [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2d5cb-108">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2d5cb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d5cb-109">Properties</span></span>

| <span data-ttu-id="2d5cb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d5cb-110">Property</span></span>      | <span data-ttu-id="2d5cb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2d5cb-111">Type</span></span>      | <span data-ttu-id="2d5cb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2d5cb-112">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="2d5cb-113">редактируем</span><span class="sxs-lookup"><span data-stu-id="2d5cb-113">editable</span></span>       |<span data-ttu-id="2d5cb-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d5cb-114">Boolean</span></span>    |<span data-ttu-id="2d5cb-115">`true`значение, если правило синхронизации может быть изменено; `false` если это правило доступно только для чтения и не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-115">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="2d5cb-116">id</span><span class="sxs-lookup"><span data-stu-id="2d5cb-116">id</span></span>             |<span data-ttu-id="2d5cb-117">Строка</span><span class="sxs-lookup"><span data-stu-id="2d5cb-117">String</span></span>     |<span data-ttu-id="2d5cb-118">Идентификатор правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-118">Synchronization rule identifier.</span></span> <span data-ttu-id="2d5cb-119">Допустимые значения: один из идентификаторов, распознаваемый обработчиком синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-119">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="2d5cb-120">Поддерживаемые идентификаторы правил можно найти в шаблоне синхронизации, возвращенном API.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-120">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="2d5cb-121">метаданных</span><span class="sxs-lookup"><span data-stu-id="2d5cb-121">metadata</span></span>       |<span data-ttu-id="2d5cb-122">Коллекция [стрингкэйстрингвалуепаир](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2d5cb-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="2d5cb-123">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-123">Additional extension properties.</span></span> <span data-ttu-id="2d5cb-124">Если вы не укажете в явной форме команду поддержки, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-124">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="2d5cb-125">name</span><span class="sxs-lookup"><span data-stu-id="2d5cb-125">name</span></span>           |<span data-ttu-id="2d5cb-126">String</span><span class="sxs-lookup"><span data-stu-id="2d5cb-126">String</span></span>     |<span data-ttu-id="2d5cb-127">Понятное имя правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-127">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="2d5cb-128">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-128">Not nullable.</span></span>|
|<span data-ttu-id="2d5cb-129">обжектмаппингс</span><span class="sxs-lookup"><span data-stu-id="2d5cb-129">objectMappings</span></span> |<span data-ttu-id="2d5cb-130">Коллекция [обжектмаппинг](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="2d5cb-130">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="2d5cb-131">Коллекция сопоставлений объектов, поддерживаемых правилом.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-131">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="2d5cb-132">Сообщает обработчику синхронизации, какие объекты должны синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-132">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="2d5cb-133">priority</span><span class="sxs-lookup"><span data-stu-id="2d5cb-133">priority</span></span>       |<span data-ttu-id="2d5cb-134">Целое число</span><span class="sxs-lookup"><span data-stu-id="2d5cb-134">Integer</span></span>    |<span data-ttu-id="2d5cb-135">Приоритет относительно других правил в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2d5cb-135">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="2d5cb-136">Правила с наименьшим номером приоритета будут обработаны первыми.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-136">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="2d5cb-137">саурцедиректоринаме</span><span class="sxs-lookup"><span data-stu-id="2d5cb-137">sourceDirectoryName</span></span>       |<span data-ttu-id="2d5cb-138">Строка</span><span class="sxs-lookup"><span data-stu-id="2d5cb-138">String</span></span>    |<span data-ttu-id="2d5cb-139">Имя исходного каталога.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-139">Name of the source directory.</span></span> <span data-ttu-id="2d5cb-140">Должно сопоставляться с одним из определений каталога в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2d5cb-140">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="2d5cb-141">таржетдиректоринаме</span><span class="sxs-lookup"><span data-stu-id="2d5cb-141">targetDirectoryName</span></span>       |<span data-ttu-id="2d5cb-142">Строка</span><span class="sxs-lookup"><span data-stu-id="2d5cb-142">String</span></span>    |<span data-ttu-id="2d5cb-143">Имя целевого каталога.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-143">Name of the target directory.</span></span> <span data-ttu-id="2d5cb-144">Должно сопоставляться с одним из определений каталога в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2d5cb-144">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d5cb-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d5cb-145">JSON representation</span></span>

<span data-ttu-id="2d5cb-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d5cb-146">The following is a JSON representation of the resource.</span></span>

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
