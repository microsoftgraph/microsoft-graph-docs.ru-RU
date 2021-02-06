---
title: Тип ресурса attributeMappingSource
description: Определяет, как значение должно быть извлечено (или преобразовано) из объекта-источника.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 50443eb85ed87bce466e7842f46d0c457f28e216
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133247"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="f46e6-103">Тип ресурса attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="f46e6-103">attributeMappingSource resource type</span></span>

<span data-ttu-id="f46e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f46e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f46e6-105">Определяет, как значение должно быть извлечено (или преобразовано) из объекта-источника.</span><span class="sxs-lookup"><span data-stu-id="f46e6-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="f46e6-106">Например, это может быть простое значение, взятное из заданного атрибута в объекте-источнике, или более сложное выражение конкатебирования, извлечения и замены строк на основе нескольких исходных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f46e6-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="f46e6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f46e6-107">Properties</span></span>

| <span data-ttu-id="f46e6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f46e6-108">Property</span></span>              | <span data-ttu-id="f46e6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f46e6-109">Type</span></span>                      | <span data-ttu-id="f46e6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f46e6-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="f46e6-111">выражение</span><span class="sxs-lookup"><span data-stu-id="f46e6-111">expression</span></span>             |<span data-ttu-id="f46e6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f46e6-112">String</span></span>                     |<span data-ttu-id="f46e6-113">Эквивалентное выражение, представление этого **объекта attributeMappingSource.**</span><span class="sxs-lookup"><span data-stu-id="f46e6-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="f46e6-114">name</span><span class="sxs-lookup"><span data-stu-id="f46e6-114">name</span></span>                   |<span data-ttu-id="f46e6-115">String</span><span class="sxs-lookup"><span data-stu-id="f46e6-115">String</span></span>                     |<span data-ttu-id="f46e6-116">Параметр name источника сопоставления.</span><span class="sxs-lookup"><span data-stu-id="f46e6-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="f46e6-117">В зависимости **от** значения свойства типа это может быть имя функции, имя атрибута источника или постоянное значение, которое необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="f46e6-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="f46e6-118">parameters</span><span class="sxs-lookup"><span data-stu-id="f46e6-118">parameters</span></span>             |<span data-ttu-id="f46e6-119">[Коллекция stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f46e6-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="f46e6-120">Если этот объект представляет функцию, перечисляет параметры функции.</span><span class="sxs-lookup"><span data-stu-id="f46e6-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="f46e6-121">Параметры состоят из **самих объектов attributeMappingSource,** что позволяет использовать сложные выражения.</span><span class="sxs-lookup"><span data-stu-id="f46e6-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="f46e6-122">Если **тип** не заданной, `Function` это свойство будет пустым или пустым массивом.</span><span class="sxs-lookup"><span data-stu-id="f46e6-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="f46e6-123">type</span><span class="sxs-lookup"><span data-stu-id="f46e6-123">type</span></span>                   | <span data-ttu-id="f46e6-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f46e6-124">String</span></span>                    |<span data-ttu-id="f46e6-125">Тип источника сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f46e6-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="f46e6-126">Возможные значения: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="f46e6-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="f46e6-127">Значение по умолчанию: `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="f46e6-127">Default is `Attribute`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f46e6-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f46e6-128">JSON representation</span></span>

<span data-ttu-id="f46e6-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f46e6-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="f46e6-130">Примеры JSON</span><span class="sxs-lookup"><span data-stu-id="f46e6-130">JSON Examples</span></span>

<span data-ttu-id="f46e6-131">Простое сопоставление атрибутов и атрибутов</span><span class="sxs-lookup"><span data-stu-id="f46e6-131">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="f46e6-132">Выражение, извлекающие первые 8 символов из атрибута источника</span><span class="sxs-lookup"><span data-stu-id="f46e6-132">Expression extracting first 8 characters from the source attribute</span></span>

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
  "suppressions": []
}
-->


