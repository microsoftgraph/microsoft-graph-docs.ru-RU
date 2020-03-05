---
title: Тип ресурса Синчронизатионруле
description: Определяет способ выполнения синхронизации для обработчика синхронизации, в том числе объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге и как атрибуты должно быть преобразовано при синхронизации из источника с целевым каталогом.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b1d8afd1f87527a5a92755ff45ec876c8d66d9c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520053"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="83f16-103">Тип ресурса Синчронизатионруле</span><span class="sxs-lookup"><span data-stu-id="83f16-103">synchronizationRule resource type</span></span>

<span data-ttu-id="83f16-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="83f16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83f16-105">Определяет способ выполнения синхронизации для обработчика синхронизации, в том числе объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге и как атрибуты должно быть преобразовано при синхронизации из источника с целевым каталогом.</span><span class="sxs-lookup"><span data-stu-id="83f16-105">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="83f16-106">**Примечание:** Правила синхронизации определяют синхронизацию в одном направлении — из исходного каталога в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="83f16-106">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="83f16-107">Исходные и целевые каталоги определяются как часть свойств правила.</span><span class="sxs-lookup"><span data-stu-id="83f16-107">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="83f16-108">Правила синхронизации обновляются в рамках [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83f16-108">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="83f16-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="83f16-109">Properties</span></span>

| <span data-ttu-id="83f16-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="83f16-110">Property</span></span>      | <span data-ttu-id="83f16-111">Тип</span><span class="sxs-lookup"><span data-stu-id="83f16-111">Type</span></span>      | <span data-ttu-id="83f16-112">Описание</span><span class="sxs-lookup"><span data-stu-id="83f16-112">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="83f16-113">редактируем</span><span class="sxs-lookup"><span data-stu-id="83f16-113">editable</span></span>       |<span data-ttu-id="83f16-114">Логический</span><span class="sxs-lookup"><span data-stu-id="83f16-114">Boolean</span></span>    |<span data-ttu-id="83f16-115">`true`значение, если правило синхронизации может быть изменено; `false` если это правило доступно только для чтения и не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="83f16-115">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="83f16-116">id</span><span class="sxs-lookup"><span data-stu-id="83f16-116">id</span></span>             |<span data-ttu-id="83f16-117">Строка</span><span class="sxs-lookup"><span data-stu-id="83f16-117">String</span></span>     |<span data-ttu-id="83f16-118">Идентификатор правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="83f16-118">Synchronization rule identifier.</span></span> <span data-ttu-id="83f16-119">Допустимые значения: один из идентификаторов, распознаваемый обработчиком синхронизации.</span><span class="sxs-lookup"><span data-stu-id="83f16-119">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="83f16-120">Поддерживаемые идентификаторы правил можно найти в шаблоне синхронизации, возвращенном API.</span><span class="sxs-lookup"><span data-stu-id="83f16-120">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="83f16-121">метаданных</span><span class="sxs-lookup"><span data-stu-id="83f16-121">metadata</span></span>       |<span data-ttu-id="83f16-122">Коллекция [стрингкэйстрингвалуепаир](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="83f16-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="83f16-123">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="83f16-123">Additional extension properties.</span></span> <span data-ttu-id="83f16-124">Если вы не укажете в явной форме команду поддержки, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="83f16-124">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="83f16-125">name</span><span class="sxs-lookup"><span data-stu-id="83f16-125">name</span></span>           |<span data-ttu-id="83f16-126">String</span><span class="sxs-lookup"><span data-stu-id="83f16-126">String</span></span>     |<span data-ttu-id="83f16-127">Понятное имя правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="83f16-127">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="83f16-128">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="83f16-128">Not nullable.</span></span>|
|<span data-ttu-id="83f16-129">обжектмаппингс</span><span class="sxs-lookup"><span data-stu-id="83f16-129">objectMappings</span></span> |<span data-ttu-id="83f16-130">Коллекция [обжектмаппинг](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="83f16-130">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="83f16-131">Коллекция сопоставлений объектов, поддерживаемых правилом.</span><span class="sxs-lookup"><span data-stu-id="83f16-131">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="83f16-132">Сообщает обработчику синхронизации, какие объекты должны синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="83f16-132">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="83f16-133">priority</span><span class="sxs-lookup"><span data-stu-id="83f16-133">priority</span></span>       |<span data-ttu-id="83f16-134">Целое число</span><span class="sxs-lookup"><span data-stu-id="83f16-134">Integer</span></span>    |<span data-ttu-id="83f16-135">Приоритет относительно других правил в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83f16-135">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="83f16-136">Правила с наименьшим номером приоритета будут обработаны первыми.</span><span class="sxs-lookup"><span data-stu-id="83f16-136">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="83f16-137">саурцедиректоринаме</span><span class="sxs-lookup"><span data-stu-id="83f16-137">sourceDirectoryName</span></span>       |<span data-ttu-id="83f16-138">String</span><span class="sxs-lookup"><span data-stu-id="83f16-138">String</span></span>    |<span data-ttu-id="83f16-139">Имя исходного каталога.</span><span class="sxs-lookup"><span data-stu-id="83f16-139">Name of the source directory.</span></span> <span data-ttu-id="83f16-140">Должно сопоставляться с одним из определений каталога в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83f16-140">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="83f16-141">таржетдиректоринаме</span><span class="sxs-lookup"><span data-stu-id="83f16-141">targetDirectoryName</span></span>       |<span data-ttu-id="83f16-142">String</span><span class="sxs-lookup"><span data-stu-id="83f16-142">String</span></span>    |<span data-ttu-id="83f16-143">Имя целевого каталога.</span><span class="sxs-lookup"><span data-stu-id="83f16-143">Name of the target directory.</span></span> <span data-ttu-id="83f16-144">Должно сопоставляться с одним из определений каталога в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83f16-144">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83f16-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83f16-145">JSON representation</span></span>

<span data-ttu-id="83f16-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83f16-146">The following is a JSON representation of the resource.</span></span>

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
