---
title: Тип ресурса Висуалпропертиес
description: 'Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 62580847844a4b397ed117ea4b256cc4f035577a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057691"
---
# <a name="visualproperties-resource-type"></a>Тип ресурса Висуалпропертиес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|title|String|Название визуального уведомления пользователя. Это поле является обязательным для полезных данных визуальных уведомлений. |
|body|String|Текст уведомления визуального пользователя. Основной текст является необязательным.|


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.visualProperties",
  "baseType": null
}-->

```json
{
  "title": "String",
  "body": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

