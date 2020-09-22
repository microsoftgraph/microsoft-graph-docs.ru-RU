---
title: Тип ресурса Аддконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e7a5675cdf150f03b283f664e248319d49c820d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024523"
---
# <a name="addcontentheaderaction-resource-type"></a>Тип ресурса Аддконтенсеадерактион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | String | Возможные значения: `left`, `right`, `center`.               |
| фонтколор     | String | Цвет шрифта, который будет использоваться для заголовка.                      |
| fontName      | String | Имя шрифта, используемого для заголовка.                       |
| fontSize      | Int32  | Размер шрифта, используемый для заголовка.                              |
| margin        | Int32  | Поле заголовка, начиная с верхнего края документа.        |
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

