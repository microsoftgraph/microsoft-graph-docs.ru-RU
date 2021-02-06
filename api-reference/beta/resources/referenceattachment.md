---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых расположениях хранения, вложенных в '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 914d04a6482b96fda0ee55c92f25bf950e594173
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136772"
---
# <a name="referenceattachment-resource-type"></a>Тип ресурса referenceAttachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для [](../resources/message.md)бизнеса или других поддерживаемых расположениях хранения, прикрепленных к событию, [](../resources/event.md)сообщению или публикации. [](../resources/post.md)

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[получение](../api/attachment-get.md); | [referenceAttachment](referenceattachment.md) |Чтение свойств и связей объекта referenceAttachment.|
|[Delete](../api/attachment-delete.md) | Нет |Удаление объекта referenceAttachment. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип контента этого вложения. Необязательный параметр.|
|id|Строка|Идентификатор вложения.  Только для чтения.|
|isFolder|Boolean|Указывает, является ли вложение ссылкой на папку. Должно иметь true, если **sourceUrl** является ссылкой на папку. Необязательный параметр.|
|isInline|Boolean|Значение true указывает, что вложение встроено в содержимое объекта. Необязательный параметр.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Необязательный параметр.|
|name|String|Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла. Обязательный элемент.|
|permission|referenceAttachmentPermission|Указывает разрешения, предоставленные для вложения типом поставщика **в providerType.** Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Необязательный параметр.|
|previewUrl|Строка|Применяется только к вложению ссылки изображения — URL-адресу для получения изображения предварительного просмотра. Используйте **thumbnailUrl и** **previewUrl** только в том случае, **если sourceUrl** идентифицирует файл изображения. Необязательный параметр.|
|providerType|referenceAttachmentProvider|Тип поставщика, который поддерживает вложение этого contentType. Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Необязательный параметр.|
|size|Int32|Размер метаданных в виде ветвей, которые хранятся в сообщении для эталонного вложения. Это значение не отображает фактический размер файла. Необязательный параметр.|
|sourceUrl|Строка|URL-адрес для получения содержимого вложения. If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true. Обязательный элемент.|
|thumbnailUrl|Строка|Применяется только к вложению ссылки изображения — URL-адресу для получения эскиза. Используйте **thumbnailUrl и** **previewUrl** только в том случае, **если sourceUrl** идентифицирует файл изображения. Необязательный параметр.|

## <a name="relationships"></a>Связи
Нет



## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


