---
title: Тип ресурса attributeMappingParameterSchema
description: Описывает один параметр, используемый в attributeMappingFunctionSchema.
localization_priority: Normal
ms.openlocfilehash: 083f89ebc5a74e6fd58a33925b2bfa46801b7961
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892171"
---
# <a name="attributemappingparameterschema-resource-type"></a>Тип ресурса attributeMappingParameterSchema

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает один параметр, используемый в [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Логический                   |Данному параметру можно указать несколько раз (например нескольких входных данных строки в `Concatenate(string,string,...)` функция). |
|name                        |Строка                    |Имя параметра. |
|Обязательный                    |Логический                   |`true`Если параметр является обязательным; в противном случае `false`. |
|type                        |String                    |Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`. Значение по умолчанию: `String`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
