---
title: Тип ресурса Аддконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 341af43f03d8a319c7aaec535681f21db0a7f7f4
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939109"
---
# <a name="addcontentheaderaction-resource-type"></a>Тип ресурса Аддконтенсеадерактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | Строка | Возможные значения: `left`, `right`, `center`.               |
| фонтколор     | Строка | Цвет шрифта, который будет использоваться для заголовка.                      |
| fontName      | Строка | Имя шрифта, используемого для заголовка.                       |
| fontSize      | Int32  | Размер шрифта, используемый для заголовка.                              |
| поля        | Int32  | Поле заголовка, начиная с верхнего края документа.        |
| текст          | Строка | Содержимое самого верхнего колонтитула.                            |
| уиелементнаме | Строка | Имя элемента пользовательского интерфейса, в котором следует поместить заголовок. |

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