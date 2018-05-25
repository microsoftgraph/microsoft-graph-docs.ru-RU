# <a name="working-with-webhooks-in-microsoft-graph"></a><span data-ttu-id="45dba-101">Работа с веб-перехватчиками в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="45dba-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="45dba-p101">REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях.</span><span class="sxs-lookup"><span data-stu-id="45dba-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="45dba-105">С помощью REST API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="45dba-105">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

* <span data-ttu-id="45dba-106">Сообщения</span><span class="sxs-lookup"><span data-stu-id="45dba-106">Messages</span></span>
* <span data-ttu-id="45dba-107">События</span><span class="sxs-lookup"><span data-stu-id="45dba-107">Events</span></span>
* <span data-ttu-id="45dba-108">Контакты</span><span class="sxs-lookup"><span data-stu-id="45dba-108">Contacts</span></span>
* <span data-ttu-id="45dba-109">пользователи;</span><span class="sxs-lookup"><span data-stu-id="45dba-109">Users</span></span>
* <span data-ttu-id="45dba-110">Группы</span><span class="sxs-lookup"><span data-stu-id="45dba-110">Groups</span></span>
* <span data-ttu-id="45dba-111">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="45dba-111">Group conversations</span></span>
* <span data-ttu-id="45dba-112">Контент с общим доступом в OneDrive, включая диски, сопоставленные с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="45dba-112">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
* <span data-ttu-id="45dba-113">Личные папки пользователя в OneDrive</span><span class="sxs-lookup"><span data-stu-id="45dba-113">User's personal OneDrive folders</span></span>

<span data-ttu-id="45dba-114">Например, вы можете создать подписку на определенную папку: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="45dba-114">For instance, you can create a subscription to a specific folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="45dba-115">Или определенный идентификатор: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="45dba-115">Or a specific ID: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="45dba-116">Или на ресурс верхнего уровня: `me/messages`, `me/contacts`, `me/events`, `users` или `groups`</span><span class="sxs-lookup"><span data-stu-id="45dba-116">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`</span></span>

<span data-ttu-id="45dba-117">В Sharepoint либо на диске в OneDrive для бизнеса: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="45dba-117">Or on a Sharepoint / OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="45dba-118">Либо в личном OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="45dba-118">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="45dba-p102">Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке. Затем приложение действует в соответствии с бизнес-логикой. Например, оно получает дополнительные данные, обновляет кэш и представления и т. д.</span><span class="sxs-lookup"><span data-stu-id="45dba-p102">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span>

<span data-ttu-id="45dba-122">Приложениям необходимо обновлять свои подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="45dba-122">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="45dba-123">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="45dba-123">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="45dba-124">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="45dba-124">For a list of maximum expiration times, see [Maximum length of subscription per resource type](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="45dba-125">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="45dba-125">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

<span data-ttu-id="45dba-p104">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api-reference/v1.0/api/subscription_post_subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="45dba-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api-reference/v1.0/api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span> 

| <span data-ttu-id="45dba-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45dba-130">Permission type</span></span>                        | <span data-ttu-id="45dba-131">Типы ресурсов, поддерживаемые в версии 1.0</span><span class="sxs-lookup"><span data-stu-id="45dba-131">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="45dba-132">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="45dba-132">Delegated - work or school account</span></span>     | <span data-ttu-id="45dba-133">[contact][], [conversation][], [drive][], [event][], [message][]</span><span class="sxs-lookup"><span data-stu-id="45dba-133">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="45dba-134">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="45dba-134">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="45dba-135">Нет</span><span class="sxs-lookup"><span data-stu-id="45dba-135">None</span></span>                                                             |
| <span data-ttu-id="45dba-136">Application</span><span class="sxs-lookup"><span data-stu-id="45dba-136">Application</span></span>                            | <span data-ttu-id="45dba-137">[contact][], [conversation][], [event][], [message][]</span><span class="sxs-lookup"><span data-stu-id="45dba-137">[contact][], [conversation][], [event][], [message][]</span></span>            |


## <a name="code-samples"></a><span data-ttu-id="45dba-138">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="45dba-138">Code samples</span></span>

<span data-ttu-id="45dba-139">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="45dba-139">The following code samples are available on GitHub.</span></span>

* [<span data-ttu-id="45dba-140">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="45dba-140">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="45dba-141">Пример веб-перехватчиков Microsoft Graph для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="45dba-141">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

### <a name="creating-a-subscription"></a><span data-ttu-id="45dba-142">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="45dba-142">Creating a subscription</span></span>

<span data-ttu-id="45dba-p105">Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="45dba-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="45dba-145">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="45dba-145">The client sends a subscription (POST) request for a specific resource.</span></span>
2. <span data-ttu-id="45dba-146">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="45dba-146">Microsoft Graph verifies the request.</span></span>
  * <span data-ttu-id="45dba-147">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="45dba-147">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
  * <span data-ttu-id="45dba-148">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="45dba-148">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>
3. <span data-ttu-id="45dba-149">Клиент отправляет маркер проверки обратно в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="45dba-149">The client sends the validation token back to Microsoft Graph.</span></span>

<span data-ttu-id="45dba-150">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления с соответствующими подписками.</span><span class="sxs-lookup"><span data-stu-id="45dba-150">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

### <a name="notification-url-validation"></a><span data-ttu-id="45dba-151">Проверка URL-адреса уведомления</span><span class="sxs-lookup"><span data-stu-id="45dba-151">Notification URL validation</span></span>

<span data-ttu-id="45dba-p106">Прежде чем создавать подписку, Microsoft Graph проверяет URL-адрес уведомлений в запросе на подписку. Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="45dba-p106">Microsoft Graph validates the notification URL in a subscription request before creating the subscription. The validation process occurs as follows:</span></span>

1. <span data-ttu-id="45dba-154">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="45dba-154">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```

2. <span data-ttu-id="45dba-155">В течение 10 секунд клиент должен предоставить отклик с указанными ниже характеристиками.</span><span class="sxs-lookup"><span data-stu-id="45dba-155">The client must provide a response with the following characteristics within 10 seconds:</span></span>

  * <span data-ttu-id="45dba-156">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="45dba-156">A 200 (OK) status code.</span></span>
  * <span data-ttu-id="45dba-157">Необходимый тип контента — текст (в том числе обычный).</span><span class="sxs-lookup"><span data-stu-id="45dba-157">The content type must be text/plain.</span></span> 
  * <span data-ttu-id="45dba-158">Текст должен включать маркер проверки, который предоставил Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="45dba-158">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="45dba-159">Клиент должен удалить маркер проверки после того, как предоставит его в отклике.</span><span class="sxs-lookup"><span data-stu-id="45dba-159">The client should discard the validation token after providing it in the response.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="45dba-160">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="45dba-160">Subscription request example</span></span>

``` http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

<span data-ttu-id="45dba-p107">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`. Определения и значения свойств представлены в [описании типа ресурса subscription](../api-reference/v1.0/resources/subscription.md). Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="45dba-p107">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required. See [subscription resource type](../api-reference/v1.0/resources/subscription.md) for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span>

<span data-ttu-id="45dba-164">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [subscription](../api-reference/v1.0/resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="45dba-164">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="45dba-165">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="45dba-165">Azure AD Resource Limitations</span></span>

<span data-ttu-id="45dba-166">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения могут возникать ошибки.</span><span class="sxs-lookup"><span data-stu-id="45dba-166">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

* <span data-ttu-id="45dba-167">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="45dba-167">Maximum subscription quotas:</span></span>

  * <span data-ttu-id="45dba-168">На приложение: 50 000 подписок всего</span><span class="sxs-lookup"><span data-stu-id="45dba-168">Per App: 50,000 total subscriptions</span></span>
  * <span data-ttu-id="45dba-169">На клиента: 35 подписок всего во всех приложениях</span><span class="sxs-lookup"><span data-stu-id="45dba-169">Per Tenant: 35 total subscriptions across all apps</span></span>
  * <span data-ttu-id="45dba-170">На сочетание приложения и клиента: 7 подписок всего</span><span class="sxs-lookup"><span data-stu-id="45dba-170">Per App and Tenant combination: 7 total subscriptions</span></span>

* <span data-ttu-id="45dba-171">Клиенты Azure AD B2C не поддерживаются</span><span class="sxs-lookup"><span data-stu-id="45dba-171">Azure AD B2C tenants are not supported</span></span>

* <span data-ttu-id="45dba-172">Пользователи потребительской версии не поддерживаются</span><span class="sxs-lookup"><span data-stu-id="45dba-172">Consumer account Users not supported</span></span>

## <a name="renewing-a-subscription"></a><span data-ttu-id="45dba-173">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="45dba-173">Renewing a subscription</span></span>

<span data-ttu-id="45dba-p108">Клиент может возобновить подписку, указав срок действия до трех дней с момента отправки запроса. Свойство expirationDateTime является обязательным.</span><span class="sxs-lookup"><span data-stu-id="45dba-p108">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span>

### <a name="subscription-renewal-example"></a><span data-ttu-id="45dba-176">Пример продления подписки</span><span class="sxs-lookup"><span data-stu-id="45dba-176">Subscription renewal example</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="45dba-p109">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [subscription](../api-reference/v1.0/resources/subscription.md) в теле отклика. Объект подписки включает новое значение expirationDateTime.</span><span class="sxs-lookup"><span data-stu-id="45dba-p109">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body. The subscription object includes the new expirationDateTime value.</span></span> 

## <a name="deleting-a-subscription"></a><span data-ttu-id="45dba-179">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="45dba-179">Deleting a subscription</span></span>

<span data-ttu-id="45dba-180">Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="45dba-180">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="45dba-181">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45dba-181">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="45dba-182">Уведомления</span><span class="sxs-lookup"><span data-stu-id="45dba-182">Notifications</span></span>

<span data-ttu-id="45dba-p110">После создания подписки клиент начнет получать уведомления. При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений. Клиент получает уведомления только об изменениях определенных типов, например *created*.</span><span class="sxs-lookup"><span data-stu-id="45dba-p110">The client starts receiving notifications after creating the subscription. Microsoft Graph sends a POST request to the notification URL when changes happen to the resource. The client only gets notifications according to the specified change type, such as *created*.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="45dba-186">Свойства уведомлений</span><span class="sxs-lookup"><span data-stu-id="45dba-186">Notification properties</span></span>

<span data-ttu-id="45dba-187">Объект уведомления содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="45dba-187">The notification object has the following properties:</span></span>

* <span data-ttu-id="45dba-188">subscriptionId — идентификатор подписки, к которой относится уведомление.</span><span class="sxs-lookup"><span data-stu-id="45dba-188">subscriptionId - The ID for the subscription to which this notification belongs.</span></span>
* <span data-ttu-id="45dba-189">subscriptionExpirationDateTime — время окончания срока действия для подписки.</span><span class="sxs-lookup"><span data-stu-id="45dba-189">subscriptionExpirationDateTime - The expiration time for the subscription.</span></span>
* <span data-ttu-id="45dba-190">clientState — свойство clientState, указанное в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="45dba-190">clientState - The clientState property specified in the subscription request.</span></span>
* <span data-ttu-id="45dba-p111">changeType — тип события, вызвавшего уведомление. Примеры: *created* при получении сообщения или *updated*, когда сообщение помечается как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="45dba-p111">changeType - The event type that caused the notification. For example, *created* on mail receive, or *updated* on marking a message read.</span></span>
* <span data-ttu-id="45dba-193">resource — URI ресурса относительно `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="45dba-193">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> 
* <span data-ttu-id="45dba-p112">resourceData — объект, зависящий от ресурса, подписка на который создается.  Например, для ресурсов Outlook:</span><span class="sxs-lookup"><span data-stu-id="45dba-p112">resourceData - The object dependent on the resource being subscribed to.  For example, for Outlook resources:</span></span>
  * <span data-ttu-id="45dba-196">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="45dba-196">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span>
  * <span data-ttu-id="45dba-197">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="45dba-197">@odata.id - The OData identifier of the object.</span></span>
  * <span data-ttu-id="45dba-198">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="45dba-198">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span>
  * <span data-ttu-id="45dba-199">id — идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="45dba-199">id - The identifier of the object.</span></span>

> <span data-ttu-id="45dba-p113">Примечание. Значение Id, указанное в resourceData, действительно в момент добавления уведомления в очередь. Некоторые действия, например перемещение сообщения в другую папку, могут привести к изменению идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="45dba-p113">Note: The Id value provided in resourceData is valid at the time the notification was queued. Some actions, such as moving a message to another folder, may result in a resource's Id being changed.</span></span> 

### <a name="notification-example"></a><span data-ttu-id="45dba-202">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="45dba-202">Notification example</span></span>

<span data-ttu-id="45dba-203">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления, аналогичные указанному ниже.</span><span class="sxs-lookup"><span data-stu-id="45dba-203">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

``` json
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
    "resourceData":
    {
      "@odata.type":"#Microsoft.Graph.Message",
      "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
      "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
      "id":"<long_id_string>"
    }
  }
  ]
}
```

<span data-ttu-id="45dba-p114">Обратите внимание, что объект value содержит список. Если в очереди много уведомлений, Microsoft Graph отправляет их в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="45dba-p114">Note the value object contains a list. If there are many queued notifications, Microsoft Graph sends them in a single request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="45dba-206">Обработка уведомления</span><span class="sxs-lookup"><span data-stu-id="45dba-206">Processing the notification</span></span>

<span data-ttu-id="45dba-p115">Когда приложение начинает получать уведомления, оно должно обрабатывать их. Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.</span><span class="sxs-lookup"><span data-stu-id="45dba-p115">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="45dba-p116">Проверьте свойство `clientState`. Свойство clientState уведомления должно совпадать со значением, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="45dba-p116">Validate the `clientState` property. The clientState property in the notification must match the one submitted with the subscription request.</span></span>
  > <span data-ttu-id="45dba-p117">Примечание. Если это не так, уведомление не следует рассматривать как действительное. Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="45dba-p117">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

2. <span data-ttu-id="45dba-213">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="45dba-213">Update your application based on your business logic.</span></span>

3. <span data-ttu-id="45dba-p118">Отправляйте код состояния `202 - Accepted` в ответе, отправляемом в Microsoft Graph. Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="45dba-p118">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
  > <span data-ttu-id="45dba-216">Код состояния `202 - Accepted` следует отправлять, даже если свойство clientState не совпадает со значением, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="45dba-216">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="45dba-217">Повторяйте эти действия для других уведомлений в запросе.</span><span class="sxs-lookup"><span data-stu-id="45dba-217">Repeat for other notifications in the request.</span></span>

## <a name="see-also"></a><span data-ttu-id="45dba-218">См. также</span><span class="sxs-lookup"><span data-stu-id="45dba-218">See also</span></span>

* [<span data-ttu-id="45dba-219">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="45dba-219">Subscription resource type</span></span>](../api-reference/v1.0/resources/subscription.md)
* [<span data-ttu-id="45dba-220">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="45dba-220">Get subscription</span></span>](../api-reference/v1.0/api/subscription_get.md)
* [<span data-ttu-id="45dba-221">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="45dba-221">Create subscription</span></span>](../api-reference/v1.0/api/subscription_post_subscriptions.md)
* [<span data-ttu-id="45dba-222">Пример Microsoft Graph Webhooks для Node.js</span><span class="sxs-lookup"><span data-stu-id="45dba-222">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="45dba-223">Пример Microsoft Graph Webhooks для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="45dba-223">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

[контакт]: ../api-reference/v1.0/resources/contact.md
[contact]: ../api-reference/v1.0/resources/contact.md
[беседа]: ../api-reference/v1.0/resources/conversation.md
[conversation]: ../api-reference/v1.0/resources/conversation.md
[диск]: ../api-reference/v1.0/resources/drive.md
[drive]: ../api-reference/v1.0/resources/drive.md
[событие]: ../api-reference/v1.0/resources/event.md
[event]: ../api-reference/v1.0/resources/event.md
[сообщение]: ../api-reference/v1.0/resources/message.md
[message]: ../api-reference/v1.0/resources/message.md
