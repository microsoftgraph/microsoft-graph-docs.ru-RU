---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 6c062ac3e832c2ce0385c4851330d5320ca34af9
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849501"
---
# <a name="attachment-resource-type"></a>Тип ресурса attachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Вы можете добавить связанное [message](../resources/message.md)содержимое в [события пользователя, сообщение,](../resources/event.md) [задачу Outlook или](../resources/outlooktask.md)запись в группе [в](../resources/post.md) виде вложения. 

События в календарях группы не поддерживают вложения.

Задачи Outlook не поддерживают ссылочные вложения.

**attachment** — базовый ресурс для следующих производных типов вложений:

* файл (ресурс [fileAttachment](../resources/fileattachment.md));
* элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));
* ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).

>**Примечание.** Существует ограничение размера файла или вложенного элемента, который можно добавить не более 4 МБ. 
>
> Но если в сообщение вкладывается файл размером от 3 до 150 МБ, [вы](../api/attachment-createuploadsession.md) можете создать сеанс отправки и итеративно отправлять диапазоны файла, чтобы вложить его. Пример [см. в разделе, посвященный крупных файлам](/graph/outlook-large-attachments) outlook, вложенные в сообщения Outlook.

## <a name="methods"></a>Методы

Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение вложения](../api/attachment-get.md) | [attachment](attachment.md) |Чтение свойств, связей или необработанного содержимого объекта, которое было вложено к пользовательскому событию, сообщению, задаче Outlook или записи.|
|[Добавление вложения в пользовательское событие](../api/event-post-attachments.md) | [attachment](attachment.md) |Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.|
|[Добавление вложения в сообщение](../api/message-post-attachments.md) | [attachment](attachment.md) |Добавление в сообщение файла, элемента или ссылки в качестве вложения. Эта операция ограничивает размер добавляемого вложения в размере не более 4 МБ.|
|[Создание сеанса для вложения большого файла](../api/attachment-createuploadsession.md)| [uploadSession](uploadsession.md) | Создать сеанс отправки, позволяющий приложению выполнять итеративную отправку диапазонов файла, например, вложенный файл в указанное **сообщение.** Размер файла должен быть от 3 до 150 МБ.|
|[Добавление вложения в задачу Outlook](../api/outlooktask-post-attachments.md) | [attachment](attachment.md) |Добавление вложенного файла или элемента в задачу Outlook.|
|[Добавление вложения в запись](../api/post-post-attachments.md) | [attachment](attachment.md) |Добавление в запись группы файла, элемента или ссылки в качестве вложения.|
|[Список вложений пользовательского события](../api/event-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для события в пользовательском календаре. |
|[Список вложений для сообщения](../api/message-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для сообщения. |
|[Список вложений задачи Outlook](../api/outlooktask-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для задачи Outlook. |
|[Список вложений для записи](../api/post-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для записи. |
|[Удаление](../api/attachment-delete.md) | Нет |Удаление объекта, прикрепка к сообщению, задаче Outlook или записи для события. |

## <a name="properties"></a>Свойства

Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип MIME.|
|id|String| Только для чтения.|
|isInline|Boolean|Значение `true`, если вложение является встроенным. В противном случае — значение `false`.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|имя|String|Отображаемое имя вложения. Он может не быть фактическим именем файла.|
|size|Int32|Размер вложения в байтах.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
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
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
