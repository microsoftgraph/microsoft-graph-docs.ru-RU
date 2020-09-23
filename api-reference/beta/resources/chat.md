---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da9dcf4a1777d23a3b5f4b73e505641057558605
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222836"
---
# <a name="chat-resource-type"></a>Тип ресурса Chat

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками. Участники могут быть пользователями или приложениями.

## <a name="methods"></a>Методы

|  Метод       |  Возвращаемый тип  | Описание| Разрешения |
|:---------------|:--------|:----------|-----------|
|[Список чатов](../api/chat-list.md) | Коллекция [чата](chat.md) | Получение списка сеансов, в которые входит пользователь.| **Только делегированные** |
|[Получение чата](../api/chat-get.md) | [chat](chat.md) | Чтение свойств и связей чата.| **Только делегированные** |
|[Список членов чата](../api/conversationmember-list.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате.| Делегирование и приложение * |
|[Получение члена чата](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате.| Делегирование и приложение * |
|[Список сообщений в чате](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в индивидуальном или групповом чате. | Делегирование и приложение * |
|[Получение сообщения в чате](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения в чате. | Делегирование и приложение * |

>**Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата. Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны. Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/жеталлмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
| id| String| Уникальный идентификатор чата. Только для чтения.|
| topic| String|  Необязательно Тема или тема чата. Доступно только для чатов групп.|
| createdDateTime| dateTimeOffset|  Дата и время создания чата. Только для чтения.|
| lastUpdatedDateTime| dateTimeOffset|  Дата и время переименования чата или изменения членства. Ластупдатеддатетиме не обновляется при отправке сообщения в чат. Только для чтения.|

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) collection | Коллекция всех приложений в чате. Допускается значение null. |
| members | Коллекция [conversationMember](conversationmember.md) | Коллекция всех людей в чате. Допускается значение null. |
| messages | Коллекция [chatMessage](chatmessage.md) | Коллекция всех сообщений в чате. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset"
}
```

## <a name="see-also"></a>См. также

- [channel](channel.md)
- [chatMessage](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->


