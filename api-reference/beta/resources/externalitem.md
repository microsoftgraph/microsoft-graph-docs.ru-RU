---
title: Тип ресурса externalItem
description: Элемент, добавленный к подключению Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 63f0285427a17280169d31a35c3a622d38a6a8c6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161710"
---
# <a name="externalitem-resource-type"></a>Тип ресурса externalItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, добавленный в подключение Microsoft [Graph.](externalconnection.md) 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод                                                        | Возвращаемый тип                     | Описание |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [Создание externalItem](../api/externalconnection-put-items.md) | [externalItem](externalitem.md) | Создайте externalItem. |
| [Get externalItem](../api/externalitem-get.md)                | [externalItem](externalitem.md) | Получите externalItem.    |
| [Обновление externalItem](../api/externalitem-update.md)          | [externalItem](externalitem.md) | Обновление externalItem. |
| [Удаление externalItem](../api/externalitem-delete.md)          | Нет                            | Удаление externalItem. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                     | Описание                          |
|:-----------|:-------------------------|:-------------------------------------|
| acl        | [Коллекция acl](acl.md) | Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. Обязательно. |
| содержимое    | [externalItemContent](externalitemcontent.md) | Обычное представление содержимого элемента. Текст в этом свойстве индексироваться в полном тексте. Необязательный параметр. |
| id         | String                   | Предоставленный разработчиком уникальный ИД элемента в пределах содержащего [externalConnection.](externalconnection.md) Должно быть буквано-цифровая и не более 128 символов. Обязательно. |
| properties | Объект                   | Пакет свойств со свойствами элемента. Свойства ДОЛЖНЫ соответствовать схеме, [определенной](schema.md) для [externalConnection.](externalconnection.md) Обязательный. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": {"@odata.type": "microsoft.graph.externalItemContent"},
  "id": "String (identifier)",
  "properties": "Object"
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
    "Error: microsoft.graph.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
