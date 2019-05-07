---
title: Тип ресурса Модифиедпроперти
description: Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: d87d0170dc811db074026e60efc63df928c65ada
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629280"
---
# <a name="modifiedproperty-resource-type"></a>Тип ресурса Модифиедпроперти

Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Указывает имя свойства целевого атрибута, которое было изменено.|
|newValue|String|Указывает обновленное значение для правильной работы.|
|oldValue|String|Указывает предыдущее значение свойства (перед обновлением).|

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
