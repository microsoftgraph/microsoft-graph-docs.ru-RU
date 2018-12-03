---
title: Работа с Microsoft Teams при помощи API Microsoft Graph
description: Группами Майкрософт — это рабочая область на основе чата в Office 365, который предоставляет встроенные доступ к календарей конкретных групп, файлы, заметки OneNote, планировщик работы планы и др.
ms.openlocfilehash: 8ec545998ec003279f1c9f2aaad35588c81011f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076924"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Работа с Microsoft Teams при помощи API Microsoft Graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Группами Майкрософт — это рабочая область на основе чата в Office 365, который предоставляет встроенные доступ к календарей конкретных групп, файлы, заметки OneNote, планировщик работы планы и др.

## <a name="key-resources-in-microsoft-teams"></a>Основные ресурсы в группах Майкрософт

| Resource | Methods |
|:---------------|:--------|
|[Группа](../resources/team.md)| [список рабочих групп](../api/user-list-joinedteams.md), [список всех групп](/graph/teams-list-all-teams), [Создание](../api/team-put-teams.md), [Чтение](../api/team-get.md), [обновление](../api/team-update.md), [Удаление](/graph/api/group-delete?view=graph-rest-1.0), [клонированной](../api/team-clone.md), [архив](../api/team-archive.md), [unarchive](../api/team-unarchive.md) |
|[group](../resources/group.md)| [Добавить элемент](../api/group-post-members.md), [Удалить элемент](../api/group-delete-members.md), [Добавьте владельца](../api/group-post-owners.md), [Удалить владельца](../api/group-delete-owners.md), [Получение файлов](drive.md), [Получение записной книжки](/graph/api/resources/notebook?view=graph-rest-1.0), [Получение планы](plannergroup.md), [Получение календаря](event.md) |
|[канал](../resources/channel.md)|[список](../api/channel-list.md), [Создание](../api/channel-post.md), [Чтение](../api/channel-get.md), [обновление](../api/channel-patch.md), [Удаление](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[список](../api/teamstab-list.md), [Создание](../api/teamstab-add.md), [Чтение](../api/teamstab-get.md), [обновление](../api/teamstab-update.md), [Удаление](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[список](../api/teamsapp-list.md), [Публикация](../api/teamsapp-publish.md), [обновление](../api/teamsapp-update.md), [Удаление](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [список](../api/teamsappinstallation-list.md), [Установка](../api/teamsappinstallation-add.md), [обновление](../api/teamsappinstallation-delete.md), [Удаление](../api/teamsappinstallation-delete.md) |
| (Предварительная версия) [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) и [chatThread](/graph/api/resources/chatthread?view=graph-rest-beta) | [список](/graph/api/channel-list-messages?view=graph-rest-beta), [Создание](/graph/api/channel-post-chatthreads?view=graph-rest-beta), [Чтение](/graph/api/channel-get-message?view=graph-rest-beta) |
| (Предварительная версия) [звонок](/graph/api/resources/call?view=graph-rest-beta) | [ответ](/graph/api/call-answer?view=graph-rest-beta), [Отклонить](/graph/api/call-reject?view=graph-rest-beta), [Перенаправление](/graph/api/call-redirect?view=graph-rest-beta), [отключить звук](/graph/api/call-mute?view=graph-rest-beta), [Включение звука](/graph/api/call-unmute?view=graph-rest-beta), [обновление метаданных](/graph/api/call-updatemetadata?view=graph-rest-beta), [Изменить экрана, общий доступ к роли](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [список участников](/graph/api/call-list-participants?view=graph-rest-beta), [приглашения участников](/graph/api/participant-invite?view=graph-rest-beta), [Отключить всех участников](/graph/api/participant-muteall?view=graph-rest-beta) |

## <a name="teams-and-groups"></a>Группы и группы

В Microsoft Graph группами Майкрософт представлены [группы](../resources/group.md) ресурсов. Группы группами Майкрософт и Office 365 устранения различные потребности совместной работы групп. Почти все групповые функции применяются к группам Майкрософт и группы Office 365, например группового календаря, файлы, заметки, фотографии, планы и т. д. Основное различие между [team](team.md) и группы с Office 365 — режим обмена данными между членами. Участники группы общаться с сохраняемого чата в контексте конкретными группами. Office 365 сгруппировать элементы общаться по беседам группы, которые являются бесед электронной почты, которые происходят в контексте группы в Outlook.

Любой группы, имеющей группы имеет свойство **resourceProvisioningOptions** , содержащий «Группа». 

>**Примечание:** Свойство **Group.resourceProvisioningOptions** может быть изменено.
Не добавлять или удалять «Группа» из этой коллекции; в противном случае вы получите неверные результаты, когда список всех групп.

Ниже приведены различия между группами и группы на уровне API.

- Сохраняемый чат доступен только для групп Майкрософт. Эта функция иерархически представлены ресурсы [канала](../resources/channel.md), [chatThread](../resources/chatthread.md)и [chatMessage](../resources/chatmessage.md) .
- Групповой беседы, доступные только для группы Office 365. Эта функция иерархически представлены ресурсы [, [conversationThread](../resources/conversationthread.md)и [публиковать](../resources/post.md) ](../resources/conversation.md). 
- Метод [списка в состав группы](../api/user-list-joinedteams.md) применяется только к группами Майкрософт.
- [Звонков и собрания по сети API-интерфейсы](./calls-api-overview.md) применяются только к группами Майкрософт.
- В разделе также [Известные проблемы](/graph/known-issues) эти интерфейсы API.

>**Примечание:** Если вы используете группы API в [приложение группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/#apps-in-microsoft-teams) , а не в отдельных приложения — например как часть tab или программа-робот под управлением Microsoft групп - следуйте указаниям в статье [С помощью Microsoft Graph на страницах группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/microsoft-graph).

## <a name="membership-changes-in-microsoft-teams"></a>Изменения членства в группах Майкрософт

Чтобы добавить участников и владельцев группы, изменения членства [группы](../resources/group.md) с тем же идентификатором.

| Вариант использования      | Глагол      | URL-адрес |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Добавление члена](../api/group-post-members.md)    | POST      | параметры ref $/members/ /Groups/ {идентификатор}  |
| [Удаление члена](../api/group-delete-members.md)   | DELETE    | /members/ /Groups/ {идентификатор} {userId} / $ref |
| [Добавление владельца](../api/group-post-owners.md)     | POST       | параметры ref $/owners/ /Groups/ {идентификатор} |
| [Удаление владельца](../api/group-delete-owners.md) | DELETE    | /owners/ /Groups/ {идентификатор} {userId} / $ref |
| [Группа обновления](../api/team-update.md)  | PATCH     | /teams/ {идентификатор} |

Мы рекомендуем при добавлении владельца также добавлять этого пользователя как члена группы. Если владелец, который не является участником группы, владельца и членство в изменения могут не отображаться немедленно в группами Майкрософт. Кроме того различных приложений и интерфейсы API будет обрабатывать, по-разному. Например группами Майкрософт покажут группам, что пользователь является участником или владельца, хотя командлеты PowerShell группами Майкрософт и joinedTeams/me/API отображаются только группы, в которой находится пользователь. Чтобы избежать путаницы, добавьте всех владельцев в список участников. 

Известная проблема: при удаление /groups/ {идентификатор} аудио- и вызывается владельцев, пользователь также удаляется из /groups/ {идентификатор} / элементы списка. Чтобы обойти это, рекомендуется удалить пользователя из владельцы и участники, а затем подождите 10 секунд, затем добавить их члены.

Добавление и удаление участников и владельцев, не ввода в фигурные скобки {}, применимую к идентификатору.

| Speed | Синтаксис | 
| ------ | ----- |
| Быстро | https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| Медленное | https://graph.microsoft.com/beta/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

Аналогично Если `userId` в URL-адрес или полезных данных выражается в виде имени участника-пользователя, а не как код GUID, будет работать медленнее.

| Speed | Синтаксис | 
| ------ | ----- |
| Быстро | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| Медленное | John@example.com | 

При переводе медленнее пути, если текущий участник группы или владелец входит в систему группами Майкрософт приложений и веб-сайт, изменения будут отражены в течение часа.
Если ни один из этих пользователей вход в систему группами Майкрософт приложений и веб-сайт, изменения не будут отражены до того времени, в течение часа после их входе в.

## <a name="see-also"></a>См. также

[Обзор API группами Майкрософт](/graph/teams-concept-overview)
