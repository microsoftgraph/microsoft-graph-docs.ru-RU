---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2611f3d60d93b8f142c9d6454f8525dbe18b9721
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236259"
---
# <a name="channel-resource-type"></a>Тип ресурса channel

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками. Каждый канал предназначен для определенной темы, отдела или проекта. Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.

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
|[Получение всех сообщений в канале](../api/channel-getallmessages.md)|Коллекция [channel](channel.md) | Получайте все сообщения каналов, в которые входит пользователь. |
|[Создание сообщения канала](../api/channel-post-messages.md) | [chatMessage](../resources/chatmessage.md) | Отправка сообщения в канал. |
|[Создание ответа на сообщение канала](../api/chatmessage-post-replies.md) | [chatMessage](../resources/chatmessage.md) | Ответ на сообщение в канале.|
|[Получение папки с файлами](../api/channel-get-filesfolder.md)| [driveItem](driveitem.md) | Получение сведений о папке SharePoint, в которой хранятся файлы канала. |
|[Перечисление вкладок](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных в канале.|
|[Перечисление участников канала](../api/channel-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка участников канала.|
|[Добавление участника канала](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | Добавление участника в канал. Поддерживается только для `channel` с типом членства `private`.|
|[Получение участника канала](../api/channel-get-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение участника канала.|
|[Обновление роли участника канала](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | Обновление свойства участника канала. Поддерживается только для канала с типом членства `private`.|
|[Удаление участника канала](../api/channel-delete-members.md) | Нет | Удаление участника канала. Поддерживается, только если параметру `channelType` присвоено значение `private`.|
|[Завершение миграции](../api/channel-completemigration.md)|[channel](channel.md)| Удаление режима миграции из канала, после чего канал становится доступным для публикации и чтения сообщений пользователями.|
|[Перечисление вкладок в канале](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных на канале.|
|[Добавление вкладки в канал](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки на канал.|
|[Получение вкладки на канале](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Получение определенной вкладки, закрепленной на канале.|
|[Вкладка "обновление" на канале](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Обновляет свойства вкладки на канале.|
|[Удаление вкладки из канала](../api/channel-delete-tabs.md) | Нет | Удаление (открепление) вкладки из канала.|
|[Подготовка адреса электронной почты канала](../api/channel-provisionemail.md) |[provisionChannelEmailResult](../resources/provisionchannelemailresult.md)| Подготовка адреса электронной почты.|
|[Удаление адреса электронной почты канала](../api/channel-removeemail.md) | Нет | Удаление адреса электронной почты.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Необязательное текстовое описание канала.|
|displayName|String|Имя канала, отображаемое для пользователя в Microsoft Teams.|
|id|String|Уникальный идентификатор канала. Только для чтения.|
|isFavoriteByDefault|Логический|Указывает, должен ли канал автоматически помечаться как "Избранное" для всех участников команды. Задается только программными средствами с помощью [Создания группы](../api/team-post.md). Значение по умолчанию: `false`.|
|email|String| Адрес электронной почты для отправки сообщений в канал. Только для чтения.|
|webUrl|String|Гиперссылка, ведущая к каналу в Microsoft Teams. Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал". Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться. Только для чтения.|
|membershipType|[channelMembershipType](../resources/enums.md#channelmembershiptype-values)|Тип канала. Можно настроить во время создания и нельзя изменить. Значение по умолчанию: standard.|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания канала.|
|moderationSettings|[channelModerationSettings](../resources/channelmoderationsettings.md)|Настройки модерации канала, чтобы контролировать, кто может создавать новые сообщения и отвечать на сообщения в этом канале.|

### <a name="instance-attributes"></a>Атрибуты экземпляра

Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.

| Имя свойства| Тип   | Описание
|:-----------------------|:-------|:-------------------------|
|@microsoft.graph.channelCreationMode|Строка|Указывает, что канал находится в состоянии миграции и в настоящее время используется для миграции. Принимает одно значение: `migration`.|

> **Примечание**: `channelCreationMode` – перечисление, принимающее значение `migration`.

Пример запроса POST см. в разделе [Запрос (создание канала в состоянии миграции)](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams#request-create-a-team-in-migration-state).

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|messages|Коллекция [chatMessage](chatmessage.md)|Коллекция всех сообщений в канале. Свойство навигации. Допускается значение NULL.|
|tabs|Коллекция [teamsTab](../resources/teamstab.md)|Коллекция всех вкладок в канале. Свойство навигации.|
|members|Коллекция [conversationMember](conversationmember.md)|Коллекция записей участников, сопоставленных с каналом.|
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
  "membershipType": "channelMembershipType",
  "createdDateTime": "string (timestamp)",
  "moderationSettings": { "@odata.type": "microsoft.graph.channelModerationSettings" }
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
