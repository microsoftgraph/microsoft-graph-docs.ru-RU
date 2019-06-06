---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8b284cdfef42e9eb3319fc51c17febcf02eba1a1
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709434"
---
# <a name="channel-resource-type"></a>Тип ресурса channel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками. Каждый канал предназначен для определенной темы, отдела или проекта.
Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление каналов](../api/channel-list.md) | Коллекция [channel](channel.md) | Получение списка каналов в команде.|
|[Создание канала](../api/channel-post.md) | [channel](channel.md) | Создание нового канала путем добавления отображаемого имени и описания.|
|[Получение канала](../api/channel-get.md) | [channel](channel.md) | Чтение свойств и связей канала.|
|[Обновление канала](../api/channel-patch.md) | [channel](channel.md) | Обновление свойств канала.|
|[Удаление канала](../api/channel-delete.md) | Нет | Удаление канала.|
|[Перечисление сообщений в каналах](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в канале |
|[Создание объекта chatMessage в канале](../api/channel-post-messages.md) | [chatMessage](../resources/chatmessage.md) | Отправка сообщения в канал. |
|[Создание ответа на chatMessage в канале](../api/channel-post-messagereply.md) | [chatMessage](../resources/chatmessage.md) | Ответ на сообщение в канале.|
|[Перечисление вкладок](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных в канале.|
|[Получение вкладки](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Чтение вкладок, закрепленных в канале.|
|[Добавление вкладки](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки в канал.|
|[Удаление вкладки](../api/teamstab-delete.md) | Нет | Удаление (открепление) вкладки из канала.|
|[Обновление вкладки](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки.|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|String|Необязательное текстовое описание канала.|
|displayName|String|Имя канала, отображаемое для пользователя в Microsoft Teams.|
|id|String|Уникальный идентификатор канала. Только для чтения.|
|isFavoriteByDefault|Boolean|Должен ли канал автоматически помечаться как "Избранное" для всех участников команды. Значение по умолчанию: `false`.|
|email|String| Адрес электронной почты для отправки сообщений в канал. Только для чтения.|
|webUrl|String|Гиперссылка, ведущая к каналу в Microsoft Teams. Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал". Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться. Только для чтения.|


## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
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
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string"
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
  "suppressions": []
}
-->
