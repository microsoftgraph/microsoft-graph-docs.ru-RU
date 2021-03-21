---
title: тип ресурса addWatermarkAction
description: Представляет действие, которое указывает сведения о водяном знаке контента, который будет добавлен в сведения, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db493c57d6de7c840e5f0606743392698cb475b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962128"
---
# <a name="addwatermarkaction-resource-type"></a>тип ресурса addWatermarkAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, которое указывает сведения о водяном знаке контента, который будет добавлен в сведения, если это применимо.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| fontColor     | Строка | Цвет шрифта, используемого для водяного знака.                      |
| fontName      | Строка | Имя шрифта, используемого для водяного знака.                       |
| fontSize      | Int32  | Размер шрифта для водяного знака.                              |
| макет        | String | Возможные значения: `horizontal`, `diagonal`.                   |
| текст          | Строка | Содержимое самого водяного знака.                            |
| uiElementName | Строка | Имя элемента пользовательского интерфейса, в котором должен быть размещен водяной знак. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "layout": "String",
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addWatermarkAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

