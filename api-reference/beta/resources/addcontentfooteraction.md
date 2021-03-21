---
title: тип ресурса addContentFooterAction
description: Представляет действие, которое указывает сведения на подножке контента, которая должна быть добавлена в сведения, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 20debce7dc408bd10d4f62b905efa55156d4d4ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962142"
---
# <a name="addcontentfooteraction-resource-type"></a>тип ресурса addContentFooterAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, которое указывает сведения на подножке контента, которая должна быть добавлена в сведения, если это применимо.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | Строка | Возможные значения: `left`, `right`, `center`.               |
| fontColor     | Строка | Цвет шрифта, используемого для подножки.                      |
| fontName      | Строка | Имя шрифта, используемого для подножки.                       |
| fontSize      | Int32  | Размер шрифта для использования для подножки.                              |
| margin        | Int32  | Поле заглавной строки из нижней части документа.     |
| текст          | Строка | Содержимое самого подножки.                            |
| uiElementName | Строка | Имя элемента пользовательского интерфейса, в котором должен размещаться подножка. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentFooterAction",
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
  "description": "addContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

