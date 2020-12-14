---
title: Тип ресурса chat
description: Чат — это коллекция chatMessages между одним или более участниками.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dcfa853f8ba246443f0f5073a4a62fd84f92adc6
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659410"
---
# <a name="chat-resource-type"></a>Тип ресурса chat

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чат — это коллекция [chatMessages](chatmessage.md) между одним или более участниками. Участниками могут быть пользователи или приложения.

> **Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) некоторые из перечисленных методов транзитивно влияют на собрание.

## <a name="methods"></a>Методы

|  Метод       |  Возвращаемый тип  | Описание| 
|:---------------|:--------|:----------|
|[Список чатов](../api/chat-list.md) | [коллекция chat](chat.md) | Получите список чатов, в которые входит пользователь.| 
|[Получение чата](../api/chat-get.md) | [chat](chat.md) | Чтение свойств и связей чата.| 
|[Список участников чата](../api/conversationmember-list.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате.| 
|[Получить участника чата](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате.| 
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
| id| String| Уникальный идентификатор чата. Только для чтения.|
| topic| String|  (Необязательно) Тема или тема чата. Доступно только для групповых чатов.|
| createdDateTime| dateTimeOffset|  Дата и время создания чата. Только для чтения.|
| lastUpdatedDateTime| dateTimeOffset|  Дата и время переименования чата или изменения членства. lastUpdatedDateTime не обновляется при отправлении сообщения в чат. Только для чтения.|

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


