---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, подключенных к '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 426d746305b2a8418fb30515720d888226d3da74
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462214"
---
# <a name="referenceattachment-resource-type"></a>Тип ресурса referenceAttachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, прикрепленных к [событию](../resources/event.md), [сообщению](../resources/message.md)или [записи](../resources/post.md) .

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[получение](../api/attachment-get.md); | [referenceAttachment](referenceattachment.md) |Чтение свойств и связей объекта referenceAttachment.|
|[Удаление](../api/attachment-delete.md) | Нет |Удаление объекта referenceAttachment. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип контента этого вложения. Необязательное свойство.|
|id|Строка|Идентификатор вложения.  Только для чтения.|
|isFolder|Boolean|Указывает, является ли вложение ссылкой на папку. Если **sourceUrl** является ссылкой на папку, необходимо задать для этого параметра значение true. Необязательное свойство.|
|isInline|Boolean|Значение true указывает, что вложение встроено в содержимое объекта. Необязательное свойство.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Необязательное свойство.|
|name|String|Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла. Обязательно.|
|права|referenceAttachmentPermission|Задает разрешения, предоставленные для вложения, по типу поставщика в **ProviderType**. Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Необязательное свойство.|
|previewUrl|String|Применяется только к вложению ссылки на URL-адрес изображения для получения изображения предварительного просмотра. Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения. Необязательное свойство.|
|providerType|Перечислений — referenceattachmentprovider|Тип поставщика, который поддерживает вложение этого contentType. Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Необязательное свойство.|
|size|Int32|Размер метаданных в байтах, хранящихся в сообщении для вложения ссылки. Это значение не отображает фактический размер файла. Необязательное свойство.|
|sourceUrl|String|URL-адрес для получения содержимого вложения. Если это URL-адрес папки, то для правильного отображения папки в Outlook или Outlook в **Интернете установите для параметра IsTrue значение true** . Обязательно.|
|thumbnailUrl|String|Применяется только к вложению ссылки на URL-адрес изображения для получения эскиза. Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения. Необязательное свойство.|

## <a name="relationships"></a>Отношения
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
