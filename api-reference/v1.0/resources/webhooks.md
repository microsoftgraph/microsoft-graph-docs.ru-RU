# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="e91ec-101">Использование Microsoft Graph для получения уведомлений об изменениях</span><span class="sxs-lookup"><span data-stu-id="e91ec-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="e91ec-102">API REST Microsoft Graph использует механизм веб-перехватчика для доставки уведомлений клиентам.</span><span class="sxs-lookup"><span data-stu-id="e91ec-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="e91ec-103">Клиент — это веб-служба, которая настраивает собственные URL-адреса для получения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="e91ec-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="e91ec-104">Клиентские приложения используйте уведомления для обновления своего состояния после изменений.</span><span class="sxs-lookup"><span data-stu-id="e91ec-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="e91ec-105">Для получения дополнительных сведений, в том числе о том, как подписаться на входящие уведомления и обрабатывать их, см. статью[Настройка уведомлений для изменения данных пользователя](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="e91ec-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="e91ec-106">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="e91ec-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="e91ec-107">Сообщения</span><span class="sxs-lookup"><span data-stu-id="e91ec-107">Messages</span></span>
- <span data-ttu-id="e91ec-108">События</span><span class="sxs-lookup"><span data-stu-id="e91ec-108">Events</span></span>
- <span data-ttu-id="e91ec-109">Контакты</span><span class="sxs-lookup"><span data-stu-id="e91ec-109">Contacts</span></span>
- <span data-ttu-id="e91ec-110">пользователи;</span><span class="sxs-lookup"><span data-stu-id="e91ec-110">Users</span></span>
- <span data-ttu-id="e91ec-111">Группы</span><span class="sxs-lookup"><span data-stu-id="e91ec-111">Groups</span></span>
- <span data-ttu-id="e91ec-112">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="e91ec-112">Group conversations</span></span>
- <span data-ttu-id="e91ec-113">Содержимое OneDrive с общим доступом, включая диски, связанные с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="e91ec-113">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="e91ec-114">Личные папки пользователей в OneDrive</span><span class="sxs-lookup"><span data-stu-id="e91ec-114">User's personal OneDrive folders</span></span>

## <a name="permissions"></a><span data-ttu-id="e91ec-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e91ec-115">Permissions</span></span>

<span data-ttu-id="e91ec-p102">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription_post_subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e91ec-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="e91ec-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e91ec-120">Permission type</span></span>                        | <span data-ttu-id="e91ec-121">Типы ресурсов, поддерживаемые в версии 1.0</span><span class="sxs-lookup"><span data-stu-id="e91ec-121">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="e91ec-122">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="e91ec-122">Delegated - work or school account</span></span>     | <span data-ttu-id="e91ec-123">[contact][], [conversation][], [drive][], [event][], [message][]</span><span class="sxs-lookup"><span data-stu-id="e91ec-123">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="e91ec-124">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="e91ec-124">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="e91ec-125">Нет</span><span class="sxs-lookup"><span data-stu-id="e91ec-125">None</span></span>                                                             |
| <span data-ttu-id="e91ec-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e91ec-126">Application</span></span>                            | <span data-ttu-id="e91ec-127">contact, conversation, event, message[ ][] [ ][] [ ][] [ ][]</span><span class="sxs-lookup"><span data-stu-id="e91ec-127">[contact][], [conversation][], [event][], [message][]</span></span>            |

## <a name="see-also"></a><span data-ttu-id="e91ec-128">См. также</span><span class="sxs-lookup"><span data-stu-id="e91ec-128">See also</span></span>

- [<span data-ttu-id="e91ec-129">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="e91ec-129">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="e91ec-130">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="e91ec-130">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="e91ec-131">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="e91ec-131">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="e91ec-132">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="e91ec-132">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="e91ec-133">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="e91ec-133">Delete subscription</span></span>](../api/subscription_delete.md)

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
