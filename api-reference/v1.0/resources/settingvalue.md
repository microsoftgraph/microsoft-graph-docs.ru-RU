---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4f565f598db7e69a48a924279a3ed228f2651755
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009220"
---
# <a name="settingvalue-resource-type"></a>Тип ресурса settingValue

Пространство имен: microsoft.graph

Параметр, представленный в виде "имя-значение".

### <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|name|String| Имя параметра (как определено в [groupSettingTemplate](groupsettingtemplate.md)). |
|value|String| Значение параметра. |

### <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

