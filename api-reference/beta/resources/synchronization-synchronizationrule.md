---
title: Тип ресурса Синчронизатионруле
description: Определяет способ выполнения синхронизации для обработчика синхронизации, в том числе объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге и как атрибуты должно быть преобразовано при синхронизации из источника с целевым каталогом.
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453646"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="0f804-103">Тип ресурса Синчронизатионруле</span><span class="sxs-lookup"><span data-stu-id="0f804-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f804-104">Определяет способ выполнения синхронизации для обработчика синхронизации, в том числе объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге и как атрибуты должно быть преобразовано при синхронизации из источника с целевым каталогом.</span><span class="sxs-lookup"><span data-stu-id="0f804-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="0f804-105">**Примечание:** Правила синхронизации определяют синхронизацию в одном направлении — из исходного каталога в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="0f804-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="0f804-106">Исходные и целевые каталоги определяются как часть свойств правила.</span><span class="sxs-lookup"><span data-stu-id="0f804-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="0f804-107">Правила синхронизации обновляются в рамках [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="0f804-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0f804-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f804-108">Properties</span></span>

| <span data-ttu-id="0f804-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f804-109">Property</span></span>      | <span data-ttu-id="0f804-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f804-110">Type</span></span>      | <span data-ttu-id="0f804-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f804-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="0f804-112">редактируем</span><span class="sxs-lookup"><span data-stu-id="0f804-112">editable</span></span>       |<span data-ttu-id="0f804-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f804-113">Boolean</span></span>    |<span data-ttu-id="0f804-114">`true`значение, если правило синхронизации может быть изменено; `false` если это правило доступно только для чтения и не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="0f804-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="0f804-115">id</span><span class="sxs-lookup"><span data-stu-id="0f804-115">id</span></span>             |<span data-ttu-id="0f804-116">Строка</span><span class="sxs-lookup"><span data-stu-id="0f804-116">String</span></span>     |<span data-ttu-id="0f804-117">Идентификатор правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0f804-117">Synchronization rule identifier.</span></span> <span data-ttu-id="0f804-118">Допустимые значения: один из идентификаторов, распознаваемый обработчиком синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0f804-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="0f804-119">Поддерживаемые идентификаторы правил можно найти в шаблоне синхронизации, возвращенном API.</span><span class="sxs-lookup"><span data-stu-id="0f804-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="0f804-120">метаданных</span><span class="sxs-lookup"><span data-stu-id="0f804-120">metadata</span></span>       |<span data-ttu-id="0f804-121">Коллекция [стрингкэйстрингвалуепаир](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0f804-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="0f804-122">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="0f804-122">Additional extension properties.</span></span> <span data-ttu-id="0f804-123">Если вы не укажете в явной форме команду поддержки, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="0f804-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="0f804-124">name</span><span class="sxs-lookup"><span data-stu-id="0f804-124">name</span></span>           |<span data-ttu-id="0f804-125">String</span><span class="sxs-lookup"><span data-stu-id="0f804-125">String</span></span>     |<span data-ttu-id="0f804-126">Понятное имя правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0f804-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="0f804-127">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0f804-127">Not nullable.</span></span>|
|<span data-ttu-id="0f804-128">Обжектмаппингс</span><span class="sxs-lookup"><span data-stu-id="0f804-128">objectMappings</span></span> |<span data-ttu-id="0f804-129">Коллекция [обжектмаппинг](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="0f804-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="0f804-130">Коллекция сопоставлений объектов, поддерживаемых правилом.</span><span class="sxs-lookup"><span data-stu-id="0f804-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="0f804-131">Сообщает обработчику синхронизации, какие объекты должны синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="0f804-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="0f804-132">priority</span><span class="sxs-lookup"><span data-stu-id="0f804-132">priority</span></span>       |<span data-ttu-id="0f804-133">Целое число</span><span class="sxs-lookup"><span data-stu-id="0f804-133">Integer</span></span>    |<span data-ttu-id="0f804-134">Приоритет относительно других правил в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="0f804-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="0f804-135">Правила с наименьшим номером приоритета будут обработаны первыми.</span><span class="sxs-lookup"><span data-stu-id="0f804-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="0f804-136">Саурцедиректоринаме</span><span class="sxs-lookup"><span data-stu-id="0f804-136">sourceDirectoryName</span></span>       |<span data-ttu-id="0f804-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0f804-137">String</span></span>    |<span data-ttu-id="0f804-138">Имя исходного каталога.</span><span class="sxs-lookup"><span data-stu-id="0f804-138">Name of the source directory.</span></span> <span data-ttu-id="0f804-139">Должно сопоставляться с одним из определений каталога в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="0f804-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="0f804-140">Таржетдиректоринаме</span><span class="sxs-lookup"><span data-stu-id="0f804-140">targetDirectoryName</span></span>       |<span data-ttu-id="0f804-141">Строка</span><span class="sxs-lookup"><span data-stu-id="0f804-141">String</span></span>    |<span data-ttu-id="0f804-142">Имя целевого каталога.</span><span class="sxs-lookup"><span data-stu-id="0f804-142">Name of the target directory.</span></span> <span data-ttu-id="0f804-143">Должно сопоставляться с одним из определений каталога в [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="0f804-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f804-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f804-144">JSON representation</span></span>

<span data-ttu-id="0f804-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f804-145">The following is a JSON representation of the resource.</span></span>

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
