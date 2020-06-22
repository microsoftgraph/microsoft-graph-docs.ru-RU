---
title: Тип ресурса team
description: 'Команда в Microsoft Teams — это коллекция каналов. '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cf94e73bfd7ad05fea8f52ea1f2f219b7933ffa7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793747"
---
# <a name="team-resource-type"></a>Тип ресурса team

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Команда в Microsoft Teams — это коллекция объектов [channel](channel.md). Канал представляет тему и логически обособляет обсуждение в команде.

Каждая команда связана с [группой](../resources/group.md). У группы такой же идентификатор, как у команды. Например, `/groups/{id}/team` совпадает с `/teams/{id}`. Дополнительные сведения о работе с группами и участниками в командах см. в статье [Работа с Microsoft Teams при помощи REST API Microsoft Graph](teams-api-overview.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание команды](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Создание команды с нуля. |
|[Создание команды из группы](../api/team-put-teams.md) | [team](team.md) | Создание команды или добавление команды в существующую группу.|
|[Получение команды](../api/team-get.md) | [team](team.md) | Получение свойств и связей указанной команды.|
|[Обновление команды](../api/team-update.md) | [team](team.md) |Обновление свойств указанной команды. |
|[Удаление команды](/graph/api/group-delete?view=graph-rest-1.0) | Нет |Удаление команды и ее связанной группы. |
|[Клонирование команды](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Копирование команды и ее связанной группы. |
|[Архивация команды](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Перевод команды в состояние только для чтения. |
|[Распаковка команды](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Восстановление команды в состояние чтения и записи. |
|[Перечисление ваших команд](../api/user-list-joinedteams.md) | Коллекция [team](team.md) | Перечисление команд, в которых вы являетесь участником. |
|[Перечисление всех команд](/graph/teams-list-all-teams) | Коллекция [group](group.md) | Перечисление всех групп, содержащих команды. |
|[Получение фотографии команды](../api/team-get-photo.md) | Двоичные данные | Вы можете получить фотографию (изображение) для команды. |
|[Обновление фотографии команды](../api/team-update-photo.md) | Отсутствует | Вы можете обновить фотографию (изображение) для команды. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|string| Имя команды. |
|description|string| Необязательное описание для команды. |
|classification|string| Необязательная метка. Обычно описывает конфиденциальность данных или работы команды. Должно соответствовать одному из предварительно настроенных наборов в каталоге клиента. |
|specialization|[teamSpecialization](teamspecialization.md)| Необязательное свойство. Указывает, предназначена ли команда для определенного варианта использования.  У каждой специализации команды есть доступ к уникальным действиям и возможностям, предназначенным для своего варианта использования. |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| Видимость группы и команды. Значение по умолчанию: Public. |
|funSettings|[teamFunSettings](teamfunsettings.md) |Параметры для настройки использования Giphy, мемов и наклеек в команде.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.|
|internalId | string | Уникальный идентификатор для команды, используемый в нескольких местах, например в журнале аудита или [API действий управления Office 365](https://docs.microsoft.com/office/office-365-management-api/office-365-management-activity-api-reference). |
|isArchived|Boolean|Находится ли команда в режиме только для чтения. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |Параметры для настройки обмена сообщениями и упоминаний в команде.|
|discoverySettings|[teamDiscoverySettings](teamdiscoverysettings.md) |Параметры для настройки возможности обнаружения команды другими пользователями.|
|webUrl|string (только для чтения) | Гиперссылка, ведущая к команде в клиенте Microsoft Teams. Это URL-адрес, получаемый при щелчке правой кнопкой мыши по команде в клиенте Microsoft Teams и выборе пункта **Получить ссылку на команду**. Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться. |
|classSettings|[teamClassSettings](teamclasssettings.md) |Настройка параметров класса. Доступна только в том случае, если команда представляет класс.|

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|channels|Коллекция [channel](channel.md)|Коллекция каналов и сообщений, связанных с командой.|
|installedApps|[teamsAppInstallation](teamsappinstallation.md) collection|Приложения, установленные в команде.|
|owners|[user](user.md)| Список владельцев команды. В настоящее время при создании группы с использованием разрешений для приложения необходимо указать только одного владельца. При использовании делегированных разрешений нельзя указать владельца (владельцем является текущий пользователь). Владельца необходимо указать в виде ИД объекта (GUID), а не имени участника-пользователя (UPN). |
|operations|Коллекция [teamsAsyncOperation](teamsasyncoperation.md)| Асинхронные операции, которые выполнялись или выполняются для этой команды. | 
|[primaryChannel](../api/team-get-primarychannel.md)|[channel](channel.md)| Общий канал для команды. | 
|schedule|[schedule](schedule.md)| Расписание смен для команды.|
|шаблон|[teamsTemplate](teamstemplate.md)| Шаблон, из которого создана команда. См. [доступные шаблоны](https://docs.microsoft.com/MicrosoftTeams/get-started-with-teams-templates). |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

>**Примечание.** Если команда относится к типу class, к ней применяется свойство **classSettings**.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "discoverySettings": {"@odata.type": "microsoft.graph.teamDiscoverySettings"},
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "displayName": "string",
  "description": "string",
  "classification": "string",
  "specialization": "string",
  "visibility": "string",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>См. также

- [Создание группы с командой](/graph/teams-create-group-and-team)
- [Работа с Microsoft Teams при помощи API Microsoft Graph](teams-api-overview.md)
