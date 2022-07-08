---
title: Тип ресурса чата
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5b77dc1d29107204172f3fd79ba9ae2a12d320bc
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66689988"
---
# <a name="chat-resource-type"></a>Тип ресурса чата

Пространство имен: microsoft.graph

Чат — это коллекция [chatMessages между](chatmessage.md) одним или несколькими участниками. Участники могут быть пользователями или приложениями.

> **Примечание**. Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md) , некоторые из перечисленных методов будут транзитивно влиять на собрание.

## <a name="methods"></a>Методы

|  Метод       |  Возвращаемый тип  | Описание| 
|:---------------|:--------|:----------|
| **Управление чатом** |||
|[Создание чата](../api/chat-post.md) | [chat](chat.md) | Создайте чат.| 
|[Получение чата](../api/chat-get.md) | [chat](chat.md) | Чтение свойств и связей чата.| 
|[Обновление чата](../api/chat-patch.md) | [chat](chat.md) | Обновление свойств чата.|
|[Перечисление участников чата](../api/chat-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате.| 
|[Добавление участника в чат](../api/chat-post-members.md) | Заголовок размещения | Добавьте пользователя в чат.| 
|[Получение участника чата](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате.| 
|[Удаление участника чата](../api/chat-delete-members.md)|Нет|Удалите пользователя из чата.|
|[Общение в чате между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Получение единого чата между пользователем и приложением |
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
| **Вкладки** |||
|[Перечисление вкладок в чате](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Список вкладок, закрепленных в чате (и связанном собрании).|
|[Вкладка "Получить" в чате](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Получение определенной вкладки, закрепленной в чате (и связанном собрании).|
|[Добавление вкладки в чат](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Добавьте (закрепите) вкладку в чат (и связанное собрание).|
|[Вкладка "Обновление" в чате](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки в чате (и связанного собрания).|
|[Удаление вкладки из чата](../api/chat-delete-tabs.md) | Нет | Удалите (открепите) вкладку из чата (и связанного собрания).|

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
| webUrl | String| URL-адрес чата в Microsoft Teams. URL-адрес должен рассматриваться как непрозрачный большой двоичный объект, а не анализироваться. Только для чтения. |

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
| members | Коллекция [conversationMember](conversationmember.md) | Коллекция всех участников чата. Допускается значение null. |
| messages | Коллекция [chatMessage](chatmessage.md) | Коллекция всех сообщений в чате. Допускается значение null. |
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


