---
title: Тип ресурса Аттрибутемаппингсаурце
description: 'Определяет способ извлечения (или преобразования) значения из исходного объекта. Например, это может быть простое значение из определенного атрибута для исходного объекта или более сложное выражение сцепления строк/извлечения/замены на основе нескольких исходных атрибутов. '
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 969f262f76f976c13f5c0a26ae53d67751b8820b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520235"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="6a5e3-104">Тип ресурса Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="6a5e3-104">attributeMappingSource resource type</span></span>

<span data-ttu-id="6a5e3-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6a5e3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a5e3-106">Определяет способ извлечения (или преобразования) значения из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-106">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="6a5e3-107">Например, это может быть простое значение из определенного атрибута для исходного объекта или более сложное выражение сцепления строк/извлечения/замены на основе нескольких исходных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-107">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="6a5e3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a5e3-108">Properties</span></span>

| <span data-ttu-id="6a5e3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a5e3-109">Property</span></span>              | <span data-ttu-id="6a5e3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6a5e3-110">Type</span></span>                      | <span data-ttu-id="6a5e3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a5e3-111">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="6a5e3-112">выражение</span><span class="sxs-lookup"><span data-stu-id="6a5e3-112">expression</span></span>             |<span data-ttu-id="6a5e3-113">String</span><span class="sxs-lookup"><span data-stu-id="6a5e3-113">String</span></span>                     |<span data-ttu-id="6a5e3-114">Эквивалентное представление этого объекта **аттрибутемаппингсаурце** в выражении.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-114">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="6a5e3-115">name</span><span class="sxs-lookup"><span data-stu-id="6a5e3-115">name</span></span>                   |<span data-ttu-id="6a5e3-116">String</span><span class="sxs-lookup"><span data-stu-id="6a5e3-116">String</span></span>                     |<span data-ttu-id="6a5e3-117">Параметр Name источника сопоставления.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-117">Name parameter of the mapping source.</span></span> <span data-ttu-id="6a5e3-118">В зависимости от значения свойства **Type** это может быть имя функции, имя исходного атрибута или значение константы, которое будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-118">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="6a5e3-119">parameters</span><span class="sxs-lookup"><span data-stu-id="6a5e3-119">parameters</span></span>             |<span data-ttu-id="6a5e3-120">Коллекция [стрингкэйаттрибутемаппингсаурцевалуепаир](synchronization-stringkeyattributemappingsourcevaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6a5e3-120">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="6a5e3-121">Если этот объект представляет функцию, перечисляет параметры функции.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-121">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="6a5e3-122">Параметры состоят из объектов **аттрибутемаппингсаурце** , что позволяет использовать сложные выражения.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-122">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="6a5e3-123">Если **тип** — Not `Function`, это свойство будет иметь значение null или пустой массив.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-123">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="6a5e3-124">type</span><span class="sxs-lookup"><span data-stu-id="6a5e3-124">type</span></span>                   | <span data-ttu-id="6a5e3-125">String</span><span class="sxs-lookup"><span data-stu-id="6a5e3-125">String</span></span>                    |<span data-ttu-id="6a5e3-126">Тип этого источника сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-126">The type of this attribute mapping source.</span></span> <span data-ttu-id="6a5e3-127">Возможные значения: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-127">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="6a5e3-128">Значение по умолчанию: `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-128">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="6a5e3-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a5e3-129">JSON representation</span></span>

<span data-ttu-id="6a5e3-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a5e3-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="6a5e3-131">Примеры JSON</span><span class="sxs-lookup"><span data-stu-id="6a5e3-131">JSON Examples</span></span>

<span data-ttu-id="6a5e3-132">Простой атрибут для сопоставления атрибутов</span><span class="sxs-lookup"><span data-stu-id="6a5e3-132">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="6a5e3-133">Выражение, извлекающее первые 8 символов из исходного атрибута</span><span class="sxs-lookup"><span data-stu-id="6a5e3-133">Expression extracting first 8 characters from the source attribute</span></span>

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
