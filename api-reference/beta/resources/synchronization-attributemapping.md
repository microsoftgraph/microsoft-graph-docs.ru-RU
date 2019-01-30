---
title: Тип ресурса attributeMapping
description: Определяет, как значения для атрибута заданный целевой поток во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641878"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="79aa6-103">Тип ресурса attributeMapping</span><span class="sxs-lookup"><span data-stu-id="79aa6-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79aa6-104">Определяет, как значения для атрибута заданный целевой поток во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="79aa6-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="79aa6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="79aa6-105">Properties</span></span>

| <span data-ttu-id="79aa6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="79aa6-106">Property</span></span>                  | <span data-ttu-id="79aa6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="79aa6-107">Type</span></span>                      | <span data-ttu-id="79aa6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="79aa6-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="79aa6-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="79aa6-109">defaultValue</span></span>               | <span data-ttu-id="79aa6-110">String</span><span class="sxs-lookup"><span data-stu-id="79aa6-110">String</span></span>                    |<span data-ttu-id="79aa6-111">По умолчанию значение для использования в случае, если свойство **source** проверялись `null`.</span><span class="sxs-lookup"><span data-stu-id="79aa6-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="79aa6-112">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="79aa6-112">Optional.</span></span>|
|<span data-ttu-id="79aa6-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="79aa6-113">exportMissingReferences</span></span>    |<span data-ttu-id="79aa6-114">String</span><span class="sxs-lookup"><span data-stu-id="79aa6-114">String</span></span>                     |<span data-ttu-id="79aa6-115">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="79aa6-115">For internal use only.</span></span>|
|<span data-ttu-id="79aa6-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="79aa6-116">flowBehavior</span></span>               |<span data-ttu-id="79aa6-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="79aa6-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="79aa6-118">Определяет, когда этот атрибут, должны быть экспортированы в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="79aa6-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="79aa6-119">Возможные значения: `FlowWhenChanged` и `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="79aa6-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="79aa6-120">Значение по умолчанию: `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="79aa6-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="79aa6-121">flowType</span><span class="sxs-lookup"><span data-stu-id="79aa6-121">flowType</span></span>                   |<span data-ttu-id="79aa6-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="79aa6-122">attributeFlowType</span></span>          |<span data-ttu-id="79aa6-123">Определяет, когда этот атрибут следует обновить в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="79aa6-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="79aa6-124">Возможные значения: `Always` (по умолчанию), `ObjectAddOnly` (только если создается новый объект), `MultiValueAddOnly` (только при изменении добавляет новые значения это многозначный атрибут).</span><span class="sxs-lookup"><span data-stu-id="79aa6-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="79aa6-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="79aa6-125">matchingPriority</span></span>           |<span data-ttu-id="79aa6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="79aa6-126">Int32</span></span>                      |<span data-ttu-id="79aa6-127">Если больше 0, этот атрибут будет использоваться для выполнения первоначальной совпадение объектов между исходный и конечный каталоги.</span><span class="sxs-lookup"><span data-stu-id="79aa6-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="79aa6-128">Обработчик синхронизации попытается найти соответствующий объект, с помощью атрибута с наименьшее значение сначала совпадающих приоритет.</span><span class="sxs-lookup"><span data-stu-id="79aa6-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="79aa6-129">Если не найден, атрибута с помощью следующего соответствия приоритет будет использоваться и так далее до совпадения или исключаются соответствующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="79aa6-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="79aa6-130">Только атрибуты, которые должны иметь уникальные значения, такие как электронной почтой, следует использовать в качестве соответствующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="79aa6-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="79aa6-131">source</span><span class="sxs-lookup"><span data-stu-id="79aa6-131">source</span></span>                     |[<span data-ttu-id="79aa6-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="79aa6-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="79aa6-133">Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="79aa6-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="79aa6-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="79aa6-134">targetAttributeName</span></span>        |<span data-ttu-id="79aa6-135">String</span><span class="sxs-lookup"><span data-stu-id="79aa6-135">String</span></span>                     |<span data-ttu-id="79aa6-136">Имя атрибута для конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="79aa6-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="79aa6-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79aa6-137">JSON representation</span></span>

<span data-ttu-id="79aa6-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79aa6-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
