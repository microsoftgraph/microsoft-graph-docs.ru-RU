---
title: Тип ресурса attributeMapping
description: Определяет, как значения для атрибута заданный целевой поток во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509324"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="ad7bf-103">Тип ресурса attributeMapping</span><span class="sxs-lookup"><span data-stu-id="ad7bf-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad7bf-104">Определяет, как значения для атрибута заданный целевой поток во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="ad7bf-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad7bf-105">Properties</span></span>

| <span data-ttu-id="ad7bf-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad7bf-106">Property</span></span>                  | <span data-ttu-id="ad7bf-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ad7bf-107">Type</span></span>                      | <span data-ttu-id="ad7bf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ad7bf-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="ad7bf-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="ad7bf-109">defaultValue</span></span>               | <span data-ttu-id="ad7bf-110">String</span><span class="sxs-lookup"><span data-stu-id="ad7bf-110">String</span></span>                    |<span data-ttu-id="ad7bf-111">По умолчанию значение для использования в случае, если свойство **source** проверялись `null`.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="ad7bf-112">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-112">Optional.</span></span>|
|<span data-ttu-id="ad7bf-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="ad7bf-113">exportMissingReferences</span></span>    |<span data-ttu-id="ad7bf-114">String</span><span class="sxs-lookup"><span data-stu-id="ad7bf-114">String</span></span>                     |<span data-ttu-id="ad7bf-115">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-115">For internal use only.</span></span>|
|<span data-ttu-id="ad7bf-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="ad7bf-116">flowBehavior</span></span>               |<span data-ttu-id="ad7bf-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="ad7bf-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="ad7bf-118">Определяет, когда этот атрибут, должны быть экспортированы в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="ad7bf-119">Возможные значения: `FlowWhenChanged` и `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="ad7bf-120">Значение по умолчанию: `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="ad7bf-121">flowType</span><span class="sxs-lookup"><span data-stu-id="ad7bf-121">flowType</span></span>                   |<span data-ttu-id="ad7bf-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="ad7bf-122">attributeFlowType</span></span>          |<span data-ttu-id="ad7bf-123">Определяет, когда этот атрибут следует обновить в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="ad7bf-124">Возможные значения: `Always` (по умолчанию), `ObjectAddOnly` (только если создается новый объект), `MultiValueAddOnly` (только при изменении добавляет новые значения это многозначный атрибут).</span><span class="sxs-lookup"><span data-stu-id="ad7bf-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="ad7bf-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="ad7bf-125">matchingPriority</span></span>           |<span data-ttu-id="ad7bf-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ad7bf-126">Int32</span></span>                      |<span data-ttu-id="ad7bf-127">Если больше 0, этот атрибут будет использоваться для выполнения первоначальной совпадение объектов между исходный и конечный каталоги.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="ad7bf-128">Обработчик синхронизации попытается найти соответствующий объект, с помощью атрибута с наименьшее значение сначала совпадающих приоритет.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="ad7bf-129">Если не найден, атрибута с помощью следующего соответствия приоритет будет использоваться и так далее до совпадения или исключаются соответствующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="ad7bf-130">Только атрибуты, которые должны иметь уникальные значения, такие как электронной почтой, следует использовать в качестве соответствующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="ad7bf-131">source</span><span class="sxs-lookup"><span data-stu-id="ad7bf-131">source</span></span>                     |[<span data-ttu-id="ad7bf-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="ad7bf-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="ad7bf-133">Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="ad7bf-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="ad7bf-134">targetAttributeName</span></span>        |<span data-ttu-id="ad7bf-135">String</span><span class="sxs-lookup"><span data-stu-id="ad7bf-135">String</span></span>                     |<span data-ttu-id="ad7bf-136">Имя атрибута для конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad7bf-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad7bf-137">JSON representation</span></span>

<span data-ttu-id="ad7bf-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad7bf-138">The following is a JSON representation of the resource.</span></span>

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
