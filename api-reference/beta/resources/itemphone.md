---
title: Тип ресурса Итемфоне
description: Тип ресурса Итемфоне
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 48c585a05043b4f17e5e7406eb44b9150b5e5bdc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523067"
---
# <a name="itemphone-resource-type"></a>Тип ресурса Итемфоне

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.

## <a name="methods"></a>Методы

| Метод                                     | Возвращаемый тип               | Описание                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [Получение Итемфоне](../api/itemphone-get.md)   | [итемфоне](itemphone.md) | Чтение свойств и связей объекта **итемфоне** . |
| [Обновление Итемфоне](../api/itemphone-update.md)       | [итемфоне](itemphone.md) | Обновление объекта **итемфоне** .                               |
| [Удаление Итемфоне](../api/itemphone-delete.md)       | Нет                      | Удаление объекта **итемфоне** .                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|displayName   |Строка       | Содержит понятное имя для номера телефона.                                                                                  |
|число        |String       | Содержит номер телефона.                                                                                                       |
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
