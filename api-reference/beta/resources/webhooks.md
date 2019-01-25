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
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="295bb-106">Использование Microsoft Graph API для получения уведомлений об изменении</span><span class="sxs-lookup"><span data-stu-id="295bb-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="295bb-107">Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах.</span><span class="sxs-lookup"><span data-stu-id="295bb-107">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="295bb-108">Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="295bb-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="295bb-109">Клиентские приложения используйте уведомления для обновления их состоянии после изменения.</span><span class="sxs-lookup"><span data-stu-id="295bb-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="295bb-110">Для получения дополнительных сведений, включая как подписаться на и обрабатывать входящие уведомления, см [уведомления об изменениях в пользовательских данных](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="295bb-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="295bb-111">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="295bb-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="295bb-112">Сообщения</span><span class="sxs-lookup"><span data-stu-id="295bb-112">Messages</span></span>
- <span data-ttu-id="295bb-113">События</span><span class="sxs-lookup"><span data-stu-id="295bb-113">Events</span></span>
- <span data-ttu-id="295bb-114">Контакты</span><span class="sxs-lookup"><span data-stu-id="295bb-114">Contacts</span></span>
- <span data-ttu-id="295bb-115">пользователи;</span><span class="sxs-lookup"><span data-stu-id="295bb-115">Users</span></span>
- <span data-ttu-id="295bb-116">Группы</span><span class="sxs-lookup"><span data-stu-id="295bb-116">Groups</span></span>
- <span data-ttu-id="295bb-117">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="295bb-117">Group conversations</span></span>
- <span data-ttu-id="295bb-118">Контент с общим доступом в OneDrive, включая диски, сопоставленные с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="295bb-118">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="295bb-119">Личные папки пользователя в OneDrive</span><span class="sxs-lookup"><span data-stu-id="295bb-119">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="295bb-120">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="295bb-120">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="295bb-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="295bb-121">Permissions</span></span>

<span data-ttu-id="295bb-p103">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="295bb-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="295bb-126">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="295bb-126">Permission type</span></span>                        | <span data-ttu-id="295bb-127">Типы поддерживаемых ресурсов</span><span class="sxs-lookup"><span data-stu-id="295bb-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="295bb-128">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="295bb-128">Delegated - work or school account</span></span>     | <span data-ttu-id="295bb-129">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="295bb-129">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="295bb-130">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="295bb-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="295bb-131">[контактов][], [диск][], [события][], [сообщения][]</span><span class="sxs-lookup"><span data-stu-id="295bb-131">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="295bb-132">Для приложений</span><span class="sxs-lookup"><span data-stu-id="295bb-132">Application</span></span>                            | <span data-ttu-id="295bb-133">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="295bb-133">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="295bb-134">См. также</span><span class="sxs-lookup"><span data-stu-id="295bb-134">See also</span></span>

- [<span data-ttu-id="295bb-135">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="295bb-135">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="295bb-136">Список подписок</span><span class="sxs-lookup"><span data-stu-id="295bb-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="295bb-137">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="295bb-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="295bb-138">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="295bb-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="295bb-139">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="295bb-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="295bb-140">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="295bb-140">Delete subscription</span></span>](../api/subscription-delete.md)

[контакт]: ./contact.md
[contact]: ./contact.md
[беседа]: ./conversation.md
[conversation]: ./conversation.md
[диск]: ./drive.md
[drive]: ./drive.md
[событие]: ./event.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
<span data-ttu-id="295bb-148">Alert</span><span class="sxs-lookup"><span data-stu-id="295bb-148">[alert]: ./alert.md</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
