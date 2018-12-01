---
title: Использование Microsoft Graph API для получения уведомлений об изменении
description: Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах. Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений. Клиентские приложения используйте уведомления для обновления их состоянии после изменения. Дополнительные сведения, включая как подписывание и обработка оповещения о входящих, посвященной Set up уведомления об изменениях в пользовательских данных.
ms.openlocfilehash: c7d468b7c5064911d27d3a93bc3160d03c2a4dc3
ms.sourcegitcommit: 02ead22efd4f10cd50f89c9f5aa3b6dfda96aeec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2018
ms.locfileid: "27123947"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="6410c-106">Использование Microsoft Graph API для получения уведомлений об изменении</span><span class="sxs-lookup"><span data-stu-id="6410c-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="6410c-107">Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах.</span><span class="sxs-lookup"><span data-stu-id="6410c-107">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="6410c-108">Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6410c-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="6410c-109">Клиентские приложения используйте уведомления для обновления их состоянии после изменения.</span><span class="sxs-lookup"><span data-stu-id="6410c-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="6410c-110">Для получения дополнительных сведений, включая как подписаться на и обрабатывать входящие уведомления, см [уведомления об изменениях в пользовательских данных](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="6410c-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="6410c-111">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="6410c-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="6410c-112">Сообщения</span><span class="sxs-lookup"><span data-stu-id="6410c-112">Messages</span></span>
- <span data-ttu-id="6410c-113">События</span><span class="sxs-lookup"><span data-stu-id="6410c-113">Events</span></span>
- <span data-ttu-id="6410c-114">Контакты</span><span class="sxs-lookup"><span data-stu-id="6410c-114">Contacts</span></span>
- <span data-ttu-id="6410c-115">пользователи;</span><span class="sxs-lookup"><span data-stu-id="6410c-115">Users</span></span>
- <span data-ttu-id="6410c-116">Группы</span><span class="sxs-lookup"><span data-stu-id="6410c-116">Groups</span></span>
- <span data-ttu-id="6410c-117">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="6410c-117">Group conversations</span></span>
- <span data-ttu-id="6410c-118">Содержимое общих на OneDrive, в том числе связанных с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="6410c-118">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="6410c-119">Личные папки OneDrive пользователей</span><span class="sxs-lookup"><span data-stu-id="6410c-119">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="6410c-120">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="6410c-120">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="6410c-121">Permissions</span><span class="sxs-lookup"><span data-stu-id="6410c-121">Permissions</span></span>

<span data-ttu-id="6410c-p103">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6410c-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="6410c-126">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6410c-126">Permission type</span></span>                        | <span data-ttu-id="6410c-127">Типы поддерживаемых ресурсов</span><span class="sxs-lookup"><span data-stu-id="6410c-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="6410c-128">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="6410c-128">Delegated - work or school account</span></span>     | <span data-ttu-id="6410c-129">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="6410c-129">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="6410c-130">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="6410c-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="6410c-131">[контактов][], [диск][], [события][], [сообщения][]</span><span class="sxs-lookup"><span data-stu-id="6410c-131">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="6410c-132">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6410c-132">Application</span></span>                            | <span data-ttu-id="6410c-133">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="6410c-133">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="6410c-134">См. также</span><span class="sxs-lookup"><span data-stu-id="6410c-134">See also</span></span>

- [<span data-ttu-id="6410c-135">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="6410c-135">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="6410c-136">Список подписок</span><span class="sxs-lookup"><span data-stu-id="6410c-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="6410c-137">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="6410c-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="6410c-138">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="6410c-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="6410c-139">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="6410c-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="6410c-140">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="6410c-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
[оповещения]: ./alert.md
[alert]: ./alert.md