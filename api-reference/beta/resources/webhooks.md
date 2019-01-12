---
title: Использование Microsoft Graph API для получения уведомлений об изменении
description: Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах. Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений. Клиентские приложения используйте уведомления для обновления их состоянии после изменения. Дополнительные сведения, включая как подписывание и обработка оповещения о входящих, посвященной Set up уведомления об изменениях в пользовательских данных.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: fe571fe0a9a7c982ee7ce93b08457586134d7d91
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986139"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="27fd9-106">Использование Microsoft Graph API для получения уведомлений об изменении</span><span class="sxs-lookup"><span data-stu-id="27fd9-106">Use the Microsoft Graph API to get change notifications</span></span>

> <span data-ttu-id="27fd9-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="27fd9-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27fd9-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27fd9-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27fd9-109">Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах.</span><span class="sxs-lookup"><span data-stu-id="27fd9-109">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="27fd9-110">Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="27fd9-110">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="27fd9-111">Клиентские приложения используйте уведомления для обновления их состоянии после изменения.</span><span class="sxs-lookup"><span data-stu-id="27fd9-111">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="27fd9-112">Для получения дополнительных сведений, включая как подписаться на и обрабатывать входящие уведомления, см [уведомления об изменениях в пользовательских данных](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="27fd9-112">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="27fd9-113">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="27fd9-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="27fd9-114">Сообщения</span><span class="sxs-lookup"><span data-stu-id="27fd9-114">Messages</span></span>
- <span data-ttu-id="27fd9-115">События</span><span class="sxs-lookup"><span data-stu-id="27fd9-115">Events</span></span>
- <span data-ttu-id="27fd9-116">Контакты</span><span class="sxs-lookup"><span data-stu-id="27fd9-116">Contacts</span></span>
- <span data-ttu-id="27fd9-117">пользователи;</span><span class="sxs-lookup"><span data-stu-id="27fd9-117">Users</span></span>
- <span data-ttu-id="27fd9-118">Группы</span><span class="sxs-lookup"><span data-stu-id="27fd9-118">Groups</span></span>
- <span data-ttu-id="27fd9-119">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="27fd9-119">Group conversations</span></span>
- <span data-ttu-id="27fd9-120">Содержимое общих на OneDrive, в том числе связанных с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="27fd9-120">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="27fd9-121">Личные папки OneDrive пользователей</span><span class="sxs-lookup"><span data-stu-id="27fd9-121">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="27fd9-122">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="27fd9-122">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="27fd9-123">Permissions</span><span class="sxs-lookup"><span data-stu-id="27fd9-123">Permissions</span></span>

<span data-ttu-id="27fd9-p104">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="27fd9-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="27fd9-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27fd9-128">Permission type</span></span>                        | <span data-ttu-id="27fd9-129">Типы поддерживаемых ресурсов</span><span class="sxs-lookup"><span data-stu-id="27fd9-129">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="27fd9-130">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="27fd9-130">Delegated - work or school account</span></span>     | <span data-ttu-id="27fd9-131">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="27fd9-131">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="27fd9-132">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="27fd9-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="27fd9-133">[контактов][], [диск][], [события][], [сообщения][]</span><span class="sxs-lookup"><span data-stu-id="27fd9-133">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="27fd9-134">Application</span><span class="sxs-lookup"><span data-stu-id="27fd9-134">Application</span></span>                            | <span data-ttu-id="27fd9-135">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="27fd9-135">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="27fd9-136">См. также</span><span class="sxs-lookup"><span data-stu-id="27fd9-136">See also</span></span>

- [<span data-ttu-id="27fd9-137">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="27fd9-137">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="27fd9-138">Список подписок</span><span class="sxs-lookup"><span data-stu-id="27fd9-138">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="27fd9-139">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="27fd9-139">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="27fd9-140">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="27fd9-140">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="27fd9-141">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="27fd9-141">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="27fd9-142">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="27fd9-142">Delete subscription</span></span>](../api/subscription-delete.md)

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
