---
title: тип ресурса parentLabelDetails
description: Представляет сведения метки родительской метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8f1ebe58c3968e0f912806eb6f339bcfd499b57a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679906"
---
# <a name="parentlabeldetails-resource-type"></a>тип ресурса parentLabelDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения метки родительской метки защиты информации. **parentLabelDetails предоставляет** сведения о единой мете защиты информации. Можно вернуть по [оценкеRemoval,](../api/informationprotectionlabel-evaluateremoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)и [extractLabel](../api/informationprotectionlabel-extractLabel.md)

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| color       | String  | Цвет, который должен отображаться в пользовательском интерфейсе для метки, если настроен.                               |
| description | String  | Описание метки, определенное администратором.                                                                 |
| id          | String  | Идентификатор метки — это глобальный уникальный идентификатор (GUID).                                                          |
| isActive    | Boolean | Указывает, активна метка или нет. Активные метки должны быть скрыты или отключены в пользовательских интерфейсах. |
| name        | String  | Простое имя метки.                                                                             |
| sensitivity | Int32   | Значение чувствительности метки, где более низкий уровень менее чувствителен.                                           |
| tooltip     | String  | Инструмент, который должен отображаться для метки в пользовательском интерфейсе.                                      |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parentLabelDetails",
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
  "description": "parentLabelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->