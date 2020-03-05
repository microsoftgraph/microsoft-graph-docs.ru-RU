---
title: Тип ресурса Екстерналитем
description: Элемент, индексируемый с помощью подключения поиска Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e115135bedecfe4b055e028d5c19902a068c8a53
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498702"
---
# <a name="externalitem-resource-type"></a>Тип ресурса Екстерналитем

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод                                                        | Возвращаемый тип                     | Описание |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [Создание Екстерналитем](../api/externalconnection-put-items.md) | [externalItem](externalitem.md) | Создайте объект Екстерналитем. |
| [Обновление Екстерналитем](../api/externalitem-update.md)          | [externalItem](externalitem.md) | Обновление Екстерналитем. |
| [Удаление Екстерналитем](../api/externalitem-delete.md)          | Нет                            | Удаление Екстерналитем. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                     | Описание                          |
|:-----------|:-------------------------|:-------------------------------------|
| списки        | Коллекция [списков управления доступом](acl.md) | Массив элементов управления доступом. Каждая запись указывает доступ, который предоставляется пользователю или группе. Обязательное. |
| content    | String                   | Представление содержимого элемента в виде обычного текста. Текст в этом свойстве является полнотекстовым индексированным. Необязательное свойство. |
| id         | String                   | Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md). Должен быть буквенно-цифровым и не превышать 128 символов. Обязательное. |
| properties | Объект                   | Контейнер свойств со свойствами элемента. Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md). Обязательное. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

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
  "content": "String",
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
