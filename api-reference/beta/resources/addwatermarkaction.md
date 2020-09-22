---
title: Тип ресурса Аддватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 884553ce1181fd3d79fe0e953fe7703b386698b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024451"
---
# <a name="addwatermarkaction-resource-type"></a>Тип ресурса Аддватермаркактион

Пространство имен: microsoft.graph

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

