---
title: Использование Microsoft Graph API для получения уведомлений об изменении
description: Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах. Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений. Клиентские приложения используйте уведомления для обновления их состоянии после изменения. Дополнительные сведения, включая как подписывание и обработка оповещения о входящих, посвященной Set up уведомления об изменениях в пользовательских данных.
ms.openlocfilehash: 8be013eeee83f31a78fb5230a0de74847d8aed80
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2018
ms.locfileid: "27082895"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="8f402-106">Использование Microsoft Graph API для получения уведомлений об изменении</span><span class="sxs-lookup"><span data-stu-id="8f402-106">Use the Microsoft Graph API to get change notifications</span></span>

> <span data-ttu-id="8f402-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f402-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f402-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f402-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f402-109">Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах.</span><span class="sxs-lookup"><span data-stu-id="8f402-109">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="8f402-110">Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8f402-110">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="8f402-111">Клиентские приложения используйте уведомления для обновления их состоянии после изменения.</span><span class="sxs-lookup"><span data-stu-id="8f402-111">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="8f402-112">Для получения дополнительных сведений, включая как подписаться на и обрабатывать входящие уведомления, см [уведомления об изменениях в пользовательских данных](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="8f402-112">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="8f402-113">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="8f402-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="8f402-114">Сообщения</span><span class="sxs-lookup"><span data-stu-id="8f402-114">Messages</span></span>
- <span data-ttu-id="8f402-115">События</span><span class="sxs-lookup"><span data-stu-id="8f402-115">Events</span></span>
- <span data-ttu-id="8f402-116">Контакты</span><span class="sxs-lookup"><span data-stu-id="8f402-116">Contacts</span></span>
- <span data-ttu-id="8f402-117">пользователи;</span><span class="sxs-lookup"><span data-stu-id="8f402-117">Users</span></span>
- <span data-ttu-id="8f402-118">Группы</span><span class="sxs-lookup"><span data-stu-id="8f402-118">Groups</span></span>
- <span data-ttu-id="8f402-119">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="8f402-119">Group conversations</span></span>
- <span data-ttu-id="8f402-120">Содержимое общих на OneDrive, в том числе связанных с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="8f402-120">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="8f402-121">Личные папки OneDrive пользователей</span><span class="sxs-lookup"><span data-stu-id="8f402-121">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="8f402-122">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="8f402-122">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="8f402-123">Permissions</span><span class="sxs-lookup"><span data-stu-id="8f402-123">Permissions</span></span>

<span data-ttu-id="8f402-p104">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8f402-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="8f402-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f402-128">Permission type</span></span>                        | <span data-ttu-id="8f402-129">Типы поддерживаемых ресурсов</span><span class="sxs-lookup"><span data-stu-id="8f402-129">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="8f402-130">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="8f402-130">Delegated - work or school account</span></span>     | <span data-ttu-id="8f402-131">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="8f402-131">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="8f402-132">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="8f402-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="8f402-133">[контактов][], [диск][], [события][], [сообщения][]</span><span class="sxs-lookup"><span data-stu-id="8f402-133">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="8f402-134">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8f402-134">Application</span></span>                            | <span data-ttu-id="8f402-135">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="8f402-135">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="8f402-136">См. также</span><span class="sxs-lookup"><span data-stu-id="8f402-136">See also</span></span>

- [<span data-ttu-id="8f402-137">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="8f402-137">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="8f402-138">Список подписок</span><span class="sxs-lookup"><span data-stu-id="8f402-138">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="8f402-139">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="8f402-139">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="8f402-140">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="8f402-140">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="8f402-141">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="8f402-141">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="8f402-142">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="8f402-142">Delete subscription</span></span>](../api/subscription-delete.md)

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