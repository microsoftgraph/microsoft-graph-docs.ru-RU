---
title: Использование Microsoft Graph API для получения уведомлений об изменении
description: Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах. Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений. Клиентские приложения используйте уведомления для обновления их состоянии после изменения. Дополнительные сведения, включая как подписывание и обработка оповещения о входящих, посвященной Set up уведомления об изменениях в пользовательских данных.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 02ab18d3fa8980211a4937433ad1616b0629bf8c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526216"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Использование Microsoft Graph API для получения уведомлений об изменении

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах. Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений. Клиентские приложения используйте уведомления для обновления их состоянии после изменения. Для получения дополнительных сведений, включая как подписаться на и обрабатывать входящие уведомления, см [уведомления об изменениях в пользовательских данных](/graph/webhooks).

С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

- Сообщения
- События
- Контакты
- пользователи;
- Группы
- Беседы группы
- Контент с общим доступом в OneDrive, включая диски, сопоставленные с сайтами SharePoint
- Личные папки пользователя в OneDrive
- Оповещения системы безопасности

## <a name="permissions"></a>Разрешения

В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.

| Тип разрешения                        | Типы поддерживаемых ресурсов                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegated — рабочая или учебная учетная запись     | [контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][] |
| Delegated — личная учетная запись Майкрософт | [контактов][], [диск][], [события][], [сообщения][]                                        |
| Для приложений                            | [контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][] |

## <a name="see-also"></a>См. также

- [Тип ресурса subscription](subscription.md)
- [Список подписок](../api/subscription-list.md)
- [Получение подписки](../api/subscription-get.md)
- [Создание подписки](../api/subscription-post-subscriptions.md)
- [Обновление подписки](../api/subscription-update.md)
- [Удаление подписки](../api/subscription-delete.md)

[контакт]: ./contact.md
[беседа]: ./conversation.md
[диск]: ./drive.md
[событие]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
Alert
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
