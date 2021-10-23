---
title: Тип ресурса чата
description: Чат — это коллекция chatMessages между одним или более участниками.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 82d7cfa6a4e966c7264be12fe23893c9cce2a8ef
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560109"
---
# <a name="chat-resource-type"></a>Тип ресурса чата

Пространство имен: microsoft.graph

Чат — это коллекция [chatMessages](chatmessage.md) между одним или более участниками. Участниками могут быть пользователи или приложения.

> **Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) то некоторые из перечисленных методов будут транзитно влиять на собрание.

## <a name="methods"></a>Методы

|  Метод       |  Возвращаемый тип  | Описание| 
|:---------------|:--------|:----------|
| **Управление чатом** |||
|[Создание чата](../api/chat-post.md) | [chat](chat.md) | Создайте новый чат.| 
|[Получение чата](../api/chat-get.md) | [chat](chat.md) | Чтение свойств и связей чата.| 
|[Обновление чата](../api/chat-patch.md) | [chat](chat.md) | Обновление свойств чата.|
|[Перечисление участников чата](../api/chat-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате.| 
|[Добавление участника в чат](../api/chat-post-members.md) | Заголовок размещения | Добавление пользователя в чат.| 
|[Получение участника чата](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате.| 
|[Удаление участника чата](../api/chat-delete-members.md)|Нет|Удалите пользователя из чата.|
|[Общение в чате между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Получите один-на-один чат между пользователем и приложением |
| **Сообщения** |||
|[Список сообщений в чате](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Получать сообщения в чате. | 
|[Получение сообщения в чате](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения в чате. | 
|[Получение сообщений во всех чатах для пользователя](../api/chats-getallmessages.md)| [коллекция чатов](chat.md)| Получение сообщений из всех чатах, в которых пользователь является участником. |
| **Приложения** |||
|[Список приложений в каталоге](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) collection | Список приложений, установленных в чате (и связанном собрании).|
|[Получить приложение в чате](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Получите определенное приложение, установленное в чате (и связанное собрание).|
|[Добавление приложения в чате](../api/chat-post-installedapps.md) | | Добавление (установка) приложения в чате (и связанное собрание).|
|[Обновление приложения в чате](../api/chat-teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения, установленного в чате (и связанного собрания).|
|[Удалить приложение из чата](../api/chat-delete-installedapps.md) | Нет | Удалить (удалить) приложение из чата (и связанного собрания).|
| **Вкладки** |||
|[Список вкладок в чате](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Вкладки списка, закрепленные в чате (и связанное собрание).|
|[Получить вкладку в чате](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Получите определенную вкладку, закрепленную в чате (и связанное собрание).|
|[Добавление вкладки в чат](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Добавьте (пин-код) вкладку в чат (и связанное собрание).|
|[Обновление вкладки в чате](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки в чате (и связанное собрание).|
|[Удаление вкладки из чата](../api/chat-delete-tabs.md) | Нет | Удалите (открепите) вкладку из чата (и связанного собрания).|

>**Примечание:** При использовании разрешений приложений убедитесь, что вы знаете, как получить ID чата. Так как чаты с разрешениями приложений не поддерживаются, возможны не все сценарии. Можно получить ID чата с делегированными разрешениями, а также из уведомлений об изменении [для /chats/getAllMessages](../api/subscription-post-subscriptions.md) с разрешениями приложений.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
| chatType| [chatType](../resources/chat.md#chattype-values) | Указывает тип чата. Возможные значения: `group`, `oneOnOne`, `meeting`, `unknownFutureValue`.|
| createdDateTime| dateTimeOffset|  Дата и время создания чата. Только для чтения.|
| id| Строка| Уникальный идентификатор чата. Только для чтения.|
| lastUpdatedDateTime| dateTimeOffset|  Дата и время переименования чата или списка участников были изменены в последний раз. Только для чтения.|
| topic| String|  (Необязательный) Тема или тема для чата. Доступно только для групповых чатов.|


### <a name="chattype-values"></a>значения chatType 

| Элемент             | Значение | Описание               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | Указывает, что чат — это чат 1:1. Размер реестра фиксирован для этого типа чата; не могут быть удалены или добавлены.|
|group;               | 1     | Указывает, что чат — это групповой чат. Размер реестра (не менее двух человек) может быть обновлен для этого типа чата. Участники могут быть удалены или добавлены позже.|
|собрание             | 2     | Указывает, что чат связан с собранием в Интернете. Этот тип чата создается только в рамках создания собрания в Интернете.|
|unknownFutureValue  | 3     | Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) collection | Коллекция всех приложений в чате. Допускается значение null. |
| members | Коллекция [conversationMember](conversationmember.md) | Коллекция всех участников в чате. Допускается значение null. |
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


