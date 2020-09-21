---
title: Тип ресурса Аттрибутемаппингпараметерсчема
description: Описывает один параметр, используемый в Аттрибутемаппингфунктионсчема.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32710c5411f054ad096bdd293a2f7d46e89a6944
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078086"
---
# <a name="attributemappingparameterschema-resource-type"></a>Тип ресурса Аттрибутемаппингпараметерсчема

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает один параметр, используемый в [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:-------------------------|:---------------|
|алловмултиплеоккурренцес    |Boolean                   |Данный параметр может быть указан несколько раз (например, с несколькими входными строками в `Concatenate(string,string,...)` функции). |
|name                        |String                    |Имя параметра. |
|Обязательный                    |Boolean                   |`true` значение, если параметр является обязательным; в противном случае `false` . |
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


