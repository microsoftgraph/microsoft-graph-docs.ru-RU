---
title: Тип ресурса Аддватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a94f517fe9f5da207febf9e776643a7c17c18d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508403"
---
# <a name="addwatermarkaction-resource-type"></a>Тип ресурса Аддватермаркактион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| фонтколор     | String | Цвет шрифта, который будет использоваться для водяного знака.                      |
| fontName      | String | Имя шрифта, который будет использоваться для водяного знака.                       |
| fontSize      | Int32  | Размер шрифта, используемый для водяного знака.                              |
| макет        | String | Возможные значения: `horizontal`, `diagonal`.                   |
| текст          | String | Содержимое водяного знака.                            |
| уиелементнаме | String | Имя элемента пользовательского интерфейса, в котором следует поместить водяной знак. |

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