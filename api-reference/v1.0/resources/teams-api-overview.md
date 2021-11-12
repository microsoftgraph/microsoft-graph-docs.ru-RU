---
title: Работа с Microsoft Teams при помощи API Microsoft Graph
description: Microsoft Teams — это рабочее пространство с чатами в Microsoft 365, обеспечивающее встроенный доступ к календарям команд, файлам, заметкам OneNote, планам Планировщика и многому другому.
ms.localizationpriority: high
author: nkramer
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: 4bd125c401847a36271edebe6a6432343bd1f5f3
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891139"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Работа с Microsoft Teams при помощи API Microsoft Graph

Microsoft Teams — это рабочее пространство с чатами в Microsoft 365, обеспечивающее встроенный доступ к календарям команд, файлам, заметкам OneNote, планам Планировщика, расписаниям Смен и многому другому.

## <a name="key-resources-in-microsoft-teams"></a>Основные ресурсы в Microsoft Teams

| Ресурс | Методы |
|:---------------|:--------|
|[team](../resources/team.md)| [Перечисление ваших команд](../api/user-list-joinedteams.md), [перечисление всех команд](/graph/teams-list-all-teams), [создание](../api/team-put-teams.md), [чтение](../api/team-get.md), [обновление](../api/team-update.md), [удаление](../api/group-delete.md), [клонирование](../api/team-clone.md), [архивирование](../api/team-archive.md), [распаковка](../api/team-unarchive.md) |
|[group](../resources/group.md)| [Добавление участника](../api/group-post-members.md), [удаление участника](../api/group-delete-members.md), [добавление владельца](../api/group-post-owners.md), [удаление владельца](../api/group-delete-owners.md), [получение файлов](drive.md), [получение записной книжки](../resources/notebook.md), [получение планов](plannergroup.md), [получение календаря](event.md) |
|[channel](../resources/channel.md)|[Список](../api/channel-list.md), [создание](../api/channel-post.md), [чтение](../api/channel-get.md), [обновление](../api/channel-patch.md), [удаление](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[Список](../api/channel-list-tabs.md), [создание](../api/channel-post-tabs.md), [чтение](../api/channel-get-tabs.md), [обновление](../api/channel-patch-tabs.md), [удаление](../api/channel-delete-tabs.md) |
|[teamsApp](../resources/teamsapp.md)|[Список](../api/appcatalogs-list-teamsapps.md), [публикация](../api/teamsapp-publish.md), [обновление](../api/teamsapp-update.md), [удаление](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [Список](../api/team-list-installedapps.md), [установка](../api/team-post-installedapps.md), [обновление](../api/team-delete-installedapps.md), [удаление](../api/team-delete-installedapps.md) |
|[chatMessage](../resources/chatmessage.md)| [список в канале](../api/channel-list-messages.md), [список в чате](../api/chat-list-messages.md), [отправка](../api/chatmessage-post.md), [чтение в канале](../api/chatmessage-get.md), [чтение в чате](../api/chatmessage-get.md)|
|[call](../resources/call.md)| [Ответ](../api/call-answer.md), [отклонение](../api/call-reject.md), [перенаправление](../api/call-redirect.md), [отключение звука](../api/call-mute.md), [включение звука](../api/call-unmute.md), [изменение роли при демонстрации экрана](../api/call-changescreensharingrole.md), [перечисление участников](../api/call-list-participants.md), [приглашение участников](../api/participant-invite.md) |
|[schedule](../resources/schedule.md)| [Создание или замена](../api/team-put-schedule.md), [получение](../api/schedule-get.md), [предоставление общего доступа](../api/schedule-share.md) |
|[schedulingGroup](../resources/schedulinggroup.md)| [Создание](../api/schedule-post-schedulinggroups.md), [список](../api/schedule-list-schedulinggroups.md), [получение](../api/schedulinggroup-get.md), [замена](../api/schedulinggroup-put.md), [удаление](../api/schedulinggroup-delete.md) |
|activityFeedNotification| [Отправить уведомление пользователю в области чата](../api/chat-sendactivitynotification.md), [Отправить уведомление пользователю в области команды](../api/team-sendactivitynotification.md), [Отправить уведомление пользователю в персональной области](../api/userteamwork-sendactivitynotification.md)|
|[shift](../resources/shift.md)| [Создание](../api/schedule-post-shifts.md), [список](../api/schedule-list-shifts.md), [получение](../api/shift-get.md), [замена](../api/shift-put.md), [удаление](../api/shift-delete.md) |
|[timeOff](../resources/timeoff.md)| [Создание](../api/schedule-post-timesoff.md), [список](../api/schedule-list-timesoff.md), [получение](../api/timeoff-get.md), [замена](../api/timeoff-put.md), [удаление](../api/timeoff-delete.md) |
|[timeOffReason](../resources/timeoffreason.md)| [Создание](../api/schedule-post-timeoffreasons.md), [список](../api/schedule-list-timeoffreasons.md), [получение](../api/timeoffreason-get.md), [замена](../api/timeoffreason-put.md), [удаление](../api/timeoffreason-delete.md) |

## <a name="microsoft-teams-limits"></a>Ограничения Microsoft Teams

Протестированные ограничения производительности (мощности) Microsoft Teams описаны в статье [Ограничения и спецификации для Microsoft Teams](/microsoftteams/limits-specifications-teams).
Эти ограничения применяются при непосредственном использовании Microsoft Teams или с помощью API Microsoft Graph.
Так как у каждой команды есть соответствующая группа, а каждая группа является объектом каталога, ограничение [количества групп](/microsoft-365/admin/create-groups/office-365-groups#group-limits) и [количества объектов каталога ("ресурсов")](/azure/active-directory/users-groups-roles/directory-service-limits-restrictions) может также оказывать влияние. 

Файлы в каналах хранятся в SharePoint; при этом применяются [ограничения SharePoint Online](/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits).

См. также [Ограничения регулирования для служб Microsoft Teams](/graph/throttling#microsoft-teams-service-limits).

## <a name="teams-and-groups"></a>Команды и группы

В Microsoft Graph приложение Microsoft Teams представлено ресурсом [group](../resources/group.md). Команды Microsoft Teams и группы Microsoft 365 предназначены для различных требований совместной работы в группе. Почти всех групповые функции применимы к командам Microsoft Teams и группам Microsoft 365, например календарь группы, файлы, заметки, фотографии, планы и т. д. Основное различие между [командой](team.md) и группой Microsoft 365 состоит в режиме общения участников. Участники команды общаются в сохраняемом чате в контексте определенной команды. Участники группы Microsoft 365 общаются с помощью групповых бесед, то есть бесед по электронной почте, которые осуществляются в контексте группы в Outlook.

У любой группы, содержащей команду, есть свойство **resourceProvisioningOptions** со значением Team.

>**Примечание.** Свойство **Group.resourceProvisioningOptions** можно изменить.
Не добавляйте и не удаляйте значение Team из этой коллекции; в противном случае вы получите неправильные результаты при перечислении всех команд.

Ниже указаны различия на уровне API между командами и группами.

- Сохраняемый чат доступен только в Microsoft Teams. Эта функция иерархически представлена ресурсами [channel](../resources/channel.md) и [chatMessage](../resources/chatmessage.md).
- Групповые беседы доступны только в группах Microsoft 365. Эта функция иерархически представлена ресурсами [conversation](../resources/conversation.md), [conversationThread](../resources/conversationthread.md) и [post](../resources/post.md).
- Метод [Перечисление команд, к которым присоединился пользователь](../api/user-list-joinedteams.md) применяется только к Microsoft Teams.
- [API звонков и собраний по сети](./communications-api-overview.md) применяются только к Microsoft Teams.
- См. также [известные проблемы](/graph/known-issues) для этих API.

>Примечание. Если вы используете интерфейсы API для групп в приложении Microsoft Teams, а не в отдельном приложении (например, для вкладки или бота в Microsoft Teams), следуйте инструкциям из статьи Использование Microsoft Graph на страницах Microsoft Teams.

## <a name="membership-changes-in-microsoft-teams"></a>Изменение состава участников в Microsoft Teams

| Вариант использования      | Глагол      | URL-адрес |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Добавление участника](../api/team-post-members.md) | POST      | /teams/{team-id}/members  |
| [Удаление участника](../api/team-delete-members.md)    | DELETE    | /teams/{team-id}/members/{membership-id} |
| [Обновление роли участника](../api/team-update-members.md) | PATCH | /teams/{team-id}/members/{membership-id} |
| [Обновление команды](../api/team-update.md)  | PATCH     | /teams/{team-id} |

## <a name="polling-requirements"></a>Требования к опросу

Если приложение опрашивает вас на предмет изменения ресурса, это можно делать раз в день. ([teamsAsyncOperation](teamsasyncoperation.md) является исключением из общего правила, так как опрашивается часто.) Если нужно узнавать об изменениях чаще, [создайте подписку](../api/subscription-post-subscriptions.md) на этот ресурс и получайте уведомления об изменениях (веб-перехватчики). Если вы не нашли поддержку для нужного типа подписки, рекомендуем оставить свой отзыв на [форуме идей платформы для разработчиков Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph). 

При опросе на предмет новых сообщений необходимо определить диапазон дат, в котором поддерживается опрос. Дополнительные сведения см. в статье [Получение изменившихся данных о сообщениях в каналах](../api/chatmessage-delta.md).

При опросе для ресурса раз за разом выполняется операция GET, чтобы проверить, не изменился ли он. Операцию GET разрешается выполнять на одном и том же ресурсе несколько раз в день, пока не проводится опрос. Например, хорошо выполнять операцию GET на /me/joinedTeams каждый раз, когда пользователь посещает или обновляет вашу веб-страницу, но было бы неправильно выполнять GET на /me/joinedTeams в цикле каждые 30 секунд, чтобы обновлять эту веб-страницу.

Если приложения не удовлетворяют требованиям опроса, это будет рассматриваться как нарушение [условий использования API Майкрософт](/legal/microsoft-apis/terms-of-use). Такое нарушение может привести к дополнительному [регулированию](/graph/throttling), а также приостановке или прекращению использования API Майкрософт.

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="see-also"></a>См. также

- [Обзор API Microsoft Teams](/graph/teams-concept-overview)
- Примеры кода: [Авиакомпания Contoso](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [мини-примеры C#](https://github.com/microsoftgraph/csharp-teams-sample-graph)
