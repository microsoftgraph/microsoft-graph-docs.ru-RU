---
title: Тип ресурса modifiedProperty
description: Указывает все измененные свойства с старое значение и новое значение для любого ресурса в Azure AD, необходимо изменить
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844458"
---
# <a name="modifiedproperty-resource-type"></a>Тип ресурса modifiedProperty
Указывает все измененные свойства с старое значение и новое значение для любого ресурса в Azure AD, необходимо изменить



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Указывает имя свойства для целевой атрибут, который был изменен.|
|newValue|String|Указывает обновленное значение для свойство.|
|oldValue|String|Указывает предыдущее (до обновления) для свойства.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
