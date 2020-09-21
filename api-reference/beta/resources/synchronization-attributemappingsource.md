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
# <a name="attributemappingsource-resource-type"></a>Тип ресурса Аттрибутемаппингсаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет способ извлечения (или преобразования) значения из исходного объекта. Например, это может быть простое значение из определенного атрибута для исходного объекта или более сложное выражение сцепления строк/извлечения/замены на основе нескольких исходных атрибутов.

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание               |
|:----------------------|:--------------------------|:--------------------------|
|выражение             |String                     |Эквивалентное представление этого объекта **аттрибутемаппингсаурце** в выражении.|
|name                   |String                     |Параметр Name источника сопоставления. В зависимости от значения свойства **Type** это может быть имя функции, имя исходного атрибута или значение константы, которое будет использоваться. |
|parameters             |Коллекция [стрингкэйаттрибутемаппингсаурцевалуепаир](synchronization-stringkeyattributemappingsourcevaluepair.md) | Если этот объект представляет функцию, перечисляет параметры функции. Параметры состоят из объектов **аттрибутемаппингсаурце** , что позволяет использовать сложные выражения. Если **тип** — Not `Function` , это свойство будет иметь значение null или пустой массив. |
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
  "suppressions": []
}
-->


