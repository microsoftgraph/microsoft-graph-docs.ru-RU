---
title: Тип ресурса канала
description: 'Канал представляет коллекцию сообщений в группе. '
author: nkramer
ms.openlocfilehash: f9ab71213180732a0c8c626d5b32b9074bd135d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337088"
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
