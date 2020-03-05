---
title: Тип ресурса Аддконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d426252b6ab83557c3d3085ac4ffa7a530aae271
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508410"
---
# <a name="addcontentheaderaction-resource-type"></a>Тип ресурса Аддконтенсеадерактион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | String | Возможные значения: `left`, `right`, `center`.               |
| фонтколор     | String | Цвет шрифта, который будет использоваться для заголовка.                      |
| fontName      | String | Имя шрифта, используемого для заголовка.                       |
| fontSize      | Int32  | Размер шрифта, используемый для заголовка.                              |
| поля        | Int32  | Поле заголовка, начиная с верхнего края документа.        |
| текст          | String | Содержимое самого верхнего колонтитула.                            |
| уиелементнаме | String | Имя элемента пользовательского интерфейса, в котором следует поместить заголовок. |

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