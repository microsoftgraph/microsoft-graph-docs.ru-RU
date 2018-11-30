---
title: Тип ресурса attributeMappingSource
description: 'Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта. Например может быть простой значение из заданного атрибута для объекта источника, или она может быть более сложного выражения string объединения и извлечения/замену на основе нескольких атрибутов источника. '
ms.openlocfilehash: aeb39c829d7be081fe9ee08aa5845e6ced1194dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078159"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="9252e-104">Тип ресурса attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="9252e-104">attributeMappingSource resource type</span></span>

> <span data-ttu-id="9252e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9252e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9252e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9252e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9252e-107">Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="9252e-107">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="9252e-108">Например может быть простой значение из заданного атрибута для объекта источника, или она может быть более сложного выражения string объединения и извлечения/замену на основе нескольких атрибутов источника.</span><span class="sxs-lookup"><span data-stu-id="9252e-108">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="9252e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9252e-109">Properties</span></span>

| <span data-ttu-id="9252e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9252e-110">Property</span></span>              | <span data-ttu-id="9252e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9252e-111">Type</span></span>                      | <span data-ttu-id="9252e-112">Description</span><span class="sxs-lookup"><span data-stu-id="9252e-112">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="9252e-113">выражение</span><span class="sxs-lookup"><span data-stu-id="9252e-113">expression</span></span>             |<span data-ttu-id="9252e-114">String</span><span class="sxs-lookup"><span data-stu-id="9252e-114">String</span></span>                     |<span data-ttu-id="9252e-115">Представление эквивалентное выражение объекта **attributeMappingSource** .</span><span class="sxs-lookup"><span data-stu-id="9252e-115">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="9252e-116">name</span><span class="sxs-lookup"><span data-stu-id="9252e-116">name</span></span>                   |<span data-ttu-id="9252e-117">String</span><span class="sxs-lookup"><span data-stu-id="9252e-117">String</span></span>                     |<span data-ttu-id="9252e-118">Имя параметра источник сопоставления.</span><span class="sxs-lookup"><span data-stu-id="9252e-118">Name parameter of the mapping source.</span></span> <span data-ttu-id="9252e-119">В зависимости от значения свойства **типа** это может быть имя функции, имя исходного атрибута или постоянное значение для использования.</span><span class="sxs-lookup"><span data-stu-id="9252e-119">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="9252e-120">parameters</span><span class="sxs-lookup"><span data-stu-id="9252e-120">parameters</span></span>             |<span data-ttu-id="9252e-121">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9252e-121">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="9252e-122">Если этот объект представляет функцию, список параметров функции.</span><span class="sxs-lookup"><span data-stu-id="9252e-122">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="9252e-123">Параметры состоят из объектов **attributeMappingSource** сами, позволяя для сложных выражений.</span><span class="sxs-lookup"><span data-stu-id="9252e-123">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="9252e-124">Если **Тип** не `Function`, это свойство будет иметь значение null или пустой массив.</span><span class="sxs-lookup"><span data-stu-id="9252e-124">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="9252e-125">type</span><span class="sxs-lookup"><span data-stu-id="9252e-125">type</span></span>                   | <span data-ttu-id="9252e-126">String</span><span class="sxs-lookup"><span data-stu-id="9252e-126">String</span></span>                    |<span data-ttu-id="9252e-127">Тип сопоставления этого атрибута источника.</span><span class="sxs-lookup"><span data-stu-id="9252e-127">The type of this attribute mapping source.</span></span> <span data-ttu-id="9252e-128">Возможные значения: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="9252e-128">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="9252e-129">Значение по умолчанию: `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="9252e-129">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="9252e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9252e-130">JSON representation</span></span>

<span data-ttu-id="9252e-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9252e-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="9252e-132">Примеры JSON</span><span class="sxs-lookup"><span data-stu-id="9252e-132">JSON Examples</span></span>

<span data-ttu-id="9252e-133">Простой атрибут для сопоставления</span><span class="sxs-lookup"><span data-stu-id="9252e-133">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="9252e-134">Выражение, извлечение первые восемь символов из исходного атрибута</span><span class="sxs-lookup"><span data-stu-id="9252e-134">Expression extracting first 8 characters from the source attribute</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
