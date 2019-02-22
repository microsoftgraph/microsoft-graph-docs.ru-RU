---
title: Получение уведомлений об изменениях с помощью API Microsoft Graph
description: REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает собственный URL-адрес для получения уведомлений. Клиентские приложения используют Уведомления для обновления состояния после внесения изменений. Дополнительные сведения, включая сведения о том, как подписываться на входящие уведомления и обрабатывать их, можно узнать в статье Set up Notifications for Changes for User Data.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1d7a3d868ffc640f7659623942ac102575fb94fc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151494"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Получение уведомлений об изменениях с помощью API Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает собственный URL-адрес для получения уведомлений. Клиентские приложения используют Уведомления для обновления состояния после внесения изменений. Дополнительные сведения, включая сведения о том, как подписываться на входящие уведомления и обрабатывать их, можно узнать [в статье Set up Notifications for Changes for User Data](/graph/webhooks).

С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

- [Сообщение][] Outlook
- [Событие][] Outlook
- Личный [контакт][] Outlook
- [user][]
- [group][]
- Беседа группы [][] Office 365
- Контент в иерархии _любой папки_ [driveItem][] в личном OneDrive пользователя
- Контент в иерархии _корневой папки_ [driveItem][] в OneDrive для бизнеса
- [ОповещенИе][] системы безопасности

## <a name="permissions"></a>Разрешения

В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.

| Тип разрешения                        | Поддерживаемые типы ресурсов                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegated — рабочая или учебная учетная запись     | [оповещение][], [контакт][], [беседа][], [driveItem][], [событие][], [Группа][], [сообщение][], [пользователь][]|
| Delegated — личная учетная запись Майкрософт | [Contact][], [driveItem][], [event][], [Message][]                                        |
| Приложение                            | [Alert][], [Contact][], [driveItem][], [event][], [Group][], [Message][], [User][]|

## <a name="see-also"></a>См. также

- [Тип ресурса subscription](subscription.md)
- [Список подписок](../api/subscription-list.md)
- [Получение подписки](../api/subscription-get.md)
- [Создание подписки](../api/subscription-post-subscriptions.md)
- [Обновление подписки](../api/subscription-update.md)
- [Удаление подписки](../api/subscription-delete.md)

[контакт]: ./contact.md
[беседа]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[акций]: ./alert.md
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
