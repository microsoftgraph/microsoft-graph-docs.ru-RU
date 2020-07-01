---
title: Тип ресурса Екстерналитем
description: Элемент, индексируемый с помощью подключения поиска Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3b82f67f12d263e56e3375ed87a9d6dff71c2204
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989905"
---
# <a name="externalitem-resource-type"></a>Тип ресурса Екстерналитем

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод                                                        | Возвращаемый тип                     | Описание |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [Создание Екстерналитем](../api/externalconnection-put-items.md) | [externalItem](externalitem.md) | Создайте объект Екстерналитем. |
| [Получение Екстерналитем](../api/externalitem-get.md)                | [externalItem](externalitem.md) | Получение Екстерналитем.    |
| [Обновление Екстерналитем](../api/externalitem-update.md)          | [externalItem](externalitem.md) | Обновление Екстерналитем. |
| [Удаление Екстерналитем](../api/externalitem-delete.md)          | Нет                            | Удаление Екстерналитем. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                     | Описание                          |
|:-----------|:-------------------------|:-------------------------------------|
| списки        | Коллекция [списков управления доступом](acl.md) | Массив элементов управления доступом. Каждая запись указывает доступ, который предоставляется пользователю или группе. Обязательный. |
| содержимое    | [екстерналитемконтент](externalitemcontent.md) | Представление содержимого элемента в виде обычного текста или в формате HTML. Текст в этом свойстве является полнотекстовым индексированным. Необязательный параметр. |
| id         | String                   | Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md). Должен быть буквенно-цифровым и не превышать 128 символов. Обязательный. |
| properties | Объект                   | Контейнер свойств со свойствами элемента. Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md). Обязательный. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "baseType": "",
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
