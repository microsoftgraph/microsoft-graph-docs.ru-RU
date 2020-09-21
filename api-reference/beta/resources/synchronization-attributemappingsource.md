---
title: Тип ресурса Аттрибутемаппингсаурце
description: Определяет способ извлечения (или преобразования) значения из исходного объекта.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8e290ae6a31b927acce27a691fad39bf00a00985
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078054"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="f98ed-103">Тип ресурса Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="f98ed-103">attributeMappingSource resource type</span></span>

<span data-ttu-id="f98ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f98ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f98ed-105">Определяет способ извлечения (или преобразования) значения из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="f98ed-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="f98ed-106">Например, это может быть простое значение из определенного атрибута для исходного объекта или более сложное выражение сцепления строк/извлечения/замены на основе нескольких исходных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f98ed-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="f98ed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f98ed-107">Properties</span></span>

| <span data-ttu-id="f98ed-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f98ed-108">Property</span></span>              | <span data-ttu-id="f98ed-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f98ed-109">Type</span></span>                      | <span data-ttu-id="f98ed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f98ed-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="f98ed-111">выражение</span><span class="sxs-lookup"><span data-stu-id="f98ed-111">expression</span></span>             |<span data-ttu-id="f98ed-112">String</span><span class="sxs-lookup"><span data-stu-id="f98ed-112">String</span></span>                     |<span data-ttu-id="f98ed-113">Эквивалентное представление этого объекта **аттрибутемаппингсаурце** в выражении.</span><span class="sxs-lookup"><span data-stu-id="f98ed-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="f98ed-114">name</span><span class="sxs-lookup"><span data-stu-id="f98ed-114">name</span></span>                   |<span data-ttu-id="f98ed-115">String</span><span class="sxs-lookup"><span data-stu-id="f98ed-115">String</span></span>                     |<span data-ttu-id="f98ed-116">Параметр Name источника сопоставления.</span><span class="sxs-lookup"><span data-stu-id="f98ed-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="f98ed-117">В зависимости от значения свойства **Type** это может быть имя функции, имя исходного атрибута или значение константы, которое будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="f98ed-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="f98ed-118">parameters</span><span class="sxs-lookup"><span data-stu-id="f98ed-118">parameters</span></span>             |<span data-ttu-id="f98ed-119">Коллекция [стрингкэйаттрибутемаппингсаурцевалуепаир](synchronization-stringkeyattributemappingsourcevaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f98ed-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="f98ed-120">Если этот объект представляет функцию, перечисляет параметры функции.</span><span class="sxs-lookup"><span data-stu-id="f98ed-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="f98ed-121">Параметры состоят из объектов **аттрибутемаппингсаурце** , что позволяет использовать сложные выражения.</span><span class="sxs-lookup"><span data-stu-id="f98ed-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="f98ed-122">Если **тип** — Not `Function` , это свойство будет иметь значение null или пустой массив.</span><span class="sxs-lookup"><span data-stu-id="f98ed-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="f98ed-123">type</span><span class="sxs-lookup"><span data-stu-id="f98ed-123">type</span></span>                   | <span data-ttu-id="f98ed-124">String</span><span class="sxs-lookup"><span data-stu-id="f98ed-124">String</span></span>                    |<span data-ttu-id="f98ed-125">Тип этого источника сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f98ed-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="f98ed-126">Возможные значения: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="f98ed-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="f98ed-127">Значение по умолчанию: `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="f98ed-127">Default is `Attribute`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f98ed-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f98ed-128">JSON representation</span></span>

<span data-ttu-id="f98ed-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f98ed-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="f98ed-130">Примеры JSON</span><span class="sxs-lookup"><span data-stu-id="f98ed-130">JSON Examples</span></span>

<span data-ttu-id="f98ed-131">Простой атрибут для сопоставления атрибутов</span><span class="sxs-lookup"><span data-stu-id="f98ed-131">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="f98ed-132">Выражение, извлекающее первые 8 символов из исходного атрибута</span><span class="sxs-lookup"><span data-stu-id="f98ed-132">Expression extracting first 8 characters from the source attribute</span></span>

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


