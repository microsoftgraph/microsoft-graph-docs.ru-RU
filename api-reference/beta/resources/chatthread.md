---
title: Тип ресурса chatThread
description: ChatThread — это коллекция chatMessages в группах Майкрософт.
ms.openlocfilehash: ef8f118ae4354a5e4197802708aecfa1fb6f8cb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081634"
---
# <a name="chatthread-resource-type"></a>Тип ресурса chatThread

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

ChatThread — это коллекция [chatMessages](chatmessage.md) в группах Майкрософт.

> На данный момент chatThreads может быть [создано в каналы](../api/channel-post-chatthreads.md).  Выпуски будущее API поддерживает чтения существующих chatThreads, а также чтения/записи прямого чаты между пользователями, которые являются выходят за рамки группы или канала.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание цепочки](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |Запустите новый поток в указанный канал, предоставляя первого сообщения.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Description|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| Допускается значение null.|
|chatMessages|[chatMessage](chatmessage.md) коллекции| Допускается значение null.|

> В настоящее время эти связи неявно, существует, но не может читать или записи.  Выпуски будущих бета-версии API будут поддерживать это.

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
  "id": "string (identifier)",
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
