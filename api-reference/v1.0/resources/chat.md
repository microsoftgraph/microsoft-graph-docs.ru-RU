---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f9cc43442e077dfe245fa8422b954859bf1c569
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564128"
---
# <a name="chat-resource-type"></a>Тип ресурса Chat

Пространство имен: microsoft.graph

Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками. Участники могут быть пользователями или приложениями.

## <a name="methods"></a>Методы

|  Метод       |  Возвращаемый тип  | Описание|
|:---------------|:--------|:----------|
|[Получение разговора между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Получение одного сеанса разговора между пользователем и приложением | 

>**Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата. Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны. Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/жеталлмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
| id| String| Уникальный идентификатор чата. Только для чтения.|


## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
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


