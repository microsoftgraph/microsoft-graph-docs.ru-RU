---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 211609f81bf2ff8123783660b50e1bdd06cb3d56
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808125"
---
# <a name="settingvalue-resource-type"></a>Тип ресурса settingValue

Пространство имен: microsoft.graph

Параметр, представленный в виде "имя-значение".

### <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|name|String| Имя параметра (как определено в [groupSettingTemplate](groupsettingtemplate.md)). |
|value|String| Значение параметра. |

### <a name="json-representation"></a>Представление в формате JSON

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
