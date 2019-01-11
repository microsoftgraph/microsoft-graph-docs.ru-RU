---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для бизнеса облачных диска и других местах, поддерживаемые хранилища, подключенного к '
localization_priority: Normal
ms.openlocfilehash: 6a334b303bea7aff768733434b9ba882de237a12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880054"
---
# <a name="referenceattachment-resource-type"></a>Тип ресурса referenceAttachment

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
|contentType|String|Тип контента этого вложения. Необязательное.|
|id|String|Идентификатор вложения.  Только для чтения.|
|isFolder|Логический|Указывает, является ли вложение ссылок в папку. Необходимо установить это значение true, если **sourceUrl** — это ссылка на папку. Необязательное.|
|isInline|Boolean|Значение true указывает, что вложение встроено в содержимое объекта. Необязательное.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Необязательное.|
|name|Строка|Текст, который отображается под значок, обозначающий внедренного вложения. Она не обязательно должна находиться фактическое имя файла. Обязательный.|
|разрешение|ReferenceAttachmentPermissions|Задает разрешения, предоставленные вложения по типу поставщика в **providerType**. Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Необязательное.|
|previewUrl|Строка|Применяется только вложения ссылку объекта на изображении - URL-адрес для получения изображения для предварительного просмотра. Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения. Необязательное.|
|providerType|ReferenceAttachmentProviders|Тип поставщика, который поддерживает вложение в этом contentType. Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Необязательное.|
|size|Int32|Размер метаданных в байтах, которые хранятся на сообщение для вложения ссылку. Это значение не отображает фактический размер файла. Необязательное.|
|sourceUrl|Строка|URL-адрес для получения содержимого вложения. Если это URL-адрес в папку, для папки для правильного отображения в Outlook или Outlook в Интернете, задайте его **isFolder** имеет значение true. Обязательный.|
|thumbnailUrl|Строка|Применяется только вложения ссылку объекта на изображении - URL-адрес для получения эскизное изображение. Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения. Необязательное.|

## <a name="relationships"></a>Связи
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
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
