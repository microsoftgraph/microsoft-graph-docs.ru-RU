---
title: тип ресурса externalItem
description: Элемент, добавленный к подключению microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c570a7e4754724ca4239b7e3dbe128d09db9d75
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366533"
---
# <a name="externalitem-resource-type"></a>тип ресурса externalItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, добавленный к подключению microsoft [Graph.](externalconnection.md) 

## <a name="methods"></a>Методы

| Метод                                                        | Возвращаемый тип                     | Описание |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [Создание externalItem](../api/externalconnection-put-items.md) | [externalItem](externalitem.md) | Создание externalItem. |
| [Get externalItem](../api/externalitem-get.md)                | [externalItem](externalitem.md) | Получите externalItem.    |
| [Обновление externalItem](../api/externalitem-update.md)          | [externalItem](externalitem.md) | Обновление externalItem. |
| [Удаление externalItem](../api/externalitem-delete.md)          | Нет                            | Удаление externalItem. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                     | Описание                          |
|:-----------|:-------------------------|:-------------------------------------|
| acl        | [коллекция acl](acl.md) | Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. Обязательный. |
| содержимое    | [externalItemContent](externalitemcontent.md) | Простое текстовое представление содержимого элемента. Текст в этом свойстве индексироваться с полным текстом. Необязательный параметр. |
| id         | String                   | Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnection.md) Должно быть альфа-числом и не более 128 символов. Обязательный. |
| properties | Объект                   | Пакет свойств со свойствами элемента. Свойства должны соответствовать [схеме,](schema.md) определенной для [externalConnection.](externalconnection.md) Обязательный. |

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
