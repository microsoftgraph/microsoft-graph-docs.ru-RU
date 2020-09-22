---
title: Тип ресурса Чатмессажеаттачмент
description: Представляет вложение для объекта сообщения чата.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: clearab
ms.openlocfilehash: 2c343d3449365d34c0bda0fd35b58e029d89711f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064313"
---
# <a name="chatmessageattachment-resource-type"></a>Тип ресурса Чатмессажеаттачмент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет вложение для объекта сообщения чата.

Сущность типа `chatMessageAttachment` возвращается в составе API [сообщений канала](../api/channel-list-messages.md) в составе объекта [chatMessage](chatmessage.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string| Только для чтения. Уникальный идентификатор вложения.|
|contentType| string | Тип мультимедиа вложенного содержимого. Он может иметь следующие значения: <br><ul><li>`reference`: Вложение — это ссылка на другой файл. Заполните contentURL ссылкой на объект.</li><li>Все типы контента, поддерживаемые [объектом приложения](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?view=azure-bot-service-4.0#attachment-object) Bot Framework</li><li>`application/vnd.microsoft.card.codesnippet`: Фрагмент кода. </li><li>`application/vnd.microsoft.card.announcement`: Заголовок извещения. </li>|
|contentUrl|string|URL-адрес содержимого вложения. Поддерживаемые протоколы: HTTP, HTTPS, File и Data.|
|содержимое|string|Содержимое вложения. Если вложение является [расширенной карточкой](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), задайте свойству объект с богатыми карточками. Это свойство и contentUrl являются взаимоисключающими.|
|name|string|Имя вложения.|
|thumbnailUrl| string |URL-адрес эскиза, который может использоваться каналом, если он поддерживается в альтернативной, меньшей форме содержимого или contentUrl. Например, если для объекта contentType задано значение Application/Word, а для параметра contentUrl задано расположение документа Word, можно включить эскиз изображения, представляющий документ. Вместо документа в канале может отображаться миниатюрное изображение. Когда пользователь щелкает изображение, канал открывает документ.|

## <a name="json-representation"></a>Представление JSON
 Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


