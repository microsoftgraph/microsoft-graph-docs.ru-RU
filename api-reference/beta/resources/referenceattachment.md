---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для бизнеса облачных диска и других местах, поддерживаемые хранилища, подключенного к '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512712"
---
# <a name="referenceattachment-resource-type"></a>Тип ресурса referenceAttachment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для Business cloud диска или другие поддерживаемые места хранения, подключенного к [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md) .

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |Чтение свойств и связей объекта referenceAttachment.|
|[Delete](../api/attachment-delete.md) | Нет |Удаление объекта referenceAttachment. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип контента этого вложения. Необязательный параметр.|
|id|String|Идентификатор вложения.  Только для чтения.|
|isFolder|Логическое|Указывает, является ли вложение ссылок в папку. Необходимо установить это значение true, если **sourceUrl** — это ссылка на папку. Необязательный параметр.|
|isInline|Boolean|Значение true указывает, что вложение встроено в содержимое объекта. Необязательный параметр.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Необязательный параметр.|
|name|String|Текст, который отображается под значок, обозначающий внедренного вложения. Она не обязательно должна находиться фактическое имя файла. Обязательный.|
|разрешение|ReferenceAttachmentPermissions|Задает разрешения, предоставленные вложения по типу поставщика в **providerType**. Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Необязательный параметр.|
|PreviewUrl|String|Применяется только вложения ссылку объекта на изображении - URL-адрес для получения изображения для предварительного просмотра. Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения. Необязательный параметр.|
|providerType|ReferenceAttachmentProviders|Тип поставщика, который поддерживает вложение в этом contentType. Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Необязательный параметр.|
|size|Int32|Размер метаданных в байтах, которые хранятся на сообщение для вложения ссылку. Это значение не отображает фактический размер файла. Необязательный параметр.|
|SourceURL|String|URL-адрес для получения содержимого вложения. Если это URL-адрес в папку, для папки для правильного отображения в Outlook или Outlook в Интернете, задайте его **isFolder** имеет значение true. Обязательный.|
|thumbnailUrl|String|Применяется только вложения ссылку объекта на изображении - URL-адрес для получения эскизное изображение. Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения. Необязательный параметр.|

## <a name="relationships"></a>Отношения
Нет



## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
