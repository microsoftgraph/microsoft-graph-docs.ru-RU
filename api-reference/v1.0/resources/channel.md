---
title: Тип ресурса канала
description: 'Канал представляет коллекцию сообщений в группе. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: f513a0c8de51cdfb8ca692098cab403dd74d747a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986350"
---
# <a name="channel-resource-type"></a>Тип ресурса канала



Канал представляет коллекцию сообщений в пределах [группы](../resources/team.md). Канал представляет раздел и логическая изоляции обсуждения в группе. Примеры может быть канала «Пятница Lunch группы» и «Архитектура обсуждений» канала.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список каналов](../api/channel-list.md) | Коллекция [канала](channel.md) | Получите список каналов в данной группы.|
|[Создание канала](../api/channel-post.md) | [канал](channel.md) | Создайте новый канал, включая отображаемое имя и описание.|
|[Получение канала](../api/channel-get.md) | [канал](channel.md) | Чтение свойства и связи канала.|
|[Обновление канала](../api/channel-patch.md) | [канал](channel.md) | Обновление свойств канала.|
|[Удаление канала](../api/channel-delete.md) | Нет | Удаление канала.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|описание|Строка|Необязательное текстовое описание для канала.|
|displayName|Строка|Имя канала, как оно будет отображаться для пользователей в группах Майкрософт.|
|id|Строка|Уникальный идентификатор, каналов. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
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
