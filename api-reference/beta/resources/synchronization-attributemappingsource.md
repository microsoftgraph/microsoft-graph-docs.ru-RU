---
title: Тип ресурса attributeMappingSource
description: 'Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта. Например может быть простой значение из заданного атрибута для объекта источника, или она может быть более сложного выражения string объединения и извлечения/замену на основе нескольких атрибутов источника. '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510409"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="b9587-104">Тип ресурса attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="b9587-104">attributeMappingSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9587-105">Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="b9587-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="b9587-106">Например может быть простой значение из заданного атрибута для объекта источника, или она может быть более сложного выражения string объединения и извлечения/замену на основе нескольких атрибутов источника.</span><span class="sxs-lookup"><span data-stu-id="b9587-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="b9587-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9587-107">Properties</span></span>

| <span data-ttu-id="b9587-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9587-108">Property</span></span>              | <span data-ttu-id="b9587-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9587-109">Type</span></span>                      | <span data-ttu-id="b9587-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9587-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="b9587-111">выражение</span><span class="sxs-lookup"><span data-stu-id="b9587-111">expression</span></span>             |<span data-ttu-id="b9587-112">String</span><span class="sxs-lookup"><span data-stu-id="b9587-112">String</span></span>                     |<span data-ttu-id="b9587-113">Представление эквивалентное выражение объекта **attributeMappingSource** .</span><span class="sxs-lookup"><span data-stu-id="b9587-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="b9587-114">name</span><span class="sxs-lookup"><span data-stu-id="b9587-114">name</span></span>                   |<span data-ttu-id="b9587-115">String</span><span class="sxs-lookup"><span data-stu-id="b9587-115">String</span></span>                     |<span data-ttu-id="b9587-116">Имя параметра источник сопоставления.</span><span class="sxs-lookup"><span data-stu-id="b9587-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="b9587-117">В зависимости от значения свойства **типа** это может быть имя функции, имя исходного атрибута или постоянное значение для использования.</span><span class="sxs-lookup"><span data-stu-id="b9587-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="b9587-118">parameters</span><span class="sxs-lookup"><span data-stu-id="b9587-118">parameters</span></span>             |<span data-ttu-id="b9587-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b9587-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="b9587-120">Если этот объект представляет функцию, список параметров функции.</span><span class="sxs-lookup"><span data-stu-id="b9587-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="b9587-121">Параметры состоят из объектов **attributeMappingSource** сами, позволяя для сложных выражений.</span><span class="sxs-lookup"><span data-stu-id="b9587-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="b9587-122">Если **Тип** не `Function`, это свойство будет иметь значение null или пустой массив.</span><span class="sxs-lookup"><span data-stu-id="b9587-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="b9587-123">type</span><span class="sxs-lookup"><span data-stu-id="b9587-123">type</span></span>                   | <span data-ttu-id="b9587-124">String</span><span class="sxs-lookup"><span data-stu-id="b9587-124">String</span></span>                    |<span data-ttu-id="b9587-125">Тип сопоставления этого атрибута источника.</span><span class="sxs-lookup"><span data-stu-id="b9587-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="b9587-126">Возможные значения: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="b9587-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="b9587-127">Значение по умолчанию: `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="b9587-127">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="b9587-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9587-128">JSON representation</span></span>

<span data-ttu-id="b9587-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9587-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}
```

## <a name="json-examples"></a><span data-ttu-id="b9587-130">Примеры JSON</span><span class="sxs-lookup"><span data-stu-id="b9587-130">JSON Examples</span></span>

<span data-ttu-id="b9587-131">Простой атрибут для сопоставления</span><span class="sxs-lookup"><span data-stu-id="b9587-131">Simple attribute to attribute mapping</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
    "expression": "[mail]",
    "name": "mail",
    "type": "Attribute"
}
```

<span data-ttu-id="b9587-132">Выражение, извлечение первые восемь символов из исходного атрибута</span><span class="sxs-lookup"><span data-stu-id="b9587-132">Expression extracting first 8 characters from the source attribute</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
 {
    "expression": "Mid([userPrincipalName], 1, 8)",
    "name": "Mid",
    "parameters": [
        {
            "key": "source",
            "value": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            }
        },
        {
            "key": "start",
            "value": {
                "expression": "\"1\"",
                "name": "1",
                "parameters": [],
                "type": "Constant"
            }
        },
        {
            "key": "length",
            "value": {
                "expression": "\"8\"",
                "name": "8",
                "parameters": [],
                "type": "Constant"
            }
        }
    ],
    "type": "Function"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingsource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
