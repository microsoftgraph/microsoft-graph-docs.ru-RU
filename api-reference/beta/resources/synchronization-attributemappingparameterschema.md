---
title: Тип ресурса Аттрибутемаппингпараметерсчема
description: Описывает один параметр, используемый в Аттрибутемаппингфунктионсчема.
localization_priority: Normal
ms.openlocfilehash: 44234e7e76b5b0d0fb514366be6106c8177b56db
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342957"
---
# <a name="attributemappingparameterschema-resource-type"></a>Тип ресурса Аттрибутемаппингпараметерсчема

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает один параметр, используемый в [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:-------------------------|:---------------|
|Алловмултиплеоккурренцес    |Логический                   |Данный параметр может быть указан несколько раз (например, с несколькими входными строками в `Concatenate(string,string,...)` функции). |
|name                        |String                    |Имя параметра. |
|Обязательный                    |Логический                   |`true`значение, если параметр является обязательным; в `false`противном случае. |
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
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
