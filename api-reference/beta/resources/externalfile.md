---
title: тип ресурса externalFile
description: Файл, индексацию с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 64b672c5f97a4093b1498c93f4402d49ff3ba417
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722029"
---
# <a name="externalfile-resource-type"></a>тип ресурса externalFile

Пространство имен: microsoft.graph

> [!CAUTION]
> Тип `externalFile` был обесценим. Разработчики не должны использовать этот тип. Внешние файлы по-прежнему могут индексироваться с помощью [типа externalItem.](externalitem.md)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, индексироваться с помощью подключения Microsoft [Search](externalconnection.md). Этот тип происходит из [типа externalItem.](externalitem.md)

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод                                                        | Возвращаемый тип  | Описание |
|:--------------------------------------------------------------|:-------------|:--|
| [Создание externalFile](../api/externalconnection-put-items.md) | externalFile | Создайте externalFile. |
| [Обновление externalFile](../api/externalitem-update.md)          | externalFile | Обновление externalFile. |
| [Удаление](../api/externalitem-delete.md)                       | Нет         | Удаление externalFile. |

## <a name="properties"></a>Свойства

| Свойство         | Тип                     | Описание                    |
|:-----------------|:-------------------------|:-------------------------------|
| acl              | [коллекция acl](acl.md) | Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. Обязательный атрибут. |
| content          | String                   | Простое текстовое представление содержимого элемента. Текст в этом свойстве индексироваться с полным текстом. Необязательное. |
| id               | String                   | Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnection.md) Должно быть альфа-числом и не более 128 символов. Обязательный атрибут. |
| createdBy        | String                   | Имя пользователя, создав файл. |
| createdDateTime  | DateTimeOffset           | Дата и время создания файла. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| расширение        | String                   | Расширение файла.            |
| lastModifiedBy   | String                   | Имя пользователя, который в последний раз изменил файл. |
| modifiedDateTime | DateTimeOffset           | Дата и время последнего изменения файла. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| name             | String                   | Имя файла. Обязательный атрибут.       |
| size             | Int64                    | Размер файла в bytes. |
| title            | String                   | Название файла.         |
| url              | String                   | URL-адрес для доступа к файлу. Обязательный. |

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


