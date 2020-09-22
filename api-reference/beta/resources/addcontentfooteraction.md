---
title: Тип ресурса Аддконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4e9edf4007d7bc5d4028e4f9202e09647ca863
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024521"
---
# <a name="addcontentfooteraction-resource-type"></a>Тип ресурса Аддконтентфутерактион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | String | Возможные значения: `left`, `right`, `center`.               |
| фонтколор     | String | Цвет шрифта, который будет использоваться для нижнего колонтитула.                      |
| fontName      | String | Имя шрифта, который будет использоваться для нижнего колонтитула.                       |
| fontSize      | Int32  | Размер шрифта, который будет использоваться для нижнего колонтитула.                              |
| margin        | Int32  | Поле заголовка из нижней части документа.     |
| текст          | String | Содержимое нижнего колонтитула.                            |
| уиелементнаме | String | Имя элемента пользовательского интерфейса, в котором следует поместить нижний колонтитул. |

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

