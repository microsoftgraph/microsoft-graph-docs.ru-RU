---
title: тип ресурса modifiedProperty
description: Указывает все свойства измененного ресурса Azure AD, включая старые и новые значения.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4c74e492b50435b7911952ffe32107008db11330
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067075"
---
# <a name="modifiedproperty-resource-type"></a>тип ресурса modifiedProperty

Пространство имен: microsoft.graph

Указывает все свойства измененного ресурса Azure AD, включая старые и новые значения.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Указывает имя свойства измененного целевого атрибута.|
|newValue|String|Указывает обновленное значение для правильности.|
|oldValue|String|Указывает предыдущее значение (перед обновлением) для свойства.|

## <a name="json-representation"></a>Представление в формате JSON

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

