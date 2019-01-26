---
title: Тип ресурса attributeMapping
description: Определяет, как значения для атрибута заданный целевой поток во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 9f33aa9a784ba3e40fd8d38650737a9064a0831c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573664"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="f3101-103">Тип ресурса attributeMapping</span><span class="sxs-lookup"><span data-stu-id="f3101-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3101-104">Определяет, как значения для атрибута заданный целевой поток во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f3101-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="f3101-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3101-105">Properties</span></span>

| <span data-ttu-id="f3101-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3101-106">Property</span></span>                  | <span data-ttu-id="f3101-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f3101-107">Type</span></span>                      | <span data-ttu-id="f3101-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f3101-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="f3101-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="f3101-109">defaultValue</span></span>               | <span data-ttu-id="f3101-110">String</span><span class="sxs-lookup"><span data-stu-id="f3101-110">String</span></span>                    |<span data-ttu-id="f3101-111">По умолчанию значение для использования в случае, если свойство **source** проверялись `null`.</span><span class="sxs-lookup"><span data-stu-id="f3101-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="f3101-112">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f3101-112">Optional.</span></span>|
|<span data-ttu-id="f3101-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="f3101-113">exportMissingReferences</span></span>    |<span data-ttu-id="f3101-114">Строка</span><span class="sxs-lookup"><span data-stu-id="f3101-114">String</span></span>                     |<span data-ttu-id="f3101-115">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="f3101-115">For internal use only.</span></span>|
|<span data-ttu-id="f3101-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="f3101-116">flowBehavior</span></span>               | <span data-ttu-id="f3101-117">Строка перечисления</span><span class="sxs-lookup"><span data-stu-id="f3101-117">enum-string</span></span>      |<span data-ttu-id="f3101-118">Определяет, когда этот атрибут, должны быть экспортированы в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="f3101-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="f3101-119">Возможные значения: `FlowWhenChanged` и `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="f3101-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="f3101-120">Значение по умолчанию: `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="f3101-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="f3101-121">flowType</span><span class="sxs-lookup"><span data-stu-id="f3101-121">flowType</span></span>                   | <span data-ttu-id="f3101-122">Строка ennum</span><span class="sxs-lookup"><span data-stu-id="f3101-122">ennum-string</span></span>          |<span data-ttu-id="f3101-123">Определяет, когда этот атрибут следует обновить в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="f3101-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="f3101-124">Возможные значения: `Always` (по умолчанию), `ObjectAddOnly` (только если создается новый объект), `MultiValueAddOnly` (только при изменении добавляет новые значения это многозначный атрибут).</span><span class="sxs-lookup"><span data-stu-id="f3101-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="f3101-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="f3101-125">matchingPriority</span></span>           |<span data-ttu-id="f3101-126">Int32</span><span class="sxs-lookup"><span data-stu-id="f3101-126">Int32</span></span>                      |<span data-ttu-id="f3101-127">Если больше 0, этот атрибут будет использоваться для выполнения первоначальной совпадение объектов между исходный и конечный каталоги.</span><span class="sxs-lookup"><span data-stu-id="f3101-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="f3101-128">Обработчик синхронизации попытается найти соответствующий объект, с помощью атрибута с наименьшее значение сначала совпадающих приоритет.</span><span class="sxs-lookup"><span data-stu-id="f3101-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="f3101-129">Если не найден, атрибута с помощью следующего соответствия приоритет будет использоваться и так далее до совпадения или исключаются соответствующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="f3101-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="f3101-130">Только атрибуты, которые должны иметь уникальные значения, такие как электронной почтой, следует использовать в качестве соответствующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="f3101-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="f3101-131">source</span><span class="sxs-lookup"><span data-stu-id="f3101-131">source</span></span>                     |[<span data-ttu-id="f3101-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="f3101-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="f3101-133">Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="f3101-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="f3101-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="f3101-134">targetAttributeName</span></span>        |<span data-ttu-id="f3101-135">Строка</span><span class="sxs-lookup"><span data-stu-id="f3101-135">String</span></span>                     |<span data-ttu-id="f3101-136">Имя атрибута для конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="f3101-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f3101-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3101-137">JSON representation</span></span>

<span data-ttu-id="f3101-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3101-138">The following is a JSON representation of the resource.</span></span>

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
  "flowBehavior": "FlowWhenChanged | FlowAlways",
  "flowType": "Always |  ObjectAddOnly | MultiValueAddOnly ",
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
