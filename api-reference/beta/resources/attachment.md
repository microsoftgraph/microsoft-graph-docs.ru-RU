---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: d1296c40bfc434262f1911c6f9453725bc033999
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137622"
---
# <a name="attachment-resource-type"></a>Тип ресурса attachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Вы можете добавить связанное содержимое к событию [пользователя,](../resources/event.md) [сообщению,](../resources/message.md)задаче [Outlook](../resources/outlooktask.md)или [записи](../resources/post.md) группы в форме вложения. 

События в календарях группы не поддерживают вложения.

Задачи Outlook не поддерживают справочные вложения.

**attachment** — базовый ресурс для следующих производных типов вложений:

* файл (ресурс [fileAttachment](../resources/fileattachment.md));
* элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));
* ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).

>**Примечание.** Размер вложенного файла или элемента не может быть меньше 4 МБ. 
>
> Однако при вложении в сообщение файла размером от 3 МБ до [](../api/attachment-createuploadsession.md) 150 МБ можно создать сеанс отправки и итеративно отправить диапазоны файла для его вложения. См. [пример вложенных больших файлов в](/graph/outlook-large-attachments) сообщения Outlook.

## <a name="methods"></a>Методы

Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение вложения](../api/attachment-get.md) | [attachment](attachment.md) |Чтение свойств, связей или необработанных содержимого вложения, вложенного в событие пользователя, сообщение, задачу Outlook или публикацию.|
|[Добавление вложения в пользовательское событие](../api/event-post-attachments.md) | [attachment](attachment.md) |Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.|
|[Добавление вложения в сообщение](../api/message-post-attachments.md) | [attachment](attachment.md) |Добавление в сообщение файла, элемента или ссылки в качестве вложения. Эта операция ограничивает размер вложения, который можно добавить, до 4 МБ.|
|[Создание сеанса для вложения большого файла](../api/attachment-createuploadsession.md)| [uploadSession](uploadsession.md) | Создайте сеанс отправки, который позволяет приложению итеративно отправлять диапазоны файла, чтобы встроить файл в указанное **сообщение.** Размер файла должен быть от 3 до 150 МБ.|
|[Добавление вложения в задачу Outlook](../api/outlooktask-post-attachments.md) (неподготовлено) | [attachment](attachment.md) |Добавление вложенного файла или элемента в задачу Outlook.|
|[Добавление вложения в запись](../api/post-post-attachments.md) | [attachment](attachment.md) |Добавление вложенного файла, элемента или ссылки в публикацию группы.|
|[Список вложений пользовательского события](../api/event-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для события в пользовательском календаре. |
|[Список вложений для сообщения](../api/message-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для сообщения. |
|[Список вложений задачи Outlook](../api/outlooktask-list-attachments.md) (неподготовлен) | Коллекция [attachment](attachment.md)  | Получите список вложений для задачи Outlook. |
|[Список вложений для записи](../api/post-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для записи. |
|[Удаление](../api/attachment-delete.md) | Нет |Удаление вложения для события, сообщения, задачи Outlook или публикации. |

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


