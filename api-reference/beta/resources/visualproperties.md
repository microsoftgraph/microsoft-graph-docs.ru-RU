---
title: Тип ресурса Висуалпропертиес
description: 'Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: f03563549cc1b2f42a274032dab7b310511c70c7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939182"
---
# <a name="visualproperties-resource-type"></a>Тип ресурса Висуалпропертиес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|title|Строка|Название визуального уведомления пользователя. Это поле является обязательным для полезных данных визуальных уведомлений. |
|body|Строка|Текст уведомления визуального пользователя. Основной текст является необязательным.|


## <a name="json-representation"></a>Представление JSON

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