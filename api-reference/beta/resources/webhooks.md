---
title: 'Получение уведомлений об изменениях с помощью API Microsoft Graph '
description: Доставка уведомлений об изменениях клиентам.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: conceptualPageType
ms.prod: change-notifications
ms.openlocfilehash: 01ad1955be9f0a3e8680871753c50d19cd9b06ab
ms.sourcegitcommit: 84db9d70672e7a36a1130ff4f4b9baf3554d287f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2022
ms.locfileid: "66810269"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Получение уведомлений об изменениях с помощью API Microsoft Graph 

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях. Дополнительные сведения, включая сведения о подписке и обработке входящих уведомлений, см. в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks).

С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

| **Ресурс** | **Поддерживаемые пути ресурсов** | **Можно ли данные ресурсов включать в уведомления**                  |
|:----------------|:------------|:-----------------------------------------|
| [printer][] облачной печати | Изменения, когда задание печати готово к скачиванию (событие JobFetchable):<br>`/print/printers/{id}/jobs` | Нет |
| [printTaskDefinition][] облачной печати | Изменения, когда доступно допустимое задание в очереди (событие JobStarted):<br>`/print/printtaskdefinition/{id}/tasks` | Нет |
| [driveItem][]на OneDrive для бизнеса | Изменения содержимого в иерархии _корневой папки_:<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | Нет |
| [driveItem][]на OneDrive (личный) | Изменения содержимого в иерархии _любой папки_:<br>`/users/{id}/drive/root` | Нет |
| [group][] | Изменения во всех группах:<br>`/groups` <br>Изменения в конкретной группе:<br>`/groups/{id}`<br>Изменения для владельцев конкретной группы:<br>`/groups/{id}/owners`<br>Изменения для участников конкретной группы:<br>`/groups/{id}/members` | Нет |
| [список][] на [сайте][] SharePoint | `/sites/{id}/lists/{id}` | Нет |
| [Беседа][] группы Microsoft 365  | Изменения в разговорах группы:<br>`groups/{id}/conversations` | Нет |
| [Событие][] Outlook | Изменения всех событий в почтовом ящике пользователя:<br>`/users/{id}/events` | Да |
| [Сообщение][] Outlook | Изменения во всех сообщениях в почтовом ящике пользователя: <br>`/users/{id}/messages`<br>Изменения в сообщениях в папке «Входящие» пользователя:<br>`/users/{id}/mailFolders('inbox')/messages` | Да |
| Личный [контакт][] Outlook | Изменения всех личных контактов в почтовом ящике пользователя:<br>`/users/{id}/contacts` | Да |
| [Оповещение][] безопасности | Изменения в конкретном предупреждении:<br>`/security/alerts/{id}` <br>Изменения в отфильтрованных оповещениях:<br> `/security/alerts/?$filter`| Нет |
| [callRecord][] в Teams | Изменения во _всех_ записях звонков: `/communications/callRecords` | Нет |
| [Канал][] Teams  | Изменения каналов во всех командах:<br>`/teams/getAllChannels` <br>Изменения канала в определенной команде:<br>`/teams/{id}/channels` | Да |
| [Чат][] Teams | Изменения в любом чате в клиенте:<br>`/chats` <br>Изменения в конкретном чате:<br>`/chats/{id}` | Да |
| [chatMessage][] Teams | Изменения в сообщениях чата во всех каналах во всех командах:<br>`/teams/getAllMessages` <br>Изменения в сообщениях чата на определенном канале:<br>`/teams/{id}/channels/{id}/messages`<br>Изменения в сообщениях чата во всех чатах:<br>`/chats/getAllMessages` <br>Изменения в сообщениях чата в конкретном чате:<br>`/chats/{id}/messages`<br>Изменения в сообщениях чата во всех чатах, в которых участвует конкретный пользователь:<br>`/users/{id}/chats/getAllMessages` | Да |
| [conversationMember][] в Teams | Изменения участия в определенной команде:<br>`/teams/{id}/members` <br> Изменения участия в определенном чате:<br>`/chats/{id}/members` <br> Изменения участия во всех чатах:<br>`/chats/getAllMembers` <br> Изменения участия во всех каналах определенной команды:<br>`teams/{id}/channels/getAllMembers` | Да |
| [onlineMeeting][] в Teams | Изменения в собрании по сети: <br>`/communications/onlineMeetings/?$filter=JoinWebUrl eq {joinWebUrl}` | Да |
| [presence][] в Teams | Изменения в присутствии одного пользователя: `/communications/presences/{id}` <br> Изменения в присутствии нескольких пользователей:<br> `/communications/presences?$filter=id in ({id},{id}...)` | Да |
| [Команда][] Teams | Изменения в любой команде в клиенте:<br>`/teams` <br>Изменения в конкретной команде:<br>`/teams/{id}` | Да |
| To Do [baseTask][] (не рекомендуется) | Изменения всех задач в определенном списке задач:<br>`/me/tasks/lists/{baseTaskListId}/tasks`<br>Изменения всех задач:<br>`/me/tasks/lists/alltasks` | Нет |
| [Задача в приложении "Список дел"][] | Изменения всех задач в определенном списке задач:<br>`/me/todo/lists/{todoTaskListId}/tasks` | Нет |
| [user][] | Изменения для всех пользователей:<br>`/users` <br>Изменения для конкретного пользователя:<br>`/users/{id}`| Нет |


> **Примечание**. Любой путь ресурса, начинающийся с `/users/{id}`, может принимать `/me` для указания вошедшего пользователя.

## <a name="permissions"></a>Permissions

В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.

| Тип разрешения                        | Поддерживаемые типы ресурсов                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Делегированное — рабочая или учебная учетная запись     | [alert][], [baseTask][] (не [рекомендуется), канал][], [чат][][, контакт][][,][] беседа, [conversationMember][], [driveItem][], [список][], [событие][], [группа][], [сообщение][], [пользователь][], [присутствие][], [chatMessage][] (предварительная версия), [команда][], [todoTask][] |
| Делегированное — личная учетная запись Майкрософт | [baseTask][] (не рекомендуется), [contact][], [driveItem][], [list][], [event][], [message][], [todoTask][]                                   |
| Для приложений                            | [alert][], [channel][], [chat][], [contact][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][], [conversationMember][], [onlinemeeting][], [printer][], [printTaskDefinition][], [team][] |

## <a name="see-also"></a>См. также

- [Тип ресурса subscription](subscription.md)
- [Перечисление подписок](../api/subscription-list.md)
- [Получение подписки](../api/subscription-get.md)
- [Создание подписки](../api/subscription-post-subscriptions.md)
- [Обновление подписки](../api/subscription-update.md)
- [Удаление подписки](../api/subscription-delete.md)

[chat]: ./chat.md
[chatMessage]: ./chatmessage.md
[contact]: ./contact.md
[conversation]: ./conversation.md
[conversationMember]: ./conversationmember.md
[channel]: ./channel.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[callRecord]: ./callrecords-callrecord.md
[alert]: ./alert.md
[presence]: ./presence.md
[printer]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md
[team]: ./team.md
[baseTask]: ./baseTask.md
[todoTask]: ./todotask.md
[Задача в приложении "Список дел"]: ./todotask.md
[onlineMeeting]: ./onlinemeeting.md
