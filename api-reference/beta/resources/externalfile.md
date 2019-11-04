---
title: Тип ресурса Екстерналфиле
description: Файл, индексируемый с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bee1ad36769066550e1a6adc3ce7427602c66e66
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938985"
---
# <a name="externalfile-resource-type"></a>Тип ресурса Екстерналфиле

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft. Этот тип является производным от типа [екстерналитем](externalitem.md) .

## <a name="methods"></a>Методы

| Метод                                                        | Возвращаемый тип  | Описание |
|:--------------------------------------------------------------|:-------------|:--|
| [Создание Екстерналфиле](../api/externalconnection-put-items.md) | екстерналфиле | Создайте объект Екстерналфиле. |
| [Обновление Екстерналфиле](../api/externalitem-update.md)          | екстерналфиле | Обновление Екстерналфиле. |
| [Delete](../api/externalitem-delete.md)                       | Нет.         | Удаление Екстерналфиле. |

## <a name="properties"></a>Свойства

| Свойство         | Тип                     | Описание                    |
|:-----------------|:-------------------------|:-------------------------------|
| списки              | Коллекция [списков управления доступом](acl.md) | Массив элементов управления доступом. Каждая запись указывает доступ, который предоставляется пользователю или группе. Обязательный элемент. |
| content          | String                   | Представление содержимого элемента в виде обычного текста. Текст в этом свойстве является полнотекстовым индексированным. Необязательный элемент. |
| id               | Строка                   | Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md). Должен быть буквенно-цифровым и не превышать 128 символов. Обязательный элемент. |
| createdBy        | Строка                   | Имя пользователя, создавшего файл. |
| createdDateTime  | DateTimeOffset           | Дата и время создания файла. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
| модулей        | Строка                   | Расширение файла.            |
| lastModifiedBy   | Строка                   | Имя пользователя, который последним изменил файл. |
| modifiedDateTime | DateTimeOffset           | Дата и время последнего изменения файла. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
| name             | Строка                   | Имя файла. Обязательный элемент.       |
| size             | Int64                    | Размер файла в байтах. |
| title            | Строка                   | Заголовок файла.         |
| url              | Строка                   | URL-адрес для доступа к файлу. Обязательный элемент. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalFile",
  "baseType": "microsoft.graph.externalItem"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": "String",
  "id": "String (identifier)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "extension": "String",
  "lastModifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "title": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
