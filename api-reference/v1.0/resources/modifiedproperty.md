---
title: Тип ресурса modifiedProperty
description: Указывает все измененные свойства ресурса Azure AD, включая старые и новые значения.
localization_priority: Normal
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4e34501f5011310eb7ade73d1c5d938cb58e65cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136040"
---
# <a name="modifiedproperty-resource-type"></a>Тип ресурса modifiedProperty

Пространство имен: microsoft.graph

Указывает все измененные свойства ресурса Azure AD, включая старые и новые значения.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Указывает имя свойства целевого атрибута, который был изменен.|
|newValue|String|Указывает обновленное значение для правильности.|
|oldValue|String|Указывает предыдущее значение свойства (перед обновлением).|

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

