---
title: Тип ресурса Аддватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ba3bd679d01d31aec779071a766ab804761e614
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939168"
---
# <a name="addwatermarkaction-resource-type"></a>Тип ресурса Аддватермаркактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| фонтколор     | Строка | Цвет шрифта, который будет использоваться для водяного знака.                      |
| fontName      | Строка | Имя шрифта, который будет использоваться для водяного знака.                       |
| fontSize      | Int32  | Размер шрифта, используемый для водяного знака.                              |
| макет        | String | Возможные значения: `horizontal`, `diagonal`.                   |
| текст          | Строка | Содержимое водяного знака.                            |
| уиелементнаме | Строка | Имя элемента пользовательского интерфейса, в котором следует поместить водяной знак. |

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