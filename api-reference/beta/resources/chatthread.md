---
title: Тип ресурса chatThread
description: chatThread — это коллекция ресурсов chatMessages в Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521343"
---
# <a name="chatthread-resource-type"></a>Тип ресурса chatThread

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
