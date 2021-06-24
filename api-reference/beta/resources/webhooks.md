---
title: 'Получение уведомлений об изменениях с помощью API Microsoft Graph '
description: Доставка уведомлений об изменениях клиентам.
localization_priority: Normal
author: Jumaodhiss
doc_type: conceptualPageType
ms.prod: change-notifications
ms.openlocfilehash: 59bcc9f45b34508197494da7bc807cadbf214deb
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107755"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Получение уведомлений об изменениях с помощью API Microsoft Graph 

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| [Событие][] Outlook | Изменения всех событий в почтовом ящике пользователя:<br>`/users/{id}/events` | Нет |
| [Сообщение][] Outlook | Изменения во всех сообщениях в почтовом ящике пользователя: <br>`/users/{id}/messages`<br>Изменения в сообщениях в папке «Входящие» пользователя:<br>`/users/{id}/mailFolders('inbox')/messages` | Нет |
| Личный [контакт][] Outlook | Изменения всех личных контактов в почтовом ящике пользователя:<br>`/users/{id}/contacts` | Нет |
| [Оповещение][] безопасности | Изменения в конкретном предупреждении:<br>`/security/alerts/{id}` <br>Изменения в отфильтрованных оповещениях:<br> `/security/alerts/?$filter`| Нет |
| [callRecord][] в Teams | Изменения во _всех_ записях звонков: `/communications/callRecords` | Нет |
| [Канал][] Teams  | Изменения каналов во всех командах:<br>`/teams/getAllChannels` <br>Изменения канала в определенной группе:<br>`/teams/{id}/channels` | Да |
| [chatMessage][] Teams | Изменения в сообщениях чата во всех каналах во всех командах:<br>`/teams/getAllMessages` <br>Изменения в сообщениях чата на определенном канале:<br>`/teams/{id}/channels/{id}/messages`<br>Изменения в сообщениях чата во всех чатах:<br>`/chats/getAllMessages` <br>Изменения в сообщениях чата в конкретном чате:<br>`/chats/{id}/messages` | Да |
| [conversationMember][] в Teams | Изменения членства в определенной команде:<br>`/teams/{id}/members` | Да |
| Teams [присутствия][] | Изменения в присутствии одного пользователя: `/communications/presences/{id}` <br> Изменения нескольких присутствий пользователей:<br> `/communications/presences?$filter=id in ({id},{id}...)` | Да |
| [Команда][] Teams | Изменения для любой команды в клиенте:<br>`/teams` <br>Изменения в определенной группе:<br>`/teams/{id}` | Да |
| [todoTask][] | Изменения всех задач в определенном списке задач:<br>`/me/todo/lists/{todoTaskListId}/tasks` | Нет |
| [user][] | Изменения для всех пользователей:<br>`/users` <br>Изменения для конкретного пользователя:<br>`/users/{id}`| Нет |


> **Примечание**. Любой путь ресурса, начинающийся с `/users/{id}`, может принимать `/me` для указания вошедшего пользователя.

## <a name="permissions"></a>Permissions

В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.

| Тип разрешения                        | Поддерживаемые типы ресурсов                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Делегированное — рабочая или учебная учетная запись     | [оповещение][], канал , контакт [][], разговор [,][] [conversationMember][] [][], [driveItem][], [список][] [,][]событие , группа , сообщение , пользователь [,][]присутствие , [chatMessage][] (предварительный просмотр), [команда][], [todoTask][] [][] [][] [][] |
| Делегированное — личная учетная запись Майкрософт | [контакт][], [driveItem][], [список][], [событие][], [сообщение][],[todoTask][]                                     |
| Приложение                            | [оповещения][], [][] [канал][] [,][]контакт , [driveItem][] [,][]список [,][]событие [,][]группа , сообщение , пользователь [,][] [callRecord][], [chatMessage][], [conversationMember][], [принтер][], [printTaskDefinition][], [команда][] |

## <a name="see-also"></a>См. также

- [Тип ресурса subscription](subscription.md)
- [Перечисление подписок](../api/subscription-list.md)
- [Получение подписки](../api/subscription-get.md)
- [Создание подписки](../api/subscription-post-subscriptions.md)
- [Обновление подписки](../api/subscription-update.md)
- [Удаление подписки](../api/subscription-delete.md)

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
[todoTask]: ./todoTask.md

