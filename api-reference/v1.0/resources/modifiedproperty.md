---
title: тип ресурса modifiedProperty
description: Указывает все свойства измененного ресурса Azure AD, включая старые и новые значения.
localization_priority: Normal
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9b1c520ac4be4e0c0957fe2b9f4f833f4065a19a2ed76ecd3166a46f7e50de6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192210"
---
# <a name="modifiedproperty-resource-type"></a>тип ресурса modifiedProperty

Пространство имен: microsoft.graph

Указывает все свойства измененного ресурса Azure AD, включая старые и новые значения.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Указывает имя свойства измененного целевого атрибута.|
|newValue|String|Указывает обновленное значение для правильности.|
|oldValue|String|Указывает предыдущее значение (перед обновлением) для свойства.|

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

