---
title: тип ресурса addContentHeaderAction
description: Представляет действие, которое указывает сведения о загонщике контента, который будет добавлен в сведения, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 65754bffc034611fd319403cd81d931addfea9f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962139"
---
# <a name="addcontentheaderaction-resource-type"></a>тип ресурса addContentHeaderAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, которое указывает сведения о загонщике контента, который будет добавлен в сведения, если это применимо.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | Строка | Возможные значения: `left`, `right`, `center`.               |
| fontColor     | Строка | Цвет шрифта, используемого для загона.                      |
| fontName      | Строка | Имя шрифта, используемого для загона.                       |
| fontSize      | Int32  | Размер шрифта, который можно использовать для загона.                              |
| margin        | Int32  | Поле загонщика в верхней части документа.        |
| текст          | Строка | Содержимое самого загона.                            |
| uiElementName | Строка | Имя элемента пользовательского интерфейса, в котором должен быть размещен заголовщик. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentHeaderAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "alignment": "String",
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "margin": 1024,
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

