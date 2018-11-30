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
# <a name="attributemappingsource-resource-type"></a>Тип ресурса attributeMappingSource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта. Например может быть простой значение из заданного атрибута для объекта источника, или она может быть более сложного выражения string объединения и извлечения/замену на основе нескольких атрибутов источника. 

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Description               |
|:----------------------|:--------------------------|:--------------------------|
|выражение             |String                     |Представление эквивалентное выражение объекта **attributeMappingSource** .|
|name                   |String                     |Имя параметра источник сопоставления. В зависимости от значения свойства **типа** это может быть имя функции, имя исходного атрибута или постоянное значение для использования. |
|parameters             |[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) коллекции | Если этот объект представляет функцию, список параметров функции. Параметры состоят из объектов **attributeMappingSource** сами, позволяя для сложных выражений. Если **Тип** не `Function`, это свойство будет иметь значение null или пустой массив. |
|type                   | String                    |Тип сопоставления этого атрибута источника. Возможные значения: `Attribute`, `Constant`, `Function`. Значение по умолчанию: `Attribute`.| 

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

Простой атрибут для сопоставления

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

Выражение, извлечение первые восемь символов из исходного атрибута

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
