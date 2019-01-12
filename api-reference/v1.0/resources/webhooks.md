---
title: Использование Microsoft Graph API для получения уведомлений об изменении
description: Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах. Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений. Клиентские приложения используйте уведомления для обновления их состоянии после изменения. Дополнительные сведения, включая как подписывание и обработка оповещения о входящих, посвященной Set up уведомления об изменениях в пользовательских данных.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: cb522c50b2cd9fec007dd32d4257dd68fc56ea6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981415"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="026ab-106">Использование Microsoft Graph API для получения уведомлений об изменении</span><span class="sxs-lookup"><span data-stu-id="026ab-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="026ab-107">Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах.</span><span class="sxs-lookup"><span data-stu-id="026ab-107">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="026ab-108">Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="026ab-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="026ab-109">Клиентские приложения используйте уведомления для обновления их состоянии после изменения.</span><span class="sxs-lookup"><span data-stu-id="026ab-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="026ab-110">Для получения дополнительных сведений, включая как подписаться на и обрабатывать входящие уведомления, см [уведомления об изменениях в пользовательских данных](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="026ab-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="026ab-111">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="026ab-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="026ab-112">Сообщения</span><span class="sxs-lookup"><span data-stu-id="026ab-112">Messages</span></span>
- <span data-ttu-id="026ab-113">События</span><span class="sxs-lookup"><span data-stu-id="026ab-113">Events</span></span>
- <span data-ttu-id="026ab-114">Контакты</span><span class="sxs-lookup"><span data-stu-id="026ab-114">Contacts</span></span>
- <span data-ttu-id="026ab-115">пользователи;</span><span class="sxs-lookup"><span data-stu-id="026ab-115">Users</span></span>
- <span data-ttu-id="026ab-116">Группы</span><span class="sxs-lookup"><span data-stu-id="026ab-116">Groups</span></span>
- <span data-ttu-id="026ab-117">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="026ab-117">Group conversations</span></span>
- <span data-ttu-id="026ab-118">Содержимое общих на OneDrive, в том числе связанных с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="026ab-118">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="026ab-119">Личные папки OneDrive пользователей</span><span class="sxs-lookup"><span data-stu-id="026ab-119">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="026ab-120">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="026ab-120">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="026ab-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="026ab-121">Permissions</span></span>

<span data-ttu-id="026ab-p103">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription-post-subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="026ab-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="026ab-126">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="026ab-126">Permission type</span></span>                        | <span data-ttu-id="026ab-127">Типы поддерживаемых ресурсов</span><span class="sxs-lookup"><span data-stu-id="026ab-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="026ab-128">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="026ab-128">Delegated - work or school account</span></span>     | <span data-ttu-id="026ab-129">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="026ab-129">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="026ab-130">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="026ab-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="026ab-131">[контактов][], [диск][], [события][], [сообщения][]</span><span class="sxs-lookup"><span data-stu-id="026ab-131">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="026ab-132">Приложение</span><span class="sxs-lookup"><span data-stu-id="026ab-132">Application</span></span>                            | <span data-ttu-id="026ab-133">[контактов][], [беседы][], [диск][], [события][], [группы][], [сообщение][], [пользователь][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="026ab-133">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="026ab-134">См. также</span><span class="sxs-lookup"><span data-stu-id="026ab-134">See also</span></span>

- [<span data-ttu-id="026ab-135">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="026ab-135">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="026ab-136">Список подписок</span><span class="sxs-lookup"><span data-stu-id="026ab-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="026ab-137">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="026ab-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="026ab-138">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="026ab-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="026ab-139">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="026ab-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="026ab-140">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="026ab-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
