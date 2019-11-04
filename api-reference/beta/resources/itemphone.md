---
title: Тип ресурса Итемфоне
description: Тип ресурса Итемфоне
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a40a0a096fa6f0616a8ff44e41e25791873fa82f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939322"
---
# <a name="itemphone-resource-type"></a>Тип ресурса Итемфоне

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о телефонных номерах, связанных с пользователем в различных службах.

## <a name="methods"></a>Методы

| Метод                                     | Возвращаемый тип               | Описание                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [Получение Итемфоне](../api/itemphone-get.md)   | [итемфоне](itemphone.md) | Чтение свойств и связей объекта **итемфоне** . |
| [Обновление Итемфоне](../api/itemphone-update.md)       | [итемфоне](itemphone.md) | Обновление объекта **итемфоне** .                               |
| [Удаление Итемфоне](../api/itemphone-delete.md)       | Нет.                      | Удаление объекта **итемфоне** .                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|displayName   |Строка       | Содержит понятное имя для номера телефона.                                                                                  |
|число        |Строка       | Содержит номер телефона.                                                                                                       |
|type          |string       | Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "number": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemPhone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
