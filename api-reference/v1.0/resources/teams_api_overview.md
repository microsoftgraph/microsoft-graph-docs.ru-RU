# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Работа с Microsoft Teams при помощи API Microsoft Graph



Группами Майкрософт — это рабочая область на основе чата в Office 365, который предоставляет встроенные доступ к календарей конкретных групп, файлы, заметки OneNote, планировщик работы планы и др.

## <a name="key-resources-in-microsoft-teams"></a>Основные ресурсы в группах Майкрософт

| Resource | Methods |
|:---------------|:--------|
|[Группа](../resources/team.md)| [список рабочих групп](../api/user_list_joinedteams.md), [список всех групп](../../../concepts/teams_list_all_teams.md), [Создание](../api/team_put_teams.md), [Чтение](../api/team_get.md), [обновление](../api/team_update.md), [Удаление](../../v1.0/api/group_delete.md), [клонированной](../api/team_clone.md), [архив](../api/team_archive.md), [unarchive](../api/team_unarchive.md) |
|[group](../resources/group.md)| [Добавить элемент](../api/group_post_members.md), [Удалить элемент](../api/group_delete_members.md), [Добавьте владельца](../api/group_post_owners.md), [Удалить владельца](../api/group_delete_owners.md), [Получение файлов](drive.md), [Получение записной книжки](../../v1.0/resources/notebook.md), [Получение планы](plannergroup.md), [Получение календаря](event.md) |
|[канал](../resources/channel.md)|[список](../api/channel_list.md), [Создание](../api/channel_post.md), [Чтение](../api/channel_get.md), [обновление](../api/channel_patch.md), [Удаление](../api/channel_delete.md)|
|[teamsTab](../resources/teamstab.md) |[список](../api/teamstab_list.md), [Создание](../api/teamstab_add.md), [Чтение](../api/teamstab_get.md), [обновление](../api/teamstab_update.md), [Удаление](../api/teamstab_delete.md) |
|[teamsApp](../resources/teamsapp.md)|[список](../api/teamsapp_list.md), [Публикация](../api/teamsapp_publish.md), [обновление](../api/teamsapp_update.md), [Удаление](../api/teamsapp_delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [список](../api/teamsappinstallation_list.md), [Установка](../api/teamsappinstallation_add.md), [обновление](../api/teamsappinstallation_delete.md), [Удаление](../api/teamsappinstallation_delete.md) |
| (Предварительная версия) [chatMessage](../../beta/resources/chatmessage.md) и [chatThread](../../beta/resources/chatthread.md) | [список](../../beta/api/channel_list_messages.md), [Создание](../../beta/api/channel_post_chatthreads.md), [Чтение](../../beta/api/channel_get_message.md) |
| (Предварительная версия) [звонок](../../beta/resources/call.md) | [ответ](../../beta/api/call_answer.md), [Отклонить](../../beta/api/call_reject.md), [Перенаправление](../../beta/api/call_redirect.md), [отключить звук](../../beta/api/call_mute.md), [Включение звука](../../beta/api/call_unmute.md), [обновление метаданных](../../beta/api/call_updatemetadata.md), [Изменить экрана, общий доступ к роли](../../beta/api/call_changescreensharingrole.md), [список участников](../../beta/api/call_list_participants.md), [приглашения участников](../../beta/api/participant_invite.md), [Отключить всех участников](../../beta/api/participant_muteall.md) |

## <a name="teams-and-groups"></a>Группы и группы

В Microsoft Graph группами Майкрософт представлены [группы](../resources/group.md) ресурсов. Группы группами Майкрософт и Office 365 устранения различные потребности совместной работы групп. Почти все групповые функции применяются к группам Майкрософт и группы Office 365, например группового календаря, файлы, заметки, фотографии, планы и т. д. Основное различие между [team](team.md) и группы с Office 365 — режим обмена данными между членами. Участники группы общаться с сохраняемого чата в контексте конкретными группами. Office 365 сгруппировать элементы общаться по беседам группы, которые являются бесед электронной почты, которые происходят в контексте группы в Outlook.

Любой группы, имеющей группы имеет свойство **resourceProvisioningOptions** , содержащий «Группа». 

>**Примечание:** Свойство **Group.resourceProvisioningOptions** может быть изменено.
Не добавлять или удалять «Группа» из этой коллекции; в противном случае вы получите неверные результаты, когда список всех групп.

Ниже приведены различия между группами и группы на уровне API.

- Метод [списка в состав группы](../api/user_list_joinedteams.md) применяется только к группами Майкрософт.
- В разделе также [Известные проблемы](../../../concepts/known_issues.md) эти интерфейсы API.

>**Примечание:** Если вы используете группы API в [приложение группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/#apps-in-microsoft-teams) , а не в отдельных приложения — например как часть tab или программа-робот под управлением Microsoft групп - следуйте указаниям в статье [С помощью Microsoft Graph на страницах группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/microsoft-graph).

## <a name="membership-changes-in-microsoft-teams"></a>Изменения членства в группах Майкрософт

Чтобы добавить участников и владельцев группы, изменения членства [группы](../resources/group.md) с тем же идентификатором.

| Вариант использования      | Глагол      | URL-адрес |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Добавление члена](../api/group_post_members.md)    | POST      | параметры ref $/members/ /Groups/ {идентификатор}  |
| [Удаление члена](../api/group_delete_members.md)   | DELETE    | /members/ /Groups/ {идентификатор} {userId} / $ref |
| [Добавление владельца](../api/group_post_owners.md)     | POST       | параметры ref $/owners/ /Groups/ {идентификатор} |
| [Удаление владельца](../api/group_delete_owners.md) | DELETE    | /owners/ /Groups/ {идентификатор} {userId} / $ref |
| [Группа обновления](../api/team_update.md)  | PATCH     | /teams/ {идентификатор} |

Мы рекомендуем при добавлении владельца также добавлять этого пользователя как члена группы. Если владелец, который не является участником группы, владельца и членство в изменения могут не отображаться немедленно в группами Майкрософт. Кроме того различных приложений и интерфейсы API будет обрабатывать, по-разному. Например группами Майкрософт покажут группам, что пользователь является участником или владельца, хотя командлеты PowerShell группами Майкрософт и joinedTeams/me/API отображаются только группы, в которой находится пользователь. Чтобы избежать путаницы, добавьте всех владельцев в список участников. 

Известная проблема: при удаление /groups/ {идентификатор} аудио- и вызывается владельцев, пользователь также удаляется из /groups/ {идентификатор} / элементы списка. Чтобы обойти это, рекомендуется удалить пользователя из владельцы и участники, а затем подождите 10 секунд, затем добавить их члены.

Добавление и удаление участников и владельцев, не ввода в фигурные скобки {}, применимую к идентификатору.

| Speed | Синтаксис | 
| ------ | ----- |
| Быстро | https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| Медленное | https://graph.microsoft.com/v1.0/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

Аналогично Если `userId` в URL-адрес или полезных данных выражается в виде имени участника-пользователя, а не как код GUID, будет работать медленнее.

| Speed | Синтаксис | 
| ------ | ----- |
| Быстро | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| Медленное | John@example.com | 

При переводе медленнее пути, если текущий участник группы или владелец входит в систему группами Майкрософт приложений и веб-сайт, изменения будут отражены в течение часа.
Если ни один из этих пользователей вход в систему группами Майкрософт приложений и веб-сайт, изменения не будут отражены до того времени, в течение часа после их входе в.

## <a name="see-also"></a>См. также

- [Обзор API группами Майкрософт](../../../concepts/teams-concept-overview.md)
- Пример кода: [Авиакомпании Contoso](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [мини примеров C#](https://github.com/microsoftgraph/csharp-teams-sample-graph)
