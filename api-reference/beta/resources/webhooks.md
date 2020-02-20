---
title: 'Получение уведомлений об изменениях с помощью API Microsoft Graph '
description: REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях. Дополнительные сведения, включая сведения о подписке и обработке входящих уведомлений, см. в статье "Настройка уведомлений об изменениях в пользовательских данных".
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: a2389044671be071cf1d43dcd788519ee49d6363
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159026"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Получение уведомлений об изменениях с помощью API Microsoft Graph 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях. Дополнительные сведения, включая сведения о подписке и обработке входящих уведомлений, см. в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks).

С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

| **Resource** | **Поддерживаемые пути к ресурсам** | **Данные ресурсов можно включать в уведомления**                  |
|:----------------|:------------|:-----------------------------------------|
| [Сообщение][] Outlook | `/users/{id}/messages`<br>`/users/{id}/mailFolders('inbox')/messages` | Нет |
| [Событие][] Outlook | `/users/{id}/events` | Нет |
| Личный [контакт][] Outlook | `/users/{id}/contacts` | Нет |
| [user][] | `/users`(изменения для всех пользователей)<br>`/users/{id}`(изменения определенного пользователя) | Нет |
| [group][] | `/groups`(изменения всех групп)<br>`/groups/{id}`(изменения в определенной группе) | Нет |
| Групповой [чат][] Office 365  | `groups/{id}/conversations` | Нет |
| Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя | `/me/drive/root` | Нет |
| Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса | `/drives/{id}/root`<br> `/me/drive/root` | Нет |
| [Оповещение][] безопасности | `/security/alerts/{id}`(изменения в определенном оповещении) <br> `/security/alerts/?$filter`(изменения в фильтруемых оповещениях)| Нет |
| [Chatmessage](/graph/api/resources/subscription?view=graph-rest-beta) Teams | `/teams/allMessages`(сообщения во всех каналах в Teams)<br>`/teams/{id}/channels/{id}/messages`(сообщения в определенном канале);<br>`/chats/allMessages`(сообщения во всех беседах)<br>`/chats/{id}/messages`(сообщения в определенном сеансе чата) | Да |

> **Note**: любой путь к ресурсу, `/users/{id}` который начинается с `/me` , может также принять ссылку на пользователя, выполнившего вход в систему.

## <a name="permissions"></a>Разрешения

В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.

| Тип разрешения                        | Поддерживаемые типы ресурсов                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Делегированное — рабочая или учебная учетная запись     | [alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]|
| Делегированное — личная учетная запись Майкрософт | [contact][], [driveItem][], [event][], [message][]                                        |
| Для приложений                            | [Alert][], [Contact][], [driveItem][], [event][], [Group][], [Message][], [User][], [chatMessage][]|

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
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
