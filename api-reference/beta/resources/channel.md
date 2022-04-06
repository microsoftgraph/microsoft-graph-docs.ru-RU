---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: akjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e7c8091f3f3e29932520e93a7be3cdd2d830c5e0
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684594"
---
# <a name="channel-resource-type"></a>Тип ресурса channel

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками. Каждый канал предназначен для определенной темы, отдела или проекта. Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление каналов](../api/channel-list.md) | Коллекция [channel](channel.md) | Получение списка каналов в команде.|
|[Перечисление входящих каналов](../api/team-list-incomingchannels.md)|Коллекция [channel](../resources/channel.md)|Получение списка каналов [, к которые](../resources/channel.md) предоставлен общий доступ **команде**.|
|[Вывод списка всех каналов](../api/team-list-allchannels.md)|Коллекция [channel](../resources/channel.md)|Получение списка [каналов в](../resources/channel.md) команде **или** общий доступ к **команде (** входящие каналы).|
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
|[Добавление участника канала](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | Добавление участника в канал. Поддерживается только для каналов с **типом membershipType** или `private` `shared`.|
|[Получение участника канала](../api/channel-get-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение участника канала.|
|[Обновление роли участника канала](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | Обновление свойства участника канала. Поддерживается только для каналов с **типом membershipType** или `private` `shared`.|
|[Удаление участника канала](../api/channel-delete-members.md) | Нет | Удаление участника канала. Поддерживается только для каналов с **типом membershipType** или `private` `shared`.|
|[Завершение миграции](../api/channel-completemigration.md)|[channel](channel.md)| Удаление режима миграции из канала, после чего канал становится доступным для публикации и чтения сообщений пользователями.|
|[Перечисление вкладок в канале](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных на канале.|
|[Добавление вкладки в канал](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки на канал.|
|[Получение вкладки на канале](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Получение определенной вкладки, закрепленной на канале.|
|[Вкладка "обновление" на канале](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Обновляет свойства вкладки на канале.|
|[Удаление вкладки из канала](../api/channel-delete-tabs.md) | Нет | Удаление (открепление) вкладки из канала.|
|[Подготовка адреса электронной почты канала](../api/channel-provisionemail.md) |[provisionChannelEmailResult](../resources/provisionchannelemailresult.md)| Подготовка адреса электронной почты для канала.|
|[Удаление адреса электронной почты канала](../api/channel-removeemail.md) | Нет | Удаление адреса электронной почты канала.|
|[Удаление входящего канала](../api/team-delete-incomingchannel.md) | Никаких других изменений не происходит| Удалите входящий канал.|
|[Перечисление команд, к которые предоставлен общий доступ с помощью канала](../api/sharedwithchannelteaminfo-list.md)|[Коллекция sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Получение списка команд, к которые предоставлен доступ каналу.|
|[Получение общего доступа к команде с помощью канала](../api/sharedwithchannelteaminfo-get.md)|[sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Получите команду, доступную каналу.|
|[Отмена общего доступа к каналу с командой](../api/sharedwithchannelteaminfo-delete.md)|Никаких других изменений не происходит|Отмените общий доступ к каналу с командой.|
|[Список разрешенных участников](../api/sharedwithchannelteaminfo-list-allowedmembers.md)|Коллекция [conversationMember](../resources/conversationmember.md)|Получение списка участников команды, имеющих доступ к общему каналу.|
|[Проверка доступа пользователей](../api/channel-doesuserhaveaccess.md)|Логический|Проверьте, имеет ли пользователь доступ к общему каналу.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Необязательное текстовое описание канала.|
|displayName|String|Имя канала, отображаемое для пользователя в Microsoft Teams.|
|id|String|Уникальный идентификатор канала. Только для чтения.|
|isFavoriteByDefault|Логический|Указывает, должен ли канал автоматически помечаться как "Избранное" для всех участников команды. Задается только программными средствами с помощью [Создания группы](../api/team-post.md). Значение по умолчанию: `false`.|
|email|String| Адрес электронной почты для отправки сообщений в канал. Только для чтения.|
|webUrl|String|Гиперссылка, ведущая к каналу в Microsoft Teams. Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал". Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться. Только для чтения.|
|membershipType|channelMembershipType|Тип канала. Можно настроить во время создания и нельзя изменить. Допустимые значения: `standard`, `private`, `unknownFutureValue`, `shared`. Значение по умолчанию — `standard`. Обратите внимание, что требуется использоваться заголовок запроса `Prefer: include-unknown-enum-members`, чтобы получить следующее значение в этом [расширяемом перечислении](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `shared`.|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания канала.|
|moderationSettings|[channelModerationSettings](../resources/channelmoderationsettings.md)|Настройки модерации канала, чтобы контролировать, кто может создавать новые сообщения и отвечать на сообщения в этом канале.|
|tenantId |string | Идентификатор Azure Active Directory клиента. |

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
|sharedWithTeams|[Коллекция sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Коллекция команд, совместно используемых с каналом.|

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
