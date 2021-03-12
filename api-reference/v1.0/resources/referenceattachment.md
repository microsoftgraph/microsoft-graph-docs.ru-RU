---
title: Тип ресурса referenceAttachment
description: Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.
localization_priority: Normal
ms.prod: outlook
author: abheek-das
doc_type: resourcePageType
ms.openlocfilehash: 8a9b4d43a7bbc31c737c85ea1a18bd14beefcb05
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722414"
---
# <a name="referenceattachment-resource-type"></a>Тип ресурса referenceAttachment

Пространство имен: microsoft.graph

Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[получение](../api/attachment-get.md); | [referenceAttachment](referenceattachment.md) |Чтение свойств и связей объекта referenceAttachment.|
|[удаление](../api/attachment-delete.md); | Нет |Удаление объекта referenceAttachment. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип контента этого вложения.|
|id|String|Идентификатор вложения.  Только для чтения.|
|isInline|Boolean|Значение true указывает, что вложение встроено в содержимое объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|name|String|Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла.|
|size|Int32|Объем метаданных, которые хранятся в сообщении с вложением (в байтах). Это значение не отображает фактический размер файла.|

## <a name="relationships"></a>Связи
Нет



## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

