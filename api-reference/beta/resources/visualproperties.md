---
title: Тип ресурса Висуалпропертиес
description: 'Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 1678f560fa003c1884a9fa673ee85b7473e36c88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519465"
---
# <a name="visualproperties-resource-type"></a>Тип ресурса Висуалпропертиес

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|title|String|Название визуального уведомления пользователя. Это поле является обязательным для полезных данных визуальных уведомлений. |
|body|String|Текст уведомления визуального пользователя. Основной текст является необязательным.|


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