---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d5f9f78ba70a6156c260ea679e6e1c081bec1dc
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782958"
---
# <a name="channel-resource-type"></a>Тип ресурса channel

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|[Завершение миграции](../api/channel-completemigration.md)|[channel](channel.md)| Удаление режима миграции из канала, после чего канал становится доступным для публикации и чтения сообщений пользователями.|

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

### <a name="instance-attributes"></a>Атрибуты экземпляра

Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.

| Имя свойства| Тип   | Описание
|:-----------------------|:-------|:-------------------------|
|@microsoft.graph.channelCreationMode|Строка|Указывает, что канал находится в состоянии миграции и в настоящее время используется для миграции. Принимает одно значение: `migration`.|

> **Примечание** : `channelCreationMode` – перечисление, принимающее значение `migration`.

Пример запроса POST см. в разделе [Запрос (создание канала в состоянии миграции)](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams#request-create-a-team-in-migration-state).

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|messages|Коллекция [chatMessage](chatmessage.md)|Коллекция всех сообщений в канале. Свойство навигации. Допускается значение null.|
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
