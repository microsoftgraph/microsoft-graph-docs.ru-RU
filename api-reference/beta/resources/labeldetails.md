---
title: тип ресурса labelDetails
description: Представляет сведения метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: eb66e395d18b7887942753abdebd91d398844290
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579302"
---
# <a name="labeldetails-resource-type"></a>тип ресурса labelDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения метки защиты информации. **LabelDetails предоставляет** сведения о единой мете защиты информации. Наследует от [parentLabelDetails](parentlabeldetails.md). Можно вернуть по [оценкеRemoval,](../api/informationprotectionlabel-evaluateremoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)и [extractLabel](../api/informationprotectionlabel-extractLabel.md)

## <a name="properties"></a>Свойства

| Свойство    | Тип                                         | Описание                                                                                                  |
| :---------- | :------------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| color       | String                                       | Цвет, который должен отображаться в пользовательском интерфейсе для метки, если настроен.                               |
| description | Строка                                       | Описание метки, определенное администратором.                                                                 |
| id          | Строка                                       | Идентификатор метки — это глобальный уникальный идентификатор (GUID).                                                         |
| isActive    | Boolean                                      | Указывает, активна метка или нет. Активные метки должны быть скрыты или отключены в пользовательских интерфейсах. |
| name        | String                                       | Простое имя метки.                                                                             |
| sensitivity | Int32                                        | Значение чувствительности метки, где более низкий уровень менее чувствителен.                                           |
| tooltip     | Строка                                       | Инструмент, который должен отображаться для метки в пользовательском интерфейсе.                                      |
| родитель      | parentLabelDetails | Родительская метка, связанная с детской меткой.                                                              |

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

