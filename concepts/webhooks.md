# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="fac5e-101">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="fac5e-101">Set up notifications for changes in user data</span></span>

<span data-ttu-id="fac5e-p101">API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.</span><span class="sxs-lookup"><span data-stu-id="fac5e-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="fac5e-105">Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке.</span><span class="sxs-lookup"><span data-stu-id="fac5e-105">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span> <span data-ttu-id="fac5e-106">Затем приложение действует в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="fac5e-106">The app then takes action according to its business logic.</span></span> <span data-ttu-id="fac5e-107">Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.</span><span class="sxs-lookup"><span data-stu-id="fac5e-107">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="fac5e-108">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="fac5e-108">Supported resources</span></span>

<span data-ttu-id="fac5e-109">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="fac5e-109">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="fac5e-110">Сообщения</span><span class="sxs-lookup"><span data-stu-id="fac5e-110">Messages</span></span>
- <span data-ttu-id="fac5e-111">События</span><span class="sxs-lookup"><span data-stu-id="fac5e-111">Events</span></span>
- <span data-ttu-id="fac5e-112">Контакты</span><span class="sxs-lookup"><span data-stu-id="fac5e-112">Contacts</span></span>
- <span data-ttu-id="fac5e-113">пользователи;</span><span class="sxs-lookup"><span data-stu-id="fac5e-113">Users</span></span>
- <span data-ttu-id="fac5e-114">Группы</span><span class="sxs-lookup"><span data-stu-id="fac5e-114">Groups</span></span>
- <span data-ttu-id="fac5e-115">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="fac5e-115">Group conversations</span></span>
- <span data-ttu-id="fac5e-116">Контент с общим доступом в OneDrive, включая диски, сопоставленные с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="fac5e-116">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="fac5e-117">Личные папки пользователя в OneDrive</span><span class="sxs-lookup"><span data-stu-id="fac5e-117">User's personal OneDrive folders</span></span>

<span data-ttu-id="fac5e-118">Например, вы можете создать подписку на определенную папку: `me/mailFolders('inbox')/messages`;</span><span class="sxs-lookup"><span data-stu-id="fac5e-118">For instance, you can create a subscription to a specific folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="fac5e-119">либо на ресурс верхнего уровня: `me/messages`, `me/contacts`, `me/events`, `users` или `groups`;</span><span class="sxs-lookup"><span data-stu-id="fac5e-119">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="fac5e-120">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`;</span><span class="sxs-lookup"><span data-stu-id="fac5e-120">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="fac5e-121">в SharePoint или либо на диске OneDrive для бизнеса: `/drive/root`;</span><span class="sxs-lookup"><span data-stu-id="fac5e-121">Or to a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="fac5e-122">либо в личном OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-122">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="fac5e-123">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="fac5e-123">Azure AD Resource Limitations</span></span>

<span data-ttu-id="fac5e-124">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения могут возникать ошибки.</span><span class="sxs-lookup"><span data-stu-id="fac5e-124">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="fac5e-125">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="fac5e-125">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="fac5e-126">На приложение: 50 000 подписок всего</span><span class="sxs-lookup"><span data-stu-id="fac5e-126">Per App: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="fac5e-127">На клиента: 35 подписок всего во всех приложениях</span><span class="sxs-lookup"><span data-stu-id="fac5e-127">Per Tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="fac5e-128">На сочетание приложения и клиента: 7 подписок всего</span><span class="sxs-lookup"><span data-stu-id="fac5e-128">Per App and Tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="fac5e-129">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="fac5e-129">Azure AD B2C tenants are not supported</span></span>

- <span data-ttu-id="fac5e-130">Уведомления для сущностей пользователей не поддерживаются для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="fac5e-130">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="fac5e-131">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="fac5e-131">Subscription lifetime</span></span>

<span data-ttu-id="fac5e-132">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="fac5e-132">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="fac5e-133">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="fac5e-133">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="fac5e-134">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="fac5e-134">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="fac5e-135">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="fac5e-135">For a list of maximum expiration times, see [Maximum length of subscription per resource type](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="fac5e-136">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="fac5e-136">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="fac5e-137">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="fac5e-137">Managing subscriptions</span></span>

<span data-ttu-id="fac5e-138">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="fac5e-138">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="fac5e-139">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="fac5e-139">Creating a subscription</span></span>

<span data-ttu-id="fac5e-p104">Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="fac5e-p104">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="fac5e-142">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="fac5e-142">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="fac5e-143">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="fac5e-143">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="fac5e-144">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="fac5e-144">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="fac5e-145">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fac5e-145">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="fac5e-146">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fac5e-146">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="fac5e-147">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fac5e-147">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="fac5e-148">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления с подписками.</span><span class="sxs-lookup"><span data-stu-id="fac5e-148">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="fac5e-149">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="fac5e-149">Subscription request example</span></span>

```http
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

<span data-ttu-id="fac5e-150">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-150">The `changeType`, `notificationUrl`, `resource` and `expirationDateTime` properties are required while the rest are optional.</span></span> <span data-ttu-id="fac5e-151">Определения и значения свойств представлены в [описании типа ресурса подписки](../api-reference/v1.0/resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="fac5e-151">See [subscription resource type](../api-reference/v1.0/resources/subscription.md) for property definitions and values.</span></span>

<span data-ttu-id="fac5e-152">Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="fac5e-152">The , , , and  properties are required. See subscription resource type for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="fac5e-153">Задание этого свойства позволит подтверждать, что полученные уведомления поступают от службы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fac5e-153">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="fac5e-154">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fac5e-154">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="fac5e-155">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](../api-reference/v1.0/resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fac5e-155">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="fac5e-156">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="fac5e-156">Notification endpoint validation</span></span>

<span data-ttu-id="fac5e-157">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="fac5e-157">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="fac5e-158">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="fac5e-158">The filtering process in a dashboard occurs as follows:</span></span>

1. <span data-ttu-id="fac5e-159">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="fac5e-159">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ```

1. <span data-ttu-id="fac5e-160">В течение 10 секунд клиент должен предоставить отклик с указанными ниже характеристиками.</span><span class="sxs-lookup"><span data-stu-id="fac5e-160">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="fac5e-161">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="fac5e-161">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="fac5e-162">Необходимый тип контента — `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-162">The content type must be text/plain.</span></span>
    - <span data-ttu-id="fac5e-163">Текст должен содержать маркер проверки, предоставленный Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fac5e-163">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="fac5e-164">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="fac5e-164">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="fac5e-165">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="fac5e-165">Renewing a subscription</span></span>

<span data-ttu-id="fac5e-166">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="fac5e-166">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span> <span data-ttu-id="fac5e-167">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="fac5e-167">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="fac5e-168">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="fac5e-168">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="fac5e-169">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](../api-reference/v1.0/resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fac5e-169">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span> <span data-ttu-id="fac5e-170">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-170">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="fac5e-171">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="fac5e-171">Deleting a subscription</span></span>

<span data-ttu-id="fac5e-172">Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="fac5e-172">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="fac5e-173">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-173">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="fac5e-174">Уведомления</span><span class="sxs-lookup"><span data-stu-id="fac5e-174">Notifications</span></span>

<span data-ttu-id="fac5e-175">После создания подписки клиент начнет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="fac5e-175">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="fac5e-176">При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="fac5e-176">Microsoft Graph sends a POST request to the notification URL:</span></span> <span data-ttu-id="fac5e-177">Уведомления отправляются только при изменениях типа, указанного в подписке, например, `created`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-177">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="fac5e-178">**Примечание.** Если вы используете несколько подписок, которые отслеживают один тип ресурса и имеют один URL-адрес уведомлений, может быть отправлено сообщение POST, содержащее несколько уведомлений с разными идентификаторами подписок.</span><span class="sxs-lookup"><span data-stu-id="fac5e-178">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="fac5e-179">Уведомления из сообщения POST могут принадлежать разным подпискам.</span><span class="sxs-lookup"><span data-stu-id="fac5e-179">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="fac5e-180">Свойства уведомлений</span><span class="sxs-lookup"><span data-stu-id="fac5e-180">Notification properties</span></span>

<span data-ttu-id="fac5e-181">Объект уведомления содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="fac5e-181">The notification object has the following properties:</span></span>

| <span data-ttu-id="fac5e-182">Свойство</span><span class="sxs-lookup"><span data-stu-id="fac5e-182">Property</span></span> | <span data-ttu-id="fac5e-183">Тип</span><span class="sxs-lookup"><span data-stu-id="fac5e-183">Type</span></span> | <span data-ttu-id="fac5e-184">Описание</span><span class="sxs-lookup"><span data-stu-id="fac5e-184">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fac5e-185">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="fac5e-185">subscriptionId</span></span> | <span data-ttu-id="fac5e-186">строка</span><span class="sxs-lookup"><span data-stu-id="fac5e-186">string</span></span> | <span data-ttu-id="fac5e-187">Идентификатор подписки, для которого было создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="fac5e-187">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="fac5e-188">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fac5e-188">SubscriptionExpirationDateTime</span></span> | [<span data-ttu-id="fac5e-189">дата и время</span><span class="sxs-lookup"><span data-stu-id="fac5e-189">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="fac5e-190">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="fac5e-190">: The expiration time for the subscription.</span></span> |
| <span data-ttu-id="fac5e-191">clientState</span><span class="sxs-lookup"><span data-stu-id="fac5e-191">clientState</span></span> | <span data-ttu-id="fac5e-192">строка</span><span class="sxs-lookup"><span data-stu-id="fac5e-192">string</span></span> | <span data-ttu-id="fac5e-193">`clientState` — свойство, указанное в запросе на подписку (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="fac5e-193">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="fac5e-194">changeType</span><span class="sxs-lookup"><span data-stu-id="fac5e-194">changeType</span></span> | <span data-ttu-id="fac5e-195">строка</span><span class="sxs-lookup"><span data-stu-id="fac5e-195">string</span></span> | <span data-ttu-id="fac5e-196">Тип события, вызвавшего уведомление.</span><span class="sxs-lookup"><span data-stu-id="fac5e-196">The event type that caused the notification.</span></span> <span data-ttu-id="fac5e-197">Примеры: `created` при получении сообщения или `updated`, когда сообщение помечается как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="fac5e-197">changeType - The event type that caused the notification. For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="fac5e-198">resource</span><span class="sxs-lookup"><span data-stu-id="fac5e-198">resource</span></span> | <span data-ttu-id="fac5e-199">строка</span><span class="sxs-lookup"><span data-stu-id="fac5e-199">string</span></span> | <span data-ttu-id="fac5e-200">Универсальный код ресурса (URI) ресурса относительно `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-200">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="fac5e-201">resourceData</span><span class="sxs-lookup"><span data-stu-id="fac5e-201">ResourceData</span></span> | <span data-ttu-id="fac5e-202">объект</span><span class="sxs-lookup"><span data-stu-id="fac5e-202">object</span></span> | <span data-ttu-id="fac5e-203">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="fac5e-203">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="fac5e-204">Например, для ресурсов Outlook `resourceData` содержит такие поля:</span><span class="sxs-lookup"><span data-stu-id="fac5e-204">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="fac5e-205">Свойство</span><span class="sxs-lookup"><span data-stu-id="fac5e-205">Property</span></span> | <span data-ttu-id="fac5e-206">Тип</span><span class="sxs-lookup"><span data-stu-id="fac5e-206">Type</span></span> | <span data-ttu-id="fac5e-207">Описание</span><span class="sxs-lookup"><span data-stu-id="fac5e-207">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fac5e-208">@odata.type</span><span class="sxs-lookup"><span data-stu-id="fac5e-208">@odata.type</span></span> | <span data-ttu-id="fac5e-209">строка</span><span class="sxs-lookup"><span data-stu-id="fac5e-209">string</span></span> | <span data-ttu-id="fac5e-210">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="fac5e-210">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="fac5e-211">@odata.id</span><span class="sxs-lookup"><span data-stu-id="fac5e-211">@odata.id</span></span> | <span data-ttu-id="fac5e-212">строка</span><span class="sxs-lookup"><span data-stu-id="fac5e-212">string</span></span> | <span data-ttu-id="fac5e-213">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="fac5e-213">@odata.id - The OData identifier of the object.</span></span> |
| <span data-ttu-id="fac5e-214">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="fac5e-214">@odata.etag</span></span> | <span data-ttu-id="fac5e-215">строка</span><span class="sxs-lookup"><span data-stu-id="fac5e-215">string</span></span> | <span data-ttu-id="fac5e-216">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="fac5e-216">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span> |
| <span data-ttu-id="fac5e-217">id</span><span class="sxs-lookup"><span data-stu-id="fac5e-217">id</span></span> | <span data-ttu-id="fac5e-218">строка</span><span class="sxs-lookup"><span data-stu-id="fac5e-218">string</span></span> | <span data-ttu-id="fac5e-219">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="fac5e-219">Id - The identifier of the object.</span></span> |

> <span data-ttu-id="fac5e-220">**Примечание.** Значение `id`, указанное в `resourceData`, действительно в момент создания уведомления.</span><span class="sxs-lookup"><span data-stu-id="fac5e-220">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="fac5e-221">Некоторые действия, такие как перемещение сообщения в другую папку, могут привести к недействительности `id` во время обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="fac5e-221">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="fac5e-222">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="fac5e-222">Notification example</span></span>

<span data-ttu-id="fac5e-223">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления, аналогичные указанному ниже.</span><span class="sxs-lookup"><span data-stu-id="fac5e-223">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
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

<span data-ttu-id="fac5e-224">Обратите внимание, что поле `value` представляет собой массив объектов.</span><span class="sxs-lookup"><span data-stu-id="fac5e-224">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="fac5e-225">Если в очереди много уведомлений, Microsoft Graph может отправлять несколько элементов в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="fac5e-225">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="fac5e-226">В одном запросе уведомления могут содержаться уведомления от разных подписок.</span><span class="sxs-lookup"><span data-stu-id="fac5e-226">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="fac5e-227">Обработка уведомления</span><span class="sxs-lookup"><span data-stu-id="fac5e-227">Processing the notification</span></span>

<span data-ttu-id="fac5e-228">Необходимо обрабатывать все уведомления, полученные программой.</span><span class="sxs-lookup"><span data-stu-id="fac5e-228">Each notification received by your app should be processed.</span></span> <span data-ttu-id="fac5e-229">Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.</span><span class="sxs-lookup"><span data-stu-id="fac5e-229">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="fac5e-230">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-230">Validate the `clientState` property.</span></span> <span data-ttu-id="fac5e-231">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="fac5e-231">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="fac5e-232">**Примечание.** Если это не так, уведомление не следует рассматривать как действительное.</span><span class="sxs-lookup"><span data-stu-id="fac5e-232">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="fac5e-233">Возможно уведомление создано не Microsoft Graph и отправлено незаконным субъектом.</span><span class="sxs-lookup"><span data-stu-id="fac5e-233">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="fac5e-234">Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="fac5e-234">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="fac5e-235">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="fac5e-235">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="fac5e-236">Отправляйте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fac5e-236">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="fac5e-237">Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="fac5e-237">Send a  status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>

    > <span data-ttu-id="fac5e-238">**Примечание.** Код состояния `202 - Accepted` следует отправлять, даже если свойство `clientState` не совпадает со значением, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="fac5e-238">You should send a  status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="fac5e-239">Такие действия не позволяют потенциальным незаконным субъектам обнаружить факт недоверия к их уведомлениям и воспользоваться этой информацией, чтобы угадать значение свойства `clientState`.</span><span class="sxs-lookup"><span data-stu-id="fac5e-239">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="fac5e-240">Повторяйте эти действия для других уведомлений в запросе.</span><span class="sxs-lookup"><span data-stu-id="fac5e-240">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="fac5e-241">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="fac5e-241">Code samples</span></span>

<span data-ttu-id="fac5e-242">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="fac5e-242">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="fac5e-243">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="fac5e-243">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="fac5e-244">Пример веб-перехватчиков Microsoft Graph для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="fac5e-244">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="fac5e-245">Пример веб-перехватчиков Microsoft Graph для WebJobs SDK</span><span class="sxs-lookup"><span data-stu-id="fac5e-245">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="fac5e-246">См. также</span><span class="sxs-lookup"><span data-stu-id="fac5e-246">See also</span></span>

- [<span data-ttu-id="fac5e-247">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="fac5e-247">Subscription resource type</span></span>](../api-reference/v1.0/resources/subscription.md)
- [<span data-ttu-id="fac5e-248">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="fac5e-248">Get subscription</span></span>](../api-reference/v1.0/api/subscription_get.md)
- [<span data-ttu-id="fac5e-249">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="fac5e-249">Create subscription</span></span>](../api-reference/v1.0/api/subscription_post_subscriptions.md)

[contact]: ../api-reference/v1.0/resources/contact.md
[conversation]: ../api-reference/v1.0/resources/conversation.md
[drive]: ../api-reference/v1.0/resources/drive.md
[event]: ../api-reference/v1.0/resources/event.md
[message]: ../api-reference/v1.0/resources/message.md
