---
title: Тип ресурса chatThread
description: chatThread — это коллекция ресурсов chatMessages в Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399607"
---
# <a name="chatthread-resource-type"></a>Тип ресурса chatThread

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

chatThread — это коллекция ресурсов [chatMessages](chatmessage.md) в Microsoft Teams.

> В настоящее время chatThreads можно [создавать в каналах](../api/channel-post-chatthreads.md).  Будущие выпуски API будут поддерживать чтение существующих chatThreads, а также чтение и запись прямых чатов между пользователями за пределами группы или канала.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание цепочки](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |Начало новой цепочки беседы в указанном канале путем предоставления первого сообщения.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| Допускается значение null.|
|chatMessages|Коллекция [chatMessage](chatmessage.md)| Допускается значение null.|

> В настоящее время эти отношения неявно существуют, но их нельзя прочитать или записать.  Эта возможность появится в будущих бета-выпусках API.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
