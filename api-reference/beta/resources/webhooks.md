---
title: 'Получение уведомлений об изменениях с помощью API Microsoft Graph '
description: REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях. Дополнительные сведения, включая сведения о подписке и обработке входящих уведомлений, см. в статье "Настройка уведомлений об изменениях в пользовательских данных".
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 8422328061ac1c2ad736435204b699544bffd2ed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341507"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="8c1b3-106">Получение уведомлений об изменениях с помощью API Microsoft Graph </span><span class="sxs-lookup"><span data-stu-id="8c1b3-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c1b3-107">REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам.</span><span class="sxs-lookup"><span data-stu-id="8c1b3-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="8c1b3-108">Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8c1b3-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="8c1b3-109">С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях.</span><span class="sxs-lookup"><span data-stu-id="8c1b3-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="8c1b3-110">Дополнительные сведения, включая сведения о подписке и обработке входящих уведомлений, см. в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="8c1b3-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="8c1b3-111">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="8c1b3-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="8c1b3-112">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="8c1b3-112">Outlook [message][]</span></span>
- <span data-ttu-id="8c1b3-113">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="8c1b3-113">Outlook [event][]</span></span>
- <span data-ttu-id="8c1b3-114">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="8c1b3-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="8c1b3-115">[user][]</span><span class="sxs-lookup"><span data-stu-id="8c1b3-115">[user][]</span></span>
- <span data-ttu-id="8c1b3-116">[group][]</span><span class="sxs-lookup"><span data-stu-id="8c1b3-116">[group][]</span></span>
- <span data-ttu-id="8c1b3-117">Групповой [чат][] Office 365 </span><span class="sxs-lookup"><span data-stu-id="8c1b3-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="8c1b3-118">Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="8c1b3-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="8c1b3-119">Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="8c1b3-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="8c1b3-120">[Оповещение][] безопасности</span><span class="sxs-lookup"><span data-stu-id="8c1b3-120">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="8c1b3-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c1b3-121">Permissions</span></span>

<span data-ttu-id="8c1b3-p103">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8c1b3-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="8c1b3-126">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c1b3-126">Permission type</span></span>                        | <span data-ttu-id="8c1b3-127">Поддерживаемые типы ресурсов</span><span class="sxs-lookup"><span data-stu-id="8c1b3-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="8c1b3-128">Делегированное — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="8c1b3-128">Delegated - work or school account</span></span>     | <span data-ttu-id="8c1b3-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span><span class="sxs-lookup"><span data-stu-id="8c1b3-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="8c1b3-130">Делегированное — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="8c1b3-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="8c1b3-131">[contact][], [driveItem][], [event][], [message][]</span><span class="sxs-lookup"><span data-stu-id="8c1b3-131">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="8c1b3-132">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c1b3-132">Application</span></span>                            | <span data-ttu-id="8c1b3-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span><span class="sxs-lookup"><span data-stu-id="8c1b3-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="8c1b3-134">См. также</span><span class="sxs-lookup"><span data-stu-id="8c1b3-134">See also</span></span>

- [<span data-ttu-id="8c1b3-135">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="8c1b3-135">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="8c1b3-136">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="8c1b3-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="8c1b3-137">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="8c1b3-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="8c1b3-138">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="8c1b3-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="8c1b3-139">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="8c1b3-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="8c1b3-140">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="8c1b3-140">Delete subscription</span></span>](../api/subscription-delete.md)

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
