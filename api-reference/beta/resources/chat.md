---
title: Тип ресурса chat
description: Чат — это коллекция chatMessages между одним или более участниками.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a5fefdff40c60951c07d26df2962fbba1249a16
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714321"
---
# <a name="chat-resource-type"></a>Тип ресурса chat

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чат — это коллекция [chatMessages](chatmessage.md) между одним или более участниками. Участниками могут быть пользователи или приложения.

> **Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) некоторые из указанных методов будут транзитивно влиять на собрание.

## <a name="methods"></a>Методы

|  Метод       |  Возвращаемый тип  | Описание| 
|:---------------|:--------|:----------|
|[Список чатов](../api/chat-list.md) | [коллекция chat](chat.md) | Получите список чатов, в которые входит пользователь.| 
|[Создание чата](../api/chat-post.md) | [chat](chat.md) | Создайте новый чат.| 
|[Получение чата](../api/chat-get.md) | [chat](chat.md) | Чтение свойств и связей чата.| 
|[Перечисление участников чата](../api/chat-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате.| 
|[Добавление участника в чат](../api/chat-post-members.md) | Заголовок размещения | Добавление пользователя в чат.| 
|[Получение участника чата](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате.| 
|[Удаление участника чата](../api/chat-delete-members.md)|Нет|Удаление пользователя из чата.|
|[Список сообщений в чате](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в индивидуальном или групповом чате. | 
|[Получение сообщения в чате](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения в чате. | 
|[Общение в чате между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Как получить один-на-один чат между пользователем и приложением |
|[Получить все сообщения чата](../api/chats-getallmessages.md)| [коллекция chat](chat.md)| Получать сообщения из всех чатов, в которых состоит пользователь, включая чаты с одним пользователем, групповые чаты и чаты собраний. |
|[Список приложений в каталоге](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) collection | Список приложений, установленных в чате (и связанном собрании).|
|[Получить приложение в чате](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Получите определенное приложение, установленное в чате (и связанном собрании).|
|[Добавление приложения в чате](../api/chat-post-installedapps.md) | | Добавление (установка) приложения в чате (и связанном собрании).|
|[Обновление приложения в чате](../api/chat-teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения, установленного в чате (и связанном собрании).|
|[Удалить приложение из чата](../api/chat-delete-installedapps.md) | Нет | Удаление приложения из чата (и связанного собрания).|
|[Список вкладок в чате](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Список вкладок, закрепленных в чате (и связанном собрании).|
|[Получить вкладку в чате](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Получить определенную вкладку, закрепленную в чате (и связанном собрании).|
|[Добавление вкладки в чат](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки в чат (и связанное собрание).|
|[Вкладка "Обновление" в чате](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки в чате (и связанном собрании).|
|[Удаление вкладки из чата](../api/chat-delete-tabs.md) | Нет | Удалите (открепите) вкладку из чата (и связанного собрания).|

>**Примечание.** При использовании разрешений приложения убедитесь, что вы знаете, как получить ИД чата. Так как перечисление чатов с разрешениями приложения не поддерживается, не все сценарии возможны. Можно получить ИД чата с делегными разрешениями и из уведомлений об изменениях [для /chats/getAllMessages с](../api/subscription-post-subscriptions.md) разрешениями приложения.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
| id| Строка| Уникальный идентификатор чата. Только для чтения.|
| topic| String|  (Необязательно) Тема или тема чата. Доступно только для групповых чатов.|
| createdDateTime| dateTimeOffset|  Дата и время создания чата. Только для чтения.|
| lastUpdatedDateTime| dateTimeOffset|  Дата и время переименования чата или последнего изменения списка участников. Только для чтения.|
| chatType| [chatType](../resources/chat.md#chattype-values) | Указывает тип чата. Возможные значения: `group` и `oneOnOne` `meeting` .|

### <a name="chattype-values"></a>значения chatType 

| Элемент             | Значение | Описание               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | Указывает, что чат является чатом 1:1. Размер составов для этого типа чата фиксирован; нельзя удалить или добавить члены;|
|group               | 1     | Указывает, что чат является групповым чатом. Для этого типа чата можно обновить размер группы (не менее двух человек). Члены можно удалить или добавить позже.|
|meeting             | 2     | Указывает, что чат связан с собранием по сети. Этот тип чата создается только при создании собрания по сети.|
|unknownFutureValue  | 3     | Значение Sentinel, чтобы указать будущие значения. |

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) collection | Коллекция всех приложений в чате. Допускается значение null. |
| members | Коллекция [conversationMember](conversationmember.md) | Коллекция всех участников чата. Допускается значение null. |
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
  "lastUpdatedDateTime": "dateTimeOffset",
  "chatType": "String"
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


