---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1745f987577d94f14f81d79a9f8afb89c1ab793
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606939"
---
# <a name="chat-resource-type"></a>Тип ресурса Chat

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками. Участники могут быть пользователями или приложениями.

## <a name="methods"></a>Методы

|  Метод       |  Возвращаемый тип  | Описание| 
|:---------------|:--------|:----------|
|[Список чатов](../api/chat-list.md) | Коллекция [чата](chat.md) | Получение списка сеансов, в которые входит пользователь.| 
|[Получение чата](../api/chat-get.md) | [chat](chat.md) | Чтение свойств и связей чата.| 
|[Список членов чата](../api/conversationmember-list.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате.| 
|[Получение члена чата](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате.| 
|[Список сообщений в чате](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в индивидуальном или групповом чате. | 
|[Получение сообщения в чате](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения в чате. | 
|[Получение разговора между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Получение одного сеанса разговора между пользователем и приложением |
|[Получение всех сообщений чата](../api/chats-getallmessages.md)| Коллекция [чата](chat.md)| Получение сообщений от всех чатов, в которых пользователь является участником, в том числе беседы в одном месте, групповых чатов и сеансов собраний. |
|[Перечисление приложений в чате](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) collection | Список приложений, установленных в чате.|
|[Получение приложения в чате](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Получение определенного приложения, установленного в чате.|
|[Добавление приложения в чат](../api/chat-post-installedapps.md) | | Добавляет (устанавливает) приложение в чат.|
|[Обновление приложения в чате](../api/chat-teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения, установленного в чате.|
|[Удаление приложения из чата](../api/chat-delete-installedapps.md) | Нет | Удаление (удаление) приложения из чата.|
|[Список вкладок в чате](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Список вкладок, закрепленных в чате.|
|[Получение вкладки в чате](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Получение определенной вкладки, закрепленной в чате.|
|[Добавление вкладки в чат](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Добавление вкладки в чат (ПИН-код).|
|[Вкладка "обновление" в чате](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Обновляет свойства вкладки в чате.|
|[Удаление вкладки из чата](../api/chat-delete-tabs.md) | Нет | Удаление (открепление) вкладки из чата.|

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


