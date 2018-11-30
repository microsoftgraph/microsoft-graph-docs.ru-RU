---
title: Тип ресурса modifiedProperty
description: Указывает все измененные свойства с старое значение и новое значение для любого ресурса в Azure AD, необходимо изменить
ms.openlocfilehash: c504969ee12798969aa39490e79cb5b60bdb5435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077437"
---
# <a name="modifiedproperty-resource-type"></a>Тип ресурса modifiedProperty
Указывает все измененные свойства с старое значение и новое значение для любого ресурса в Azure AD, необходимо изменить



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Указывает имя свойства для целевой атрибут, который был изменен.|
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