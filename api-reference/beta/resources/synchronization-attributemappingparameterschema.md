---
title: Тип ресурса attributeMappingParameterSchema
description: Описывает один параметр, используемый в attributeMappingFunctionSchema.
ms.openlocfilehash: 164387a345f245f390d24b89a349e02ee2242041
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081506"
---
# <a name="attributemappingparameterschema-resource-type"></a>Тип ресурса attributeMappingParameterSchema

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает один параметр, используемый в [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Description    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Логический                   |Данному параметру можно указать несколько раз (например нескольких входных данных строки в `Concatenate(string,string,...)` функция). |
|name                        |String                    |Имя параметра. |
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