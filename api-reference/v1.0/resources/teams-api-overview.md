---
title: Работа с Microsoft Teams при помощи API Microsoft Graph
description: Microsoft Teams — это рабочее пространство с чатами в Office 365, обеспечивающее встроенный доступ к календарям команд, файлам, заметкам OneNote, планам Планировщика и многому другому.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: bd21b806635885e5feda3fde4c8fe6463aa9ec62
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033833"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Работа с Microsoft Teams при помощи API Microsoft Graph



Microsoft Teams — это рабочее пространство с чатами в Office 365, обеспечивающее встроенный доступ к календарям команд, файлам, заметкам OneNote, планам Планировщика, расписаниям Смен и многому другому.

## <a name="key-resources-in-microsoft-teams"></a>Основные ресурсы в Microsoft Teams

| Ресурс | Методы |
|:---------------|:--------|
|[team](../resources/team.md)| [Перечисление ваших команд](../api/user-list-joinedteams.md), [перечисление всех команд](/graph/teams-list-all-teams), [создание](../api/team-put-teams.md), [чтение](../api/team-get.md), [обновление](../api/team-update.md), [удаление](/graph/api/group-delete?view=graph-rest-1.0), [клонирование](../api/team-clone.md), [архивирование](../api/team-archive.md), [распаковка](../api/team-unarchive.md) |
|[group](../resources/group.md)| [Добавление участника](../api/group-post-members.md), [удаление участника](../api/group-delete-members.md), [добавление владельца](../api/group-post-owners.md), [удаление владельца](../api/group-delete-owners.md), [получение файлов](drive.md), [получение записной книжки](/graph/api/resources/notebook?view=graph-rest-1.0), [получение планов](plannergroup.md), [получение календаря](event.md) |
|[channel](../resources/channel.md)|[Список](../api/channel-list.md), [создание](../api/channel-post.md), [чтение](../api/channel-get.md), [обновление](../api/channel-patch.md), [удаление](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[Список](../api/teamstab-list.md), [создание](../api/teamstab-add.md), [чтение](../api/teamstab-get.md), [обновление](../api/teamstab-update.md), [удаление](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[Список](../api/teamsapp-list.md), [публикация](../api/teamsapp-publish.md), [обновление](../api/teamsapp-update.md), [удаление](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [Список](../api/teamsappinstallation-list.md), [установка](../api/teamsappinstallation-add.md), [обновление](../api/teamsappinstallation-delete.md), [удаление](../api/teamsappinstallation-delete.md) |
| [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (предварительная версия)| [Список](/graph/api/channel-list-messages?view=graph-rest-beta), [отправка](/graph/api/channel-post-chatmessage?view=graph-rest-beta), [чтение](/graph/api/channel-get-message?view=graph-rest-beta) |
| [call](/graph/api/resources/call?view=graph-rest-beta) (предварительная версия)| [Ответ](/graph/api/call-answer?view=graph-rest-beta), [отклонение](/graph/api/call-reject?view=graph-rest-beta), [перенаправление](/graph/api/call-redirect?view=graph-rest-beta), [отключение звука](/graph/api/call-mute?view=graph-rest-beta), [включение звука](/graph/api/call-unmute?view=graph-rest-beta), [обновление метаданных](/graph/api/call-updatemetadata?view=graph-rest-beta), [изменение роли при демонстрации экрана](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [перечисление участников](/graph/api/call-list-participants?view=graph-rest-beta), [приглашение участников](/graph/api/participant-invite?view=graph-rest-beta), [отключение звука всех участников](/graph/api/participant-muteall?view=graph-rest-beta) |
|[schedule](/graph/api/resources/schedule?view=graph-rest-beta) (предварительная версия)| [Создание или замена](/graph/api/team-put-schedule?view=graph-rest-beta), [получение](/graph/api/schedule-get?view=graph-rest-beta), [предоставление общего доступа](/graph/api/schedule-share?view=graph-rest-beta) |
|[schedulingGroup](/graph/api/resources/schedulinggroup?view=graph-rest-beta) (предварительная версия)| [Создание](/graph/api/schedule-post-schedulinggroups?view=graph-rest-beta), [список](/graph/api/schedule-list-schedulinggroups?view=graph-rest-beta), [получение](/graph/api/schedulinggroup-get?view=graph-rest-beta), [замена](/graph/api/schedulinggroup-put?view=graph-rest-beta), [удаление](/graph/api/schedulinggroup-delete?view=graph-rest-beta) |
|[shift](/graph/api/resources/shift?view=graph-rest-beta) (предварительная версия)| [Создание](/graph/api/schedule-post-shifts?view=graph-rest-beta), [список](/graph/api/schedule-list-shifts?view=graph-rest-beta), [получение](/graph/api/shift-get?view=graph-rest-beta), [замена](/graph/api/shift-put?view=graph-rest-beta), [удаление](/graph/api/shift-delete?view=graph-rest-beta) |
|[timeOff](/graph/api/resources/timeoff?view=graph-rest-beta) (предварительная версия)| [Создание](/graph/api/schedule-post-timesoff?view=graph-rest-beta), [список](/graph/api/schedule-list-timesoff?view=graph-rest-beta), [получение](/graph/api/timeoff-get?view=graph-rest-beta), [замена](/graph/api/timeoff-put?view=graph-rest-beta), [удаление](/graph/api/timeoff-delete?view=graph-rest-beta) |
|[timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta) (предварительная версия)| [Создание](/graph/api/schedule-post-timeoffreasons?view=graph-rest-beta), [список](/graph/api/schedule-list-timeoffreasons?view=graph-rest-beta), [получение](/graph/api/timeoffreason-get?view=graph-rest-beta), [замена](/graph/api/timeoffreason-put?view=graph-rest-beta), [удаление](/graph/api/timeoffreason-delete?view=graph-rest-beta) |

## <a name="teams-and-groups"></a>Команды и группы

В Microsoft Graph приложение Microsoft Teams представлено ресурсом [group](../resources/group.md). Группы Microsoft Teams и Office 365 предназначены для различных требований совместной работы в группе. Почти всех групповые функции применимы к группам Microsoft Teams и Office 365, например календарь группы, файлы, заметки, фотографии, планы и т. д. Основное различие между [командой](team.md) и группой Office 365 состоит в режиме общения участников. Участники команды общаются в сохраняемом чате в контексте определенной команды. Участники группы Office 365 общаются с помощью групповых бесед, которые являются беседами по электронной почте, осуществляемыми в контексте группы в Outlook.

У любой группы, содержащей команду, есть свойство **resourceProvisioningOptions** со значением Team. 

>**Примечание.** Свойство **Group.resourceProvisioningOptions** можно изменить.
Не добавляйте и не удаляйте значение Team из этой коллекции; в противном случае вы получите неправильные результаты при перечислении всех команд.

Ниже указаны различия на уровне API между командами и группами.

- Метод [Перечисление команд, к которым присоединился пользователь](../api/user-list-joinedteams.md) применяется только к Microsoft Teams.
- См. также [известные проблемы](/graph/known-issues) для этих API.

>Примечание. Если вы используете интерфейсы API для групп в приложении Microsoft Teams, а не в отдельном приложении (например, для вкладки или бота в Microsoft Teams), следуйте инструкциям из статьи Использование Microsoft Graph на страницах Microsoft Teams.

## <a name="membership-changes-in-microsoft-teams"></a>Изменение состава участников в Microsoft Teams

Чтобы добавить участников и владельцев в команду, измените состав участников [группы](../resources/group.md) с таким же идентификатором.

| Вариант использования      | Глагол      | URL-адрес |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Добавление участника](../api/group-post-members.md)    | POST      | /groups/{id}/members/$ref  |
| [Удаление участника](../api/group-delete-members.md)   | DELETE    | /groups/{id}/members/{userId}/$ref |
| [Добавление владельца](../api/group-post-owners.md)     | POST       | /groups/{id}/owners/$ref |
| [Удаление владельца](../api/group-delete-owners.md) | DELETE    | /groups/{id}/owners/{userId}/$ref |
| [Обновление команды](../api/team-update.md)  | PATCH     | /teams/{id} |

При добавлении владельца также рекомендуется добавить этого пользователя в качестве участника. Если владелец группы не является ее участником, изменения состава владельцев и участников могут сразу не отображаться в Microsoft Teams. Кроме того, разные приложения и API обрабатывают их по-разному. Например, Microsoft Teams отображает команды, в которых пользователь является участником или владельцем, а командлеты PowerShell Microsoft Teams и API /me/joinedTeams отображают только команды, в которых пользователь является участником. Чтобы избежать путаницы, добавьте всех владельцев в список участников. 

Известная проблема: если вызвать запрос DELETE /groups/{id}/owners, пользователь также удаляется из списка /groups/{id}/members. Чтобы устранить эту проблему, рекомендуется удалить пользователя из владельцев и участников, подождать 10 секунд и снова добавить его к участникам.

При добавлении и удалении участников и владельцев, не применяйте фигурные скобки {} вокруг идентификатора.

| Скорость | Синтаксис | 
| ------ | ----- |
| Быстро | https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| Медленно | https://graph.microsoft.com/v1.0/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

Аналогичным образом, если параметр `userId` в URL-адресе или полезных данных выражается как имя участника-пользователя (UPN), а не как идентификатор GUID, производительность будет ниже.

| Скорость | Синтаксис | 
| ------ | ----- |
| Быстро | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| Медленно | alexeyorekhov@example.com | 

При выборе медленного пути, если текущий участник или владелец команды вошел в систему в приложении или на веб-сайте Microsoft Teams, изменения отразятся в течение часа.
Если ни один из таких пользователей не вошел в систему в приложении или на веб-сайте Microsoft Teams, изменения не отразятся, пока не пройдет час после входа одного из них.

## <a name="see-also"></a>См. также

- [Обзор API Microsoft Teams](/graph/teams-concept-overview)
- Примеры кода: [Авиакомпания Contoso](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [мини-примеры C#](https://github.com/microsoftgraph/csharp-teams-sample-graph)
