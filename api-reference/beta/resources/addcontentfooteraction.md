---
title: Тип ресурса Аддконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b1a2cb0f3e2ffbfb5554c4ae0323cf4fd028e0c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939111"
---
# <a name="addcontentfooteraction-resource-type"></a>Тип ресурса Аддконтентфутерактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | Строка | Возможные значения: `left`, `right`, `center`.               |
| фонтколор     | Строка | Цвет шрифта, который будет использоваться для нижнего колонтитула.                      |
| fontName      | Строка | Имя шрифта, который будет использоваться для нижнего колонтитула.                       |
| fontSize      | Int32  | Размер шрифта, который будет использоваться для нижнего колонтитула.                              |
| поля        | Int32  | Поле заголовка из нижней части документа.     |
| текст          | Строка | Содержимое нижнего колонтитула.                            |
| уиелементнаме | Строка | Имя элемента пользовательского интерфейса, в котором следует поместить нижний колонтитул. |

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