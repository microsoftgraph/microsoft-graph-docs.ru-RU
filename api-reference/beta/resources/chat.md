---
title: Тип ресурса чата
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f38b797c18c315e6053d285ce0c2485cd44218aa
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690011"
---
# <a name="chat-resource-type"></a>Тип ресурса чата

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чат — это коллекция [chatMessages между](chatmessage.md) одним или несколькими участниками. Участники могут быть пользователями или приложениями.

> **Примечание**. Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md) , некоторые из перечисленных методов будут транзитивно влиять на собрание.

## <a name="methods"></a>Методы

|  Метод       |  Возвращаемый тип  | Описание| 
|:---------------|:--------|:----------|
| **Управление чатом** |||
|[Перечисление чатов](../api/chat-list.md) | [коллекция чатов](chat.md) | Получение списка чатов, в которые входит пользователь.| 
|[Создание чата](../api/chat-post.md) | [chat](chat.md) | Создайте чат.| 
|[Получение чата](../api/chat-get.md) | [chat](chat.md) | Чтение свойств и связей чата.| 
|[Обновление чата](../api/chat-patch.md) | [chat](chat.md) | Обновление свойств чата.|
|[Перечисление участников чата](../api/chat-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате.| 
|[Добавление участника в чат](../api/chat-post-members.md) | Заголовок размещения | Добавьте пользователя в чат.| 
|[Получение участника чата](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате.| 
|[Удаление участника чата](../api/chat-delete-members.md)|Нет|Удалите пользователя из чата.|
|[Общение в чате между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Получите чат "один к одному" между пользователем и приложением.|
|[Пометка чата как прочитаного](../api/chat-markchatreadforuser.md) |Нет| Пометьте чат как чтение для пользователя.|
|[Пометка чата как непрочитанного](../api/chat-markchatunreadforuser.md) |Нет| Пометьте чат как непрочитанные для пользователя.|
|[Скрытие чата](../api/chat-hideforuser.md)|Нет|Скрытие чата для пользователя.|
|[Отобразить чат](../api/chat-unhideforuser.md)|Нет|Отобразить чат для пользователя.|
| **Сообщения** |||
|[Вывод списка сообщений в чате](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в чате. | 
|[Получение сообщения в чате](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения в чате. | 
|[Получение сообщений во всех чатах для пользователя](../api/chats-getallmessages.md)| [коллекция чатов](chat.md)| Получение сообщений из всех чатах, в которых пользователь является участником. |
| **Приложения** |||
|[Список приложений в каталоге](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) collection | Список приложений, установленных в чате (и связанном собрании).|
|[Получение приложения в чате](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Получение определенного приложения, установленного в чате (и связанном собрании).|
|[Добавление приложения в чате](../api/chat-post-installedapps.md) | | Добавление (установка) приложения в чате (и связанном собрании).|
|[Обновление приложения в чате](../api/chat-teamsappinstallation-upgrade.md) | Нет | Обновите приложение до последней версии, установленной в чате (и связанном собрании).|
|[Удаление приложения из чата](../api/chat-delete-installedapps.md) | Нет | Удаление приложения из чата (и связанного собрания).|
|[Перечисление предоставленных разрешений](../api/chat-list-permissiongrants.md) | Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, предоставленных приложениям в этом чате.|
| **Вкладки** |||
|[Перечисление вкладок в чате](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Список вкладок, закрепленных в чате (и связанном собрании).|
|[Вкладка "Получить" в чате](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Получение определенной вкладки, закрепленной в чате (и связанном собрании).|
|[Добавление вкладки в чат](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Добавьте (закрепите) вкладку в чат (и связанное собрание).|
|[Вкладка "Обновление" в чате](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки в чате (и связанного собрания).|
|[Удаление вкладки из чата](../api/chat-delete-tabs.md) | Нет | Удалите (открепите) вкладку из чата (и связанного собрания).|
| **Операции** |||
|[Перечисление операций в чате](../api/chat-list-operations.md) | Коллекция [teamsAsyncOperation](teamsAsyncOperation.md) | Получение списка асинхронных операций, которые выполнялись или выполнялись в чате.|
|[Получение операции в чате](../api/teamsasyncoperation-get.md#example-get-operation-on-chat) | [teamsAsyncOperation](teamsAsyncOperation.md) | Получение одной асинхронной операции, которая выполнялась или выполнялась в чате.|
| **Закрепленные сообщения** |||
|[Вывод списка закрепленных сообщений](../api/chat-list-pinnedmessages.md)|[Коллекция pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|Получение списка закрепленных сообщений в чате.|
|[Закрепление сообщения](../api/chat-post-pinnedmessages.md)|[pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|Закрепите сообщение чата в чате.|
|[Открепление сообщения](../api/chat-delete-pinnedmessages.md)|Нет|Открепите сообщение из чата.|

>**Примечание:** При использовании разрешений приложения убедитесь, что знаете, как получить идентификатор чата. Так как перечисление чатов с разрешениями приложения не поддерживается, возможны не все сценарии. Можно получить идентификаторы чата с делегированными разрешениями, а также из уведомлений об изменениях [для /chats/getAllMessages](../api/subscription-post-subscriptions.md) с разрешениями приложения.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
| chatType| [chatType](../resources/chat.md#chattype-values) | Указывает тип чата. Возможные значения: `group`, `oneOnOne`, `meeting`, `unknownFutureValue`.|
| createdDateTime| dateTimeOffset|  Дата и время создания чата. Только для чтения.|
| id| Строка| Уникальный идентификатор чата. Только для чтения.|
| lastUpdatedDateTime| dateTimeOffset|  Дата и время последнего переименования чата или списка участников. Только для чтения.|
| onlineMeetingInfo | [teamworkOnlineMeetingInfo](../resources/teamworkonlinemeetinginfo.md) | Представляет сведения о собрании по сети. Если чат не связан с собранием по сети, свойство будет пустым. Только для чтения.|
| tenantId| String | Идентификатор клиента, в котором был создан чат. Только для чтения.|
| topic| String|  (Необязательно) Тема или раздел для чата. Доступно только для групповых чатов.|
| Точки обзора|[chatViewpoint](../resources/chatviewpoint.md)|Представляет сведения о чате, относящиеся к вызываемой стороне, например дату и время чтения последнего сообщения. Это свойство заполняется только в том случае, если запрос выполняется в делегированном контексте.|
| webUrl| String | URL-адрес чата в Microsoft Teams. URL-адрес должен рассматриваться как непрозрачный большой двоичный объект, а не анализироваться. Только для чтения.|


### <a name="chattype-values"></a>Значения chatType 

| Элемент             | Значение | Описание               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | Указывает, что чат является чатом 1:1. Размер реестра для этого типа чата фиксирован. невозможно удалить или добавить элементы.|
|group               | 1     | Указывает, что чат является групповым чатом. Для этого типа чата можно изменить размер реестра (не менее двух человек). Члены можно удалить или добавить позже.|
|Конференц             | 2     | Указывает, что чат связан с собранием по сети. Этот тип чата создается только при создании собрания по сети.|
|unknownFutureValue  | 3     | Значение sentinel для развиваемого перечисления. Не следует использовать. |

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) collection | Коллекция всех приложений в чате. Допускается значение null. |
| lastMessagePreview | [chatMessageInfo](chatmessageinfo.md)| Предварительный просмотр последнего сообщения, отправленного в чате. Значение NULL, если сообщения не были отправлены в чате. В настоящее время [это свойство поддерживается](../api/chat-list.md) только операцией чатов списка.|
| members | Коллекция [conversationMember](conversationmember.md) | Коллекция всех участников чата. Допускается значение null. |
| messages | Коллекция [chatMessage](chatmessage.md) | Коллекция всех сообщений в чате. Допускается значение null. |
| operations | Коллекция [teamsAsyncOperation](teamsasyncoperation.md) | Коллекция всех асинхронных операций Teams, которые выполнялись или выполнялись в чате. Допускается значение null. |
| permissionGrants| Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)| Коллекция разрешений, предоставленных приложениям для чата.|
| pinnedMessages | [Коллекция pinnedChatMessageInfo](pinnedchatmessageinfo.md) | Коллекция всех закрепленных сообщений в чате. Допускается значение null. |
| tabs | Коллекция [teamsTab](teamstab.md) | Коллекция всех вкладок в чате. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
  "chatType": "string",
  "webUrl": "string",
  "tenantId": "string",
  "viewpoint": {
    "@odata.type": "microsoft.graph.chatViewpoint"
  },
  "onlineMeetingInfo": {
    "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
  }
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


