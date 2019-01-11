---
title: Тип ресурса settingValue
description: Параметр, представленный парой "имя-значение".
localization_priority: Normal
ms.openlocfilehash: 3edf5bdc1fae77702206eae78d53fcf0fdc5b644
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834036"
---
# <a name="settingvalue-resource-type"></a>Тип ресурса settingValue

Параметр, представленный парой "имя-значение".

### <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|name|String| Имя параметра, определенное [groupSettingTemplate](groupsettingtemplate.md). |
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
