---
title: Тип ресурса Аттрибутемаппингсаурце
description: 'Определяет способ извлечения (или преобразования) значения из исходного объекта. Например, это может быть простое значение из определенного атрибута для исходного объекта или более сложное выражение сцепления строк/извлечения/замены на основе нескольких исходных атрибутов. '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582182"
---
# <a name="attributemappingsource-resource-type"></a>Тип ресурса Аттрибутемаппингсаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет способ извлечения (или преобразования) значения из исходного объекта. Например, это может быть простое значение из определенного атрибута для исходного объекта или более сложное выражение сцепления строк/извлечения/замены на основе нескольких исходных атрибутов. 

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание               |
|:----------------------|:--------------------------|:--------------------------|
|выражение             |String                     |Эквивалентное представление этого объекта **аттрибутемаппингсаурце** в выражении.|
|name                   |String                     |Параметр Name источника сопоставления. В зависимости от значения свойства **Type** это может быть имя функции, имя исходного атрибута или значение константы, которое будет использоваться. |
|parameters             |Коллекция [стрингкэйаттрибутемаппингсаурцевалуепаир](synchronization-stringkeyattributemappingsourcevaluepair.md) | Если этот объект представляет функцию, перечисляет параметры функции. Параметры состоят из объектов **аттрибутемаппингсаурце** , что позволяет использовать сложные выражения. Если **тип** — Not `Function`, это свойство будет иметь значение null или пустой массив. |
|type                   | String                    |Тип этого источника сопоставления атрибутов. Возможные значения: `Attribute`, `Constant`, `Function`. Значение по умолчанию: `Attribute`.| 

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

Простой атрибут для сопоставления атрибутов

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

Выражение, извлекающее первые 8 символов из исходного атрибута

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
