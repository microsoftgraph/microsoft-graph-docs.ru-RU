---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых хранилищах, присоединенных к '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: e0c3723648710fb1640927fad10e0847e1e155a6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721322"
---
# <a name="referenceattachment-resource-type"></a>Тип ресурса referenceAttachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для [](../resources/message.md)бизнеса или других поддерживаемых хранилищах, присоединенных к событию, [](../resources/event.md)сообщению или сообщению. [](../resources/post.md)

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[получение](../api/attachment-get.md); | [referenceAttachment](referenceattachment.md) |Чтение свойств и связей объекта referenceAttachment.|
|[Удаление](../api/attachment-delete.md) | Нет |Удаление объекта referenceAttachment. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип контента этого вложения. Необязательное.|
|id|String|Идентификатор вложения.  Только для чтения.|
|isFolder|Boolean|Указывает, является ли вложение ссылкой на папку. Необходимо установить это, если **sourceUrl** является ссылкой на папку. Необязательное.|
|isInline|Boolean|Значение true указывает, что вложение встроено в содержимое объекта. Необязательное.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательное.|
|name|String|Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла. Обязательный атрибут.|
|разрешение|referenceAttachmentPermission|Указывает разрешения, предоставленные для вложения типом поставщика в **providerType.** Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Необязательное.|
|previewUrl|String|Применяется только к ссылке на вложение изображения — URL-адрес для получения изображения предварительного просмотра. Используйте **thumbnailUrl и** **previewUrl** только тогда, когда **sourceUrl** идентифицирует файл изображений. Необязательное.|
|providerType|referenceAttachmentProvider|Тип поставщика, который поддерживает вложение этого contentType. Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Необязательное.|
|size|Int32|Размер метаданных в bytes, хранимых в сообщении для эталонного вложения. Это значение не отображает фактический размер файла. Необязательное.|
|sourceUrl|String|URL-адрес для получения содержимого вложения. Если это URL-адрес папки, то для правильного отображения папки в Outlook или Outlook в Интернете заданной **являетсяFolder** to true. Обязательный атрибут.|
|thumbnailUrl|String|Применяется только к ссылке на вложение изображения — URL-адрес для получения эскизного изображения. Используйте **thumbnailUrl и** **previewUrl** только тогда, когда **sourceUrl** идентифицирует файл изображений. Необязательное.|

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


