---
title: Тип ресурса канала
description: 'Канал представляет коллекцию chatMessages в группе. '
ms.openlocfilehash: 90a2c6641a79829e340f2487d7f0381998d2a205
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081958"
---
# <a name="channel-resource-type"></a>Тип ресурса канала

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Канал представляет коллекцию [chatMessages](chatmessage.md) внутри [групп](../resources/team.md). Канал представляет раздел и логическая изоляции обсуждения в группе. Примеры может быть канала «Пятница Lunch группы» и «Архитектура обсуждений» канала.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список каналов](../api/channel-list.md) | Коллекция [канала](channel.md) | Получите список каналов в данной группы.|
|[Создание канала](../api/channel-post.md) | [канал](channel.md) | Создайте новый канал, включая отображаемое имя и описание.|
|[Получение канала](../api/channel-get.md) | [канал](channel.md) | Чтение свойства и связи канала.|
|[Обновление канала](../api/channel-patch.md) | [канал](channel.md) | Обновление свойств канала.|
|[Удаление канала](../api/channel-delete.md) | Нет | Удаление канала.|
|[Список сообщения](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в канале |
|[Создать поток разговора](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) коллекции| Создайте поток разговора в указанном канала.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|описание|String|Необязательное текстовое описание для канала.|
|displayName|String|Имя канала, как оно будет отображаться для пользователей в группах Майкрософт.|
|id|String|Уникальный идентификатор, каналов. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Description|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) коллекции|Коллекция всех сообщений в канале. Свойство навигации. Допускается значение null. В настоящее время этот интерфейс API только поддерживает чтение, но со временем будут поддерживать сообщения о записи слишком.|
|chatThreads|[chatThread](chatthread.md) коллекции|(Это постепенно пользу свойства сообщения) chatThreads поддерживает создание новых сообщений, но не чтение сообщений. ChatThreads — это свойство навигации, а значение NULL.|
|вкладки|[teamsTab](../resources/teamstab.md) коллекции|Коллекция всех вкладок в канале. Свойство навигации.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
