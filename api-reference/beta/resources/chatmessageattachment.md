---
title: Тип ресурса chatMessageAttachment
description: Представляет вложение в сущность сообщения чата.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: caf7d1693395d9272a8999910dcaa29a9bef11da
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060760"
---
# <a name="chatmessageattachment-resource-type"></a>Тип ресурса chatMessageAttachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет вложение в сущность сообщения чата.

Сущность типа возвращается `chatMessageAttachment` как [часть API](../api/channel-list-messages.md) получения сообщений канала в составе сущности [chatMessage](chatmessage.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string| Только для чтения. Уникальный идентификатор вложения.|
|contentType| string | Тип носителя вложения контента. Он может иметь следующие значения: <br><ul><li>`reference`: вложение — это ссылка на другой файл. Заполните contentURL ссылкой на объект.</li><li>Любые contentTypes, поддерживаемые объектом [Attachment Bot Framework](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)</li><li>`application/vnd.microsoft.card.codesnippet`: фрагмент кода. </li><li>`application/vnd.microsoft.card.announcement`: заголовок объявления. </li>|
|contentUrl|string|URL-адрес содержимого вложения. Поддерживаемые протоколы: HTTP, HTTPS, файл и данные.|
|содержимое|string|Содержимое вложения. Если вложение является форматированным [карточкой](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), задайте для свойства объект форматированного карточки. Это свойство и contentUrl являются взаимоисключающими.|
|name|string|Имя вложения.|
|teamsAppId| string |Идентификатор приложения Teams, связанного с вложением. Это свойство используется специально для атрибута Teams сообщений указанному приложению.|
|thumbnailUrl| string |URL-адрес эскиза, который канал может использовать, если он поддерживает использование альтернативной, меньшей формы содержимого или contentUrl. Например, если задать contentType для приложения или слова и задать contentUrl для расположения документа Word, можно включить эскиз изображения, представляющего документ. Вместо документа в канале может отображаться эскиз. Когда пользователь щелкает изображение, канал открывает документ.|


## <a name="json-representation"></a>Представление JSON
 Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl",
    "teamsAppId"
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
  "teamsAppId": "string",
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


