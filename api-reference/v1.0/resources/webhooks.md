# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="41dd0-101">Использование Microsoft Graph API для получения уведомлений об изменении</span><span class="sxs-lookup"><span data-stu-id="41dd0-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="41dd0-102">Microsoft Graph REST API использует механизм webhook для доставки уведомлений на клиентах.</span><span class="sxs-lookup"><span data-stu-id="41dd0-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="41dd0-103">Клиент — веб-службы, который настраивает URL-адреса для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="41dd0-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="41dd0-104">Клиентские приложения используйте уведомления для обновления их состоянии после изменения.</span><span class="sxs-lookup"><span data-stu-id="41dd0-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="41dd0-105">Для получения дополнительных сведений, включая как подписаться на и обрабатывать входящие уведомления, см [уведомления об изменениях в пользовательских данных](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="41dd0-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="41dd0-106">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="41dd0-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="41dd0-107">Сообщения</span><span class="sxs-lookup"><span data-stu-id="41dd0-107">Messages</span></span>
- <span data-ttu-id="41dd0-108">События</span><span class="sxs-lookup"><span data-stu-id="41dd0-108">Events</span></span>
- <span data-ttu-id="41dd0-109">Контакты</span><span class="sxs-lookup"><span data-stu-id="41dd0-109">Contacts</span></span>
- <span data-ttu-id="41dd0-110">пользователи;</span><span class="sxs-lookup"><span data-stu-id="41dd0-110">Users</span></span>
- <span data-ttu-id="41dd0-111">Группы</span><span class="sxs-lookup"><span data-stu-id="41dd0-111">Groups</span></span>
- <span data-ttu-id="41dd0-112">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="41dd0-112">Group conversations</span></span>
- <span data-ttu-id="41dd0-113">Содержимое общих на OneDrive, в том числе связанных с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="41dd0-113">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="41dd0-114">Личные папки OneDrive пользователей</span><span class="sxs-lookup"><span data-stu-id="41dd0-114">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="41dd0-115">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="41dd0-115">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="41dd0-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41dd0-116">Permissions</span></span>

<span data-ttu-id="41dd0-p102">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription_post_subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="41dd0-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="41dd0-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41dd0-121">Permission type</span></span>                        | <span data-ttu-id="41dd0-122">Типы ресурсов, поддерживаемые в версии 1.0</span><span class="sxs-lookup"><span data-stu-id="41dd0-122">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="41dd0-123">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="41dd0-123">Delegated - work or school account</span></span>     | <span data-ttu-id="41dd0-124">[контактов][], [беседы][], [диск][], [события][], [сообщения][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="41dd0-124">[contact][], [conversation][], [drive][], [event][], [message][], [alert][]</span></span> |
| <span data-ttu-id="41dd0-125">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="41dd0-125">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="41dd0-126">Нет</span><span class="sxs-lookup"><span data-stu-id="41dd0-126">None</span></span>                                                             |
| <span data-ttu-id="41dd0-127">Application</span><span class="sxs-lookup"><span data-stu-id="41dd0-127">Application</span></span>                            | <span data-ttu-id="41dd0-128">[контактов][], [беседы][], [события][], [сообщения][], [оповещения][]</span><span class="sxs-lookup"><span data-stu-id="41dd0-128">[contact][], [conversation][], [event][], [message][], [alert][]</span></span>           |

## <a name="see-also"></a><span data-ttu-id="41dd0-129">См. также</span><span class="sxs-lookup"><span data-stu-id="41dd0-129">See also</span></span>

- [<span data-ttu-id="41dd0-130">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="41dd0-130">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="41dd0-131">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="41dd0-131">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="41dd0-132">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="41dd0-132">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="41dd0-133">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="41dd0-133">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="41dd0-134">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="41dd0-134">Delete subscription</span></span>](../api/subscription_delete.md)

[контакт]: ./contact.md
[contact]: ./contact.md
[беседа]: ./conversation.md
[conversation]: ./conversation.md
[диск]: ./drive.md
[drive]: ./drive.md
[событие]: ./event.md
[event]: ./event.md
[сообщение]: ./message.md
[message]: ./message.md
[оповещения]: ./alert.md
[alert]: ./alert.md