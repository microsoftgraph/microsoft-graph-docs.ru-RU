---
title: 'Получение уведомлений об изменениях с помощью API Microsoft Graph '
description: REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях. Дополнительные сведения, включая сведения о подписке и обработке входящих уведомлений, см. в статье "Настройка уведомлений об изменениях в пользовательских данных".
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: aa8bcf293c0b85c242a442961e07e81fb6f9a818
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519444"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Получение уведомлений об изменениях с помощью API Microsoft Graph 

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях. Дополнительные сведения, включая сведения о подписке и обработке входящих уведомлений, см. в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks).

С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

| **Ресурс** | **Поддерживаемые пути ресурсов** | **Можно ли данные ресурсов включать в уведомления**                  |
|:----------------|:------------|:-----------------------------------------|
| [Сообщение][] Outlook | Изменения во всех сообщениях в почтовом ящике пользователя: <br>`/users/{id}/messages`<br>Изменения в сообщениях в папке «Входящие» пользователя:<br>`/users/{id}/mailFolders('inbox')/messages` | Нет |
| [Событие][] Outlook | Изменения всех событий в почтовом ящике пользователя:<br>`/users/{id}/events` | Нет |
| Личный [контакт][] Outlook | Изменения всех личных контактов в почтовом ящике пользователя:<br>`/users/{id}/contacts` | Нет |
| [user][] | Изменения для всех пользователей:<br>`/users` <br>Изменения для конкретного пользователя:<br>`/users/{id}`| Нет |
| [group][] | Изменения во всех группах:<br>`/groups` <br>Изменения в конкретной группе:<br>`/groups/{id}` | Нет |
| Групповой [чат][] Office 365  | Изменения в разговорах группы:<br>`groups/{id}/conversations` | Нет |
| [driveItem][]на OneDrive (личный) | Изменения содержимого в иерархии _любой папки_:<br>`/users/{id}/drive/root` | Нет |
| [driveItem][]на OneDrive для бизнеса | Изменения содержимого в иерархии _корневой папки_:<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | Нет |
| [список][] на [сайте][] SharePoint | `/sites/{id}/lists/{id}` | Нет |
| [Оповещение][] безопасности | Изменения в конкретном предупреждении:<br>`/security/alerts/{id}` <br>Изменения в отфильтрованных оповещениях:<br> `/security/alerts/?$filter`| Нет |
| [Каллрекорд][] Teams | Изменения _всех_ записей вызовов:`/communications/callRecords` | Нет |
| [chatMessage](/graph/api/resources/subscription?view=graph-rest-beta) Teams | Изменения в сообщениях чата во всех каналах во всех командах:<br>`/teams/allMessages` <br>Изменения в сообщениях чата на определенном канале:<br>`/teams/{id}/channels/{id}/messages`<br>Изменения в сообщениях чата во всех чатах:<br>`/chats/allMessages` <br>Изменения в сообщениях чата в конкретном чате:<br>`/chats/{id}/messages` | Да |

> **Примечание**. Любой путь ресурса, начинающийся с `/users/{id}`, может принимать `/me` для указания вошедшего пользователя.

## <a name="permissions"></a>Permissions

В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.

| Тип разрешения                        | Поддерживаемые типы ресурсов                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Делегированное — рабочая или учебная учетная запись     | [alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][]|
| Делегированное — личная учетная запись Майкрософт | [contact][], [driveItem][], [list][], [event][], [message][]                                        |
| Для приложения                            | [Alert][], [Contact][], [driveItem][], [List][], [event][], [Group][], [Message][], [User][], [каллрекорд][], [chatMessage][]|

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
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[callRecord]: ./callrecords-callrecord.md
[alert]: ./alert.md
