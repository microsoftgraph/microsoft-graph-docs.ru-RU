---
title: Тип ресурса группы
description: 'Группы в группах Microsoft — это коллекция каналов. '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 85694e18771ac17873f97cedf68d074ee550f787
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878549"
---
# <a name="team-resource-type"></a>Тип ресурса группы



Группы в группах Microsoft — это коллекция [каналов](channel.md). Канал представляет раздел и логическая изоляции обсуждения в группе.

Для любой группы связан с [группы](../resources/group.md).
Группа имеет тот же идентификатор, как команда — например, /groups/ {идентификатор} / team совпадает с /teams/ {идентификатор}.
Дополнительные сведения о работе с группами и участниками групп показано [Использование интерфейса API REST графическое представление Microsoft для работы с группами Майкрософт](teams-api-overview.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание группы](../api/team-put-teams.md) | [Группа](team.md) | Создание новой группы или добавление группы к существующей группе.|
|[Получение группы](../api/team-get.md) | [Группа](team.md) | Извлечение свойств и связи из указанной группы.|
|[Группа обновления](../api/team-update.md) | [Группа](team.md) |Обновление свойств указанной группы. |
|[Удаление группы](/graph/api/group-delete?view=graph-rest-1.0) | Нет |Удаление группы и его связанную группу. |
|[Клонирование группы](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Скопируйте группа и его связанную группу. |
|[Группа архива](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Поместите группа в состояние только для чтения. |
|[Unarchive группы](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Восстановите группа в состояние чтение запись. |
|[Список рабочих групп](../api/user-list-joinedteams.md) | семейства сайтов [групп](team.md) | Список групп, которые вы являетесь членом. |
|[Список всех групп](/graph/teams-list-all-teams) | Коллекция объектов [group](group.md) | Список всех групп, которые имеют группами. |
|[Публикация приложений для вашей организации](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | Создание групп приложений видимым только для вашей организации. |
|[Добавление приложения в группу](../api/teamsappinstallation-add.md) | [teamsappinstallation](teamsappinstallation.md) | Добавляет (установить) приложения в группу.|
|[Добавление вкладки канала](../api/teamstab-add.md) | [teamsTab](../resources/teamstab.md) | Добавляет (установить) вкладки канал группы.|

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:---------------|:--------|:----------|
|funSettings|[teamFunSettings](teamfunsettings.md) |Параметры для настройки использования Giphy, memes и наклейки рабочих групп.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.|
|isArchived|Логический|Является ли эта группа в режиме только для чтения. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.|
|webUrl|String (только для чтения) | Гиперссылка, будут поступать на группы в клиенте группами Майкрософт. Это URL-адрес, который вы получаете при щелкните правой кнопкой мыши группы в клиенте Microsoft группы и выберите **получить ссылку на группы**. Этот URL-адрес должен быть обрабатываются как непрозрачный больших двоичных объектов и не синтаксический анализ. |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|каналы|Коллекция [канала](channel.md)|Коллекция каналы & сообщения, связанный с группой.|
|installedApps|[teamsAppInstallation](teamsappinstallation.md) коллекции|Приложения, установленные в этой группе.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
  "isArchived": false,
  "webUrl": "https://...longUrl..."
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
- [Создание группы с группой](/graph/teams-create-group-and-team)
- [Использование интерфейсов API групп](teams-api-overview.md)
