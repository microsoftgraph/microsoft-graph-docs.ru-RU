---
title: 'Получение уведомлений об изменениях с помощью API Microsoft Graph '
description: Доставка уведомлений об изменениях клиентам.
ms.localizationpriority: high
author: Jumaodhiss
ms.prod: change-notifications
doc_type: conceptualPageType
ms.openlocfilehash: d76959a962da2ae13c05c5ac042aa63bca6da317
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821129"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Получение уведомлений об изменениях с помощью API Microsoft Graph 

Пространство имен: microsoft.graph

REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях. Дополнительные сведения, включая сведения о подписке и обработке входящих уведомлений, см. в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks).

С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

| **Ресурс** | **Поддерживаемые пути ресурсов** | **Можно ли данные ресурсов включать в уведомления**                  |
|:----------------|:------------|:-----------------------------------------|
| [printer][] облачной печати | Изменения, когда задание печати готово к скачиванию (событие JobFetchable):<br>`/print/printers/{id}/jobs` | Нет |
| [printTaskDefinition][] облачной печати | Изменения, когда доступно допустимое задание в очереди (событие JobStarted):<br>`/print/printtaskdefinition/{id}/tasks` | Нет |
| [Сообщение][] Outlook | Изменения во всех сообщениях в почтовом ящике пользователя: <br>`/users/{id}/messages`<br>Изменения в сообщениях в папке «Входящие» пользователя:<br>`/users/{id}/mailFolders('inbox')/messages` | Нет |
| [Событие][] Outlook | Изменения всех событий в почтовом ящике пользователя:<br>`/users/{id}/events` | Нет |
| Личный [контакт][] Outlook | Изменения всех личных контактов в почтовом ящике пользователя:<br>`/users/{id}/contacts` | Нет |
| [user][] | Изменения для всех пользователей:<br>`/users` <br>Изменения для конкретного пользователя:<br>`/users/{id}`| Нет |
| [group][] | Изменения во всех группах:<br>`/groups` <br>Изменения в конкретной группе:<br>`/groups/{id}`<br>Изменения для владельцев конкретной группы:<br>`/groups/{id}/owners`<br>Изменения для участников конкретной группы:<br>`/groups/{id}/members`  | Нет |
| [Беседа][] группы Microsoft 365  | Изменения в разговорах группы:<br>`groups/{id}/conversations` | Нет |
| [driveItem][]на OneDrive (личный) | Изменения содержимого в иерархии _любой папки_:<br>`/users/{id}/drive/root` | Нет |
| [driveItem][]на OneDrive для бизнеса | Изменения содержимого в иерархии _корневой папки_:<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | Нет |
| [список][] на [сайте][] SharePoint | Изменения содержимого в _списке_: <br>`/sites/{id}/lists/{id}` | Нет |
| [Оповещение][] безопасности | Изменения в конкретном предупреждении:<br>`/security/alerts/{id}` <br>Изменения в отфильтрованных оповещениях:<br> `/security/alerts/?$filter`| Нет |
| [callRecord][] в Teams | Изменения во _всех_ записях звонков: `/communications/callRecords` | Нет |
| [chatMessage][] Teams | Изменения в сообщениях чата во всех каналах во всех командах:<br>`/teams/getAllMessages` <br>Изменения в сообщениях чата на определенном канале:<br>`/teams/{id}/channels/{id}/messages`<br>Изменения в сообщениях чата во всех чатах:<br>`/chats/getAllMessages` <br>Изменения в сообщениях чата в конкретном чате:<br>`/chats/{id}/messages` | Да |
| [Задача в приложении "Список дел"][] | Изменения всех задач в определенном списке задач:<br>`/me/todo/lists/{todoTaskListId}/tasks`<br>Изменения всех задач:<br>`/me/todo/lists/alltasks` | Нет |

> **Примечание**. Любой путь ресурса, начинающийся с `/users/{id}`, может принимать `/me` для указания вошедшего пользователя.

## <a name="permissions"></a>Permissions

В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.

| Тип разрешения                        | Поддерживаемые типы ресурсов                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Делегированное — рабочая или учебная учетная запись     | [alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [todoTask][], [user][]|
| Делегированное — личная учетная запись Майкрософт | [contact][], [driveItem][], [list][], [event][], [message][], [todoTask][]                                       |
| Приложение                            | [alert][], [contact][], [list][], [driveItem][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][], [printer][], [printTaskDefinition][]|


## <a name="see-also"></a>См. также

- [Тип ресурса subscription](./subscription.md)
- [Перечисление подписок](../api/subscription-list.md)
- [Получение подписки](../api/subscription-get.md)
- [Создание подписки](../api/subscription-post-subscriptions.md)
- [Обновление подписки](../api/subscription-update.md)
- [Удаление подписки](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[callRecord]: ./callrecords-callrecord.md
[alert]: ./alert.md
[printer]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md
[Задача в приложении "Список дел"]: ./todotask.md
[todoTask]: ./todotask.md

