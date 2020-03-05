---
title: Тип ресурса Аддконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 05bbd7ee4b2d4b2b9c4e772b19bd26c86d91cc69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508424"
---
# <a name="addcontentfooteraction-resource-type"></a>Тип ресурса Аддконтентфутерактион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | String | Возможные значения: `left`, `right`, `center`.               |
| фонтколор     | String | Цвет шрифта, который будет использоваться для нижнего колонтитула.                      |
| fontName      | String | Имя шрифта, который будет использоваться для нижнего колонтитула.                       |
| fontSize      | Int32  | Размер шрифта, который будет использоваться для нижнего колонтитула.                              |
| поля        | Int32  | Поле заголовка из нижней части документа.     |
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