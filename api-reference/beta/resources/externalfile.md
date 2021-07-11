---
title: тип ресурса externalFile
description: Файл, индексацию с помощью Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 23a89cb83e85f16fc4cf2faa3c285bafb9fd66cf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366550"
---
# <a name="externalfile-resource-type"></a>тип ресурса externalFile

Пространство имен: microsoft.graph

> [!CAUTION]
> Тип `externalFile` был обесценим. Разработчики не должны использовать этот тип. Внешние файлы по-прежнему могут индексироваться с помощью [типа externalItem.](externalitem.md)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, индексация с помощью Поиск (Майкрософт) [подключения.](externalconnection.md) Этот тип происходит из [типа externalItem.](externalitem.md)

## <a name="methods"></a>Методы

| Метод                                                        | Возвращаемый тип  | Описание |
|:--------------------------------------------------------------|:-------------|:--|
| [Создание externalFile](../api/externalconnection-put-items.md) | externalFile | Создайте externalFile. |
| [Обновление externalFile](../api/externalitem-update.md)          | externalFile | Обновление externalFile. |
| [Delete](../api/externalitem-delete.md)                       | Нет         | Удаление externalFile. |

## <a name="properties"></a>Свойства

| Свойство         | Тип                     | Описание                    |
|:-----------------|:-------------------------|:-------------------------------|
| acl              | [коллекция acl](acl.md) | Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. Обязательный. |
| content          | String                   | Простое текстовое представление содержимого элемента. Текст в этом свойстве индексироваться с полным текстом. Необязательный параметр. |
| id               | String                   | Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnection.md) Должно быть альфа-числом и не более 128 символов. Обязательный. |
| createdBy        | String                   | Имя пользователя, создав файл. |
| createdDateTime  | DateTimeOffset           | Дата и время создания файла. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| расширение        | String                   | Расширение файла.            |
| lastModifiedBy   | String                   | Имя пользователя, который в последний раз изменил файл. |
| modifiedDateTime | DateTimeOffset           | Дата и время последнего изменения файла. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| name             | String                   | Имя файла. Обязательный.       |
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


