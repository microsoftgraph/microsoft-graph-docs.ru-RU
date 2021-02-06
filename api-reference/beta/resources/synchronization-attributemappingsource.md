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
# <a name="attributemappingsource-resource-type"></a>Тип ресурса attributeMappingSource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как значение должно быть извлечено (или преобразовано) из объекта-источника. Например, это может быть простое значение, взятное из заданного атрибута в объекте-источнике, или более сложное выражение конкатебирования, извлечения и замены строк на основе нескольких исходных атрибутов.

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание               |
|:----------------------|:--------------------------|:--------------------------|
|выражение             |Строка                     |Эквивалентное выражение, представление этого **объекта attributeMappingSource.**|
|name                   |String                     |Параметр name источника сопоставления. В зависимости **от** значения свойства типа это может быть имя функции, имя атрибута источника или постоянное значение, которое необходимо использовать. |
|parameters             |[Коллекция stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) | Если этот объект представляет функцию, перечисляет параметры функции. Параметры состоят из **самих объектов attributeMappingSource,** что позволяет использовать сложные выражения. Если **тип** не заданной, `Function` это свойство будет пустым или пустым массивом. |
|type                   | Строка                    |Тип источника сопоставления атрибутов. Возможные значения: `Attribute`, `Constant`, `Function`. Значение по умолчанию: `Attribute`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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

## <a name="json-examples"></a>Примеры JSON

Простое сопоставление атрибутов и атрибутов

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

Выражение, извлекающие первые 8 символов из атрибута источника

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


