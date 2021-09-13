---
title: тип ресурса chatMessageAttachment
description: Представляет вложение в объект сообщения чата.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: 1b02a5c034be39ee9eeb941b7fe875e8d4c9e8c1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094417"
---
# <a name="chatmessageattachment-resource-type"></a>тип ресурса chatMessageAttachment

Пространство имен: microsoft.graph

Представляет вложение в объект сообщения чата.

Объект типа возвращается в рамках API сообщений get channel, как часть `chatMessageAttachment` [сущности chatMessage.](chatmessage.md) [](../api/channel-list-messages.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string| Только для чтения. Уникальный id вложения.|
|contentType| string | Тип мультимедиа вложения контента. Он может иметь следующие значения: <br><ul><li>`reference`: Вложение — это ссылка на другой файл. Заполнять contentURL ссылкой на объект.</li><li>Любые contentTypes, поддерживаемые [](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object) объектом вложения Bot Framework</li><li>`application/vnd.microsoft.card.codesnippet`. Фрагмент кода. </li><li>`application/vnd.microsoft.card.announcement`: Заглавная ведерка объявления. </li>|
|contentUrl|string|URL-адрес для содержимого вложения. Поддерживаемые протоколы: http, https, file и data.|
|содержимое|string|Содержимое вложения. Если вложение является [богатой картой,](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference)установите свойство объекту богатой карты. Это свойство и contentUrl являются взаимоисключающими.|
|name|string|Имя вложения.|
|thumbnailUrl| string |URL-адрес изображения эскиза, который канал может использовать, если поддерживает использование альтернативной, более мелкой формы контента или contentUrl. Например, если вы установите contentType для приложения/слова и установите contentUrl к расположению документа Word, вы можете включить эскизное изображение, которое представляет документ. Канал может отображать изображение эскиза вместо документа. Когда пользователь щелкает изображение, канал откроет документ.|

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

