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
# <a name="attributemappingsource-resource-type"></a>Тип ресурса attributeMappingSource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта. Например может быть простой значение из заданного атрибута для объекта источника, или она может быть более сложного выражения string объединения и извлечения/замену на основе нескольких атрибутов источника. 

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание               |
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
