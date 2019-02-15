---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994470"
---
# <a name="channel-resource-type"></a>Тип ресурса channel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Канал — это коллекция объектов [chatMessages](chatmessage.md) в [команде](../resources/team.md). Канал представляет тему и логически обособляет обсуждение в команде. Примеры: канал "Пятничный обед команды" и канал "Обсуждение архитектуры".


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление каналов](../api/channel-list.md) | Коллекция [channel](channel.md) | Получение списка каналов в команде.|
|[Создание канала](../api/channel-post.md) | [channel](channel.md) | Создание нового канала путем добавления отображаемого имени и описания.|
|[Получение канала](../api/channel-get.md) | [channel](channel.md) | Чтение свойств и связей канала.|
|[Обновление канала](../api/channel-patch.md) | [channel](channel.md) | Обновление свойств канала.|
|[Удаление канала](../api/channel-delete.md) | Нет | Удаление канала.|
|[Перечисление сообщений в каналах](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в канале |
|[Отправка сообщения канала](../api/channel-post-chatmessage.md)  | [chatMessage](../resources/chatmessage.md) | [Отправка сообщения в канал](../api/channel-post-chatmessage.md) |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|String|Необязательное текстовое описание канала.|
|displayName|String|Имя канала, отображаемое для пользователя в Microsoft Teams.|
|id|String|Уникальный идентификатор канала. Только для чтения.|
|isFavoriteByDefault|Boolean|Должен ли канал автоматически помечаться как "Избранное" для всех участников команды. Значение по умолчанию: `false`.|
|email|Boolean| Адрес электронной почты для отправки сообщений в канал. Только для чтения.|
|webUrl|String|Гиперссылка, ведущая к каналу в Microsoft Teams. Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал". Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться. Только для чтения.|


## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|messages|Коллекция [chatMessage](chatmessage.md)|Коллекция всех сообщений в канале. Свойство навигации. Допускается значение null. В настоящее время этот API поддерживает чтение, но в конечном итоге будет также поддерживать написание сообщений.|
|tabs|Коллекция [teamsTab](../resources/teamstab.md)|Коллекция всех вкладок в канале. Свойство навигации.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
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
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
