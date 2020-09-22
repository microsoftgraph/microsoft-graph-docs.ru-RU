---
title: Тип ресурса Екстерналитем
description: Элемент, добавляемый в подключение Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ec2c66c91612738295ac4ba49524593d61ff70e4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193409"
---
# <a name="externalitem-resource-type"></a>Тип ресурса Екстерналитем

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, добавляемый в [Подключение](externalconnection.md)Microsoft Graph. 

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
| списки        | Коллекция [списков управления доступом](acl.md) | Массив элементов управления доступом. Каждая запись указывает доступ, который предоставляется пользователю или группе. Обязательно. |
| содержимое    | [екстерналитемконтент](externalitemcontent.md) | Представление содержимого элемента в виде обычного текста. Текст в этом свойстве является полнотекстовым индексированным. Необязательно. |
| id         | String                   | Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md). Должен быть буквенно-цифровым и не превышать 128 символов. Обязательно. |
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
