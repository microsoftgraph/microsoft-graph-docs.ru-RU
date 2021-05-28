---
title: Тип ресурса team
description: 'Команда Microsoft Teams — это коллекция каналов. '
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d6ebc247ec6868cd32e2ef3790f7542d9eb546fe
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682049"
---
# <a name="team-resource-type"></a>Тип ресурса team

Пространство имен: microsoft.graph



Команда в Microsoft Teams — это коллекция объектов [channel](channel.md).
Канал представляет тему и логически обособляет обсуждение в команде.

Каждая команда связана с [группой](../resources/group.md).
У группы такой же идентификатор, как у команды. Например, /groups/{id}/team совпадает с /teams/{id}.
Дополнительные сведения о работе с группами и участниками в командах см. в статье [Работа с Microsoft Teams при помощи REST API Microsoft Graph](teams-api-overview.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание команды](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Создание команды с нуля. |
|[Создание команды из группы](../api/team-put-teams.md) | [team](team.md) | Создание команды или добавление команды в существующую группу.|
|[Получение команды](../api/team-get.md) | [team](team.md) | Получение свойств и связей указанной команды.|
|[Обновление команды](../api/team-update.md) | [team](team.md) |Обновление свойств указанной команды. |
|[Удаление команды](../api/group-delete.md) | Нет |Удаление команды и ее связанной группы. |
|[Перечисление участников](../api/team-list-members.md)|Коллекция [conversationMember](../resources/conversationmember.md)|Получение списка участников группы.|
|[Добавление участника](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Добавление нового участника в группу.|
|[Получение участника](../api/team-get-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение участника группы.|
|[Обновление роли участника](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.|
|[Удаление участника](../api/team-delete-members.md)|Нет|Удаление существующего участника из группы.|
|[Архивация команды](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Перевод команды в состояние только для чтения. |
|[Распаковка команды](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Восстановление команды в состояние чтения и записи. |
|[Клонирование команды](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Копирование команды и ее связанной группы. |
|[Перечисление ваших команд](../api/user-list-joinedteams.md) | Коллекция [team](team.md) | Перечисление команд, в которых вы являетесь участником. |
|[Завершение миграции](../api/team-completemigration.md)|[team](team.md)| Удаление режима миграции из команды, после чего команда становится доступной для публикации и чтения сообщений пользователями.|
|[Перечисление приложений, установленных в команде](../api/team-list-installedapps.md) | Коллекция [teamsAppInstallation](teamsappinstallation.md) | Перечисление приложений, установленных в команде.|
|[Добавление приложения в команду](../api/team-post-installedapps.md) |Нет | Добавление (установка) приложения в команду.|
|[Получение приложения, установленного в команде](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Получение указанного приложения, установленного в команде.|
|[Обновление приложения, установленного в команде](../api/team-teamsappinstallation-upgrade.md) | Нет | Обновление приложения, установленного в команде, до последней версии.|
|[Удаление приложения из команды](../api/team-delete-installedapps.md) | Нет | Удаление приложения из команды.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|string| Имя команды. |
|description|string| Необязательное описание для команды. Максимальная длина: 1024 символов. |
|classification|string| Необязательная метка. Обычно описывает конфиденциальность данных или работы команды. Должно соответствовать одному из предварительно настроенных наборов в каталоге клиента. |
|specialization|[teamSpecialization](teamspecialization.md)| Необязательное свойство. Указывает, предназначена ли команда для определенного варианта использования.  У каждой специализации команды есть доступ к уникальным действиям и возможностям, предназначенным для своего варианта использования. |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| Видимость группы и команды. По умолчанию значение "Общедоступно". |
|funSettings|[teamFunSettings](teamfunsettings.md) |Параметры для настройки использования Giphy, мемов и наклеек в команде.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.|
|internalId | string | Уникальный идентификатор для команды, используемый в нескольких местах, например в журнале аудита или [API действий управления Office 365](/office/office-365-management-api/office-365-management-activity-api-reference). |
|isArchived|Boolean|Находится ли команда в режиме только для чтения. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |Параметры для настройки обмена сообщениями и упоминаний в команде.|
|webUrl|string (только для чтения) | Гиперссылка, ведущая к команде в клиенте Microsoft Teams. Это URL-адрес, получаемый при щелчке правой кнопкой мыши по команде в клиенте Microsoft Teams и выборе пункта **Получить ссылку на команду**. Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться. |
|createdDateTime|dateTimeOffset|Метка времени создания команды.|

### <a name="instance-attributes"></a>Атрибуты экземпляра

Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.

| Имя свойства| Тип   | Описание
|:-----------------------|:-------|:-------------------------|
|@microsoft.graph.teamCreationMode|Строка|Указывает, что команда находится в состоянии миграции и в настоящее время используется для миграции. Принимает одно значение: `migration`. **Примечание**. В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества импортированных данных.|

Пример запроса POST см. в разделе [Запрос (создание команды в состоянии миграции)](https://docs.microsoft.com/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|channels|Коллекция [channel](channel.md)|Коллекция каналов и сообщений, связанных с командой.|
|installedApps|[teamsAppInstallation](teamsappinstallation.md) collection|Приложения, установленные в команде.|
|members|Коллекция [conversationMember](../resources/conversationmember.md)|Участники и владельцы команды.|
|operations|Коллекция [teamsAsyncOperation](teamsasyncoperation.md)| Асинхронные операции, которые выполнялись или выполняются для этой команды. | 
|[primaryChannel](../api/team-get-primarychannel.md)|[channel](channel.md)| Общий канал для команды. | 
|schedule|[schedule](schedule.md)| Расписание смен для команды.|
|шаблон|[teamsTemplate](teamstemplate.md)| Шаблон, из которого создана команда. См. [доступные шаблоны](/MicrosoftTeams/get-started-with-teams-templates). |

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
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"},
  "createdDateTime": "dateTimeOffset"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>См. также

- [Работа с Microsoft Teams при помощи API Microsoft Graph](teams-api-overview.md)
- [Создание группы с командой](/graph/teams-create-group-and-team)
- [Перечисление всех команд](/graph/teams-list-all-teams)

