---
title: тип ресурса externalItem
description: Элемент, добавленный к подключению microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8660365d5d08d0084066cea3349e841269469241
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467859"
---
# <a name="externalitem-resource-type"></a>тип ресурса externalItem

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, добавленный к подключению microsoft [Graph.](externalconnectors-externalconnection.md)

## <a name="methods"></a>Методы

| Метод                                                        | Возвращаемый тип                     | Описание |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [Создание externalItem](../api/externalconnectors-externalconnection-put-items.md) | [externalItem](externalconnectors-externalitem.md) | Создание externalItem. |
| [Get externalItem](../api/externalconnectors-externalitem-get.md)                | [externalItem](externalconnectors-externalitem.md) | Получите externalItem.    |
| [Обновление externalItem](../api/externalconnectors-externalitem-update.md)          | [externalItem](externalconnectors-externalitem.md) | Обновление externalItem. |
| [Удаление externalItem](../api/externalconnectors-externalitem-delete.md)          | Нет                            | Удаление externalItem. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                     | Описание                          |
|:-----------|:-------------------------|:-------------------------------------|
| acl        | [коллекция microsoft.graph.externalConnectors.acl](externalconnectors-acl.md) | Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. Обязательный элемент. |
| содержимое    | [microsoft.graph.externalConnectors.externalItemContent](externalconnectors-externalitemcontent.md) | Простое текстовое представление содержимого элемента. Текст в этом свойстве индексироваться с полным текстом. Необязательное. |
| id         | String                   | Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnectors-externalconnection.md) Должно быть альфа-числом и не более 128 символов. Обязательный элемент. |
| properties | Объект                   | Пакет свойств со свойствами элемента. Свойства должны соответствовать [схеме,](externalconnectors-schema.md) определенной для [externalConnection.](externalconnectors-externalconnection.md) Обязательный. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "id": "String (identifier)",
  "properties": "Object",
  "content": { "@odata.type": "microsoft.graph.externalConnectors.externalItemContent" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.externalConnectors.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
