---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 59a6b111c08b6bfb408b1f28b4db343843ed12ad
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932586"
---
# <a name="channel-resource-type"></a>Тип ресурса channel

Пространство имен: microsoft.graph

[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками. Каждый канал предназначен для определенной темы, отдела или проекта. Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление каналов](../api/channel-list.md) | Коллекция [channel](channel.md) | Получение списка каналов в команде.|
|[Создание канала](../api/channel-post.md) | [channel](channel.md) | Создание нового канала путем добавления отображаемого имени и описания.|
|[Получение канала](../api/channel-get.md) | [channel](channel.md) | Чтение свойств и связей канала.|
|[Обновление канала](../api/channel-patch.md) | [channel](channel.md) | Обновление свойств канала.|
|[Удаление канала](../api/channel-delete.md) | Нет | Удаление канала.|
|[Получение дельты сообщения](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Получение добавочных сообщений в канале. |
|[Перечисление сообщений в каналах](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в канале |
|[Перечисление участников канала](../api/conversationmember-list.md)| Коллекция [conversationMember](conversationmember.md)| Получение списка участников канала. |
|[Получение участника канала](../api/conversationmember-get.md)| [conversationMember](conversationmember.md)| Получение участника канала. |
|[Добавление участника канала](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| Добавление участника в канал. Поддерживается, только если параметру `channelType` присвоено значение `private`.|
|[Обновление участника канала](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| Обновление участника канала. Поддерживается, только если параметру `channelType` присвоено значение `private`.|
|[Удаление участника канала](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| Удаление участника канала. Поддерживается, только если параметру `channelType` присвоено значение `private`.|
|[Создание объекта chatMessage в канале](../api/channel-post-message.md) | [chatMessage](../resources/chatmessage.md) | Отправка сообщения в канал. |
|[Создание ответа на chatMessage в канале](../api/channel-post-messagereply.md) | [chatMessage](../resources/chatmessage.md) | Ответ на сообщение в канале.|
|[Получение папки с файлами](../api/driveitem-get.md)| [driveItem](driveitem.md) | Получение сведений о папке SharePoint, в которой хранятся файлы канала. |
|[Перечисление вкладок](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных в канале.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Необязательное текстовое описание канала.|
|displayName|String|Имя канала, отображаемое для пользователя в Microsoft Teams.|
|id|String|Уникальный идентификатор канала. Только для чтения.|
|isFavoriteByDefault|Логический|Указывает, должен ли канал автоматически помечаться как "Избранное" для всех участников команды. Задается только программными средствами с помощью [Создания группы](../api/team-post.md). Значение по умолчанию: `false`.|
|email|String| Адрес электронной почты для отправки сообщений в канал. Только для чтения.|
|webUrl|String|Гиперссылка, ведущая к каналу в Microsoft Teams. Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал". Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться. Только для чтения.|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания канала.|

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|messages|Коллекция [chatMessage](chatmessage.md)|Коллекция всех сообщений в канале. Свойство навигации. Допускается значение null.|
|tabs|Коллекция [teamsTab](../resources/teamstab.md)|Коллекция всех вкладок в канале. Свойство навигации.|
|[filesFolder](../api/channel-get-filesfolder.md)|[driveItem](driveitem.md)|Метаданные для расположения, в котором хранятся файлы канала.|
|operations|Коллекция [teamsAsyncOperation](teamsasyncoperation.md)| Асинхронные операции, которые выполнялись или выполняются для этой команды. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
  "webUrl": "string",
  "createdDateTime": "string (timestamp)"
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
