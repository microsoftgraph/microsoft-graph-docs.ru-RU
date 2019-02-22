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
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="f2a1c-106">Получение уведомлений об изменениях с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f2a1c-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2a1c-107">REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам.</span><span class="sxs-lookup"><span data-stu-id="f2a1c-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="f2a1c-108">Клиент — это веб-служба, которая настраивает собственный URL-адрес для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f2a1c-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="f2a1c-109">Клиентские приложения используют Уведомления для обновления состояния после внесения изменений.</span><span class="sxs-lookup"><span data-stu-id="f2a1c-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="f2a1c-110">Дополнительные сведения, включая сведения о том, как подписываться на входящие уведомления и обрабатывать их, можно узнать [в статье Set up Notifications for Changes for User Data](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="f2a1c-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="f2a1c-111">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="f2a1c-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="f2a1c-112">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="f2a1c-112">Outlook [message][]</span></span>
- <span data-ttu-id="f2a1c-113">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="f2a1c-113">Outlook [event][]</span></span>
- <span data-ttu-id="f2a1c-114">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="f2a1c-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="f2a1c-115">[user][]</span><span class="sxs-lookup"><span data-stu-id="f2a1c-115">[user][]</span></span>
- <span data-ttu-id="f2a1c-116">[group][]</span><span class="sxs-lookup"><span data-stu-id="f2a1c-116">[group][]</span></span>
- <span data-ttu-id="f2a1c-117">Беседа группы [][] Office 365</span><span class="sxs-lookup"><span data-stu-id="f2a1c-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="f2a1c-118">Контент в иерархии _любой папки_ [driveItem][] в личном OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="f2a1c-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="f2a1c-119">Контент в иерархии _корневой папки_ [driveItem][] в OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="f2a1c-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="f2a1c-120">[ОповещенИе][] системы безопасности</span><span class="sxs-lookup"><span data-stu-id="f2a1c-120">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="f2a1c-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2a1c-121">Permissions</span></span>

<span data-ttu-id="f2a1c-p103">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f2a1c-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="f2a1c-126">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2a1c-126">Permission type</span></span>                        | <span data-ttu-id="f2a1c-127">Поддерживаемые типы ресурсов</span><span class="sxs-lookup"><span data-stu-id="f2a1c-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="f2a1c-128">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="f2a1c-128">Delegated - work or school account</span></span>     | <span data-ttu-id="f2a1c-129">[оповещение][], [контакт][], [беседа][], [driveItem][], [событие][], [Группа][], [сообщение][], [пользователь][]</span><span class="sxs-lookup"><span data-stu-id="f2a1c-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="f2a1c-130">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="f2a1c-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="f2a1c-131">[Contact][], [driveItem][], [event][], [Message][]</span><span class="sxs-lookup"><span data-stu-id="f2a1c-131">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="f2a1c-132">Приложение</span><span class="sxs-lookup"><span data-stu-id="f2a1c-132">Application</span></span>                            | <span data-ttu-id="f2a1c-133">[Alert][], [Contact][], [driveItem][], [event][], [Group][], [Message][], [User][]</span><span class="sxs-lookup"><span data-stu-id="f2a1c-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="f2a1c-134">См. также</span><span class="sxs-lookup"><span data-stu-id="f2a1c-134">See also</span></span>

- [<span data-ttu-id="f2a1c-135">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="f2a1c-135">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="f2a1c-136">Список подписок</span><span class="sxs-lookup"><span data-stu-id="f2a1c-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="f2a1c-137">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="f2a1c-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="f2a1c-138">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="f2a1c-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="f2a1c-139">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="f2a1c-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="f2a1c-140">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="f2a1c-140">Delete subscription</span></span>](../api/subscription-delete.md)

[контакт]: ./contact.md
[contact]: ./contact.md
[беседа]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[акций]: ./alert.md
[alert]: ./alert.md
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
