---
title: Тип ресурса Лабелдетаилс
description: Представляет сведения о метке метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cf031459004e0c0d56b5b09145ed897a9f960142
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523011"
---
# <a name="labeldetails-resource-type"></a>Тип ресурса Лабелдетаилс

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о метке метки защиты информации. **лабелдетаилс** предоставляет сведения об отдельной метке защиты информации. Могут возвращаться [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md), [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)и [екстрактлабел](../api/informationprotectionlabel-extractLabel.md)

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| color       | String  | Цвет, который должен отображаться в пользовательском интерфейсе для метки, если она настроена.                               |
| description | String  | Заданное администратором описание метки.                                                                 |
| id          | Строка  | ИДЕНТИФИКАТОР метки является глобальным уникальным идентификатором (GUID).                                                          |
| isActive    | Логический | Указывает, активна ли метка. Активные метки должны быть скрыты или отключены в пользовательских интерфейсах. |
| name        | String  | Имя в виде открытого текста метки.                                                                             |
| sensitivity | Int32   | Значение чувствительности метки, где меньше конфиденциально.                                           |
| tooltip     | String  | Всплывающая подсказка, отображаемая для метки в пользовательском интерфейсе.                                      |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelDetails",
  "baseType": null
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->