---
title: Настройка уведомлений об изменениях в пользовательских данных
description: API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.
ms.openlocfilehash: faaa1be8330118f1cbebf5362903f0e114816b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092724"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="5a020-105">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="5a020-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="5a020-p102">API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.</span><span class="sxs-lookup"><span data-stu-id="5a020-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="5a020-109">Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке.</span><span class="sxs-lookup"><span data-stu-id="5a020-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="5a020-110">Затем приложение действует в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="5a020-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="5a020-111">Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.</span><span class="sxs-lookup"><span data-stu-id="5a020-111">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="5a020-112">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="5a020-112">Supported resources</span></span>

<span data-ttu-id="5a020-113">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="5a020-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="5a020-114">Сообщения</span><span class="sxs-lookup"><span data-stu-id="5a020-114">Messages</span></span>
- <span data-ttu-id="5a020-115">События</span><span class="sxs-lookup"><span data-stu-id="5a020-115">Events</span></span>
- <span data-ttu-id="5a020-116">Контакты</span><span class="sxs-lookup"><span data-stu-id="5a020-116">Contacts</span></span>
- <span data-ttu-id="5a020-117">пользователи;</span><span class="sxs-lookup"><span data-stu-id="5a020-117">Users</span></span>
- <span data-ttu-id="5a020-118">Группы</span><span class="sxs-lookup"><span data-stu-id="5a020-118">Groups</span></span>
- <span data-ttu-id="5a020-119">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="5a020-119">Group conversations</span></span>
- <span data-ttu-id="5a020-120">Контент с общим доступом в OneDrive, включая диски, сопоставленные с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="5a020-120">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="5a020-121">Личные папки пользователя в OneDrive</span><span class="sxs-lookup"><span data-stu-id="5a020-121">User's personal OneDrive folders</span></span>
- <span data-ttu-id="5a020-122">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="5a020-122">Security Alerts</span></span>

<span data-ttu-id="5a020-123">Например, вы можете создать подписку на определенную папку: `me/mailFolders('inbox')/messages`;</span><span class="sxs-lookup"><span data-stu-id="5a020-123">For instance, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="5a020-124">либо на ресурс верхнего уровня: `me/messages`, `me/contacts`, `me/events`, `users` или `groups`;</span><span class="sxs-lookup"><span data-stu-id="5a020-124">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="5a020-125">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`;</span><span class="sxs-lookup"><span data-stu-id="5a020-125">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="5a020-126">либо на диск SharePoint/OneDrive для бизнеса: `/drive/root`;</span><span class="sxs-lookup"><span data-stu-id="5a020-126">Or to a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="5a020-127">либо на личный OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="5a020-127">Or to a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="5a020-128">либо на новое [оповещение API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`.</span><span class="sxs-lookup"><span data-stu-id="5a020-128">Or to a new [Security API alert](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="5a020-129">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="5a020-129">Azure AD resource limitations</span></span>

<span data-ttu-id="5a020-130">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения могут возникать ошибки.</span><span class="sxs-lookup"><span data-stu-id="5a020-130">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="5a020-131">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="5a020-131">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="5a020-132">На приложение: 50 000 подписок всего</span><span class="sxs-lookup"><span data-stu-id="5a020-132">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="5a020-133">На клиента: 35 подписок всего во всех приложениях</span><span class="sxs-lookup"><span data-stu-id="5a020-133">Per tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="5a020-134">На сочетание приложения и клиента: 7 подписок всего</span><span class="sxs-lookup"><span data-stu-id="5a020-134">Per app and tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="5a020-135">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="5a020-135">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="5a020-136">Уведомления для сущностей пользователей не поддерживаются для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5a020-136">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="5a020-137">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="5a020-137">Subscription lifetime</span></span>

<span data-ttu-id="5a020-138">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="5a020-138">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="5a020-139">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="5a020-139">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="5a020-140">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="5a020-140">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="5a020-141">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="5a020-141">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="5a020-142">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="5a020-142">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="5a020-143">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="5a020-143">Managing subscriptions</span></span>

<span data-ttu-id="5a020-144">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="5a020-144">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="5a020-145">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="5a020-145">Creating a subscription</span></span>

<span data-ttu-id="5a020-p105">Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="5a020-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="5a020-148">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="5a020-148">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="5a020-149">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="5a020-149">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="5a020-150">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5a020-150">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="5a020-151">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5a020-151">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="5a020-152">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5a020-152">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="5a020-153">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5a020-153">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="5a020-154">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления с подписками.</span><span class="sxs-lookup"><span data-stu-id="5a020-154">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="5a020-155">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="5a020-155">Subscription request example</span></span>

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

<span data-ttu-id="5a020-156">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="5a020-156">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="5a020-157">Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="5a020-157">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="5a020-158">Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5a020-158">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="5a020-159">Задание этого свойства позволит подтверждать, что полученные уведомления поступают от службы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5a020-159">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="5a020-160">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5a020-160">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="5a020-161">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5a020-161">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="5a020-162">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="5a020-162">Notification endpoint validation</span></span>

<span data-ttu-id="5a020-163">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="5a020-163">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="5a020-164">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="5a020-164">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="5a020-165">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="5a020-165">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="5a020-166">**Важно!** Так как `validationToken` — это параметр запроса, он должен декодироваться клиентом согласно правилам кодирования HTTP.</span><span class="sxs-lookup"><span data-stu-id="5a020-166">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="5a020-167">Если клиент не декодирует маркер и использует закодированное значение на следующем шаге (ответ), конечная точка не пройдет проверку.</span><span class="sxs-lookup"><span data-stu-id="5a020-167">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="5a020-168">Кроме того, клиент должен рассматривать значение маркера как непрозрачное, так как формат маркера может измениться в будущем без уведомления.</span><span class="sxs-lookup"><span data-stu-id="5a020-168">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="5a020-169">В течение 10 секунд клиент должен предоставить ответ со следующими характеристиками:</span><span class="sxs-lookup"><span data-stu-id="5a020-169">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="5a020-170">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="5a020-170">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="5a020-171">Необходимый тип контента — `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="5a020-171">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="5a020-172">Текст должен содержать маркер проверки, предоставленный Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5a020-172">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="5a020-173">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="5a020-173">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="5a020-174">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="5a020-174">Renewing a subscription</span></span>

<span data-ttu-id="5a020-175">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="5a020-175">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="5a020-176">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="5a020-176">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="5a020-177">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="5a020-177">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="5a020-178">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5a020-178">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="5a020-179">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="5a020-179">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="5a020-180">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="5a020-180">Deleting a subscription</span></span>

<span data-ttu-id="5a020-181">Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="5a020-181">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="5a020-182">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5a020-182">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="5a020-183">Уведомления</span><span class="sxs-lookup"><span data-stu-id="5a020-183">Notifications</span></span>

<span data-ttu-id="5a020-184">После создания подписки клиент начнет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="5a020-184">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="5a020-185">При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5a020-185">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="5a020-186">Уведомления отправляются только при изменениях типа, указанного в подписке, например, `created`.</span><span class="sxs-lookup"><span data-stu-id="5a020-186">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="5a020-187">**Примечание.** Если вы используете несколько подписок, которые отслеживают один тип ресурса и имеют один URL-адрес уведомлений, может быть отправлено сообщение POST, содержащее несколько уведомлений с разными идентификаторами подписок.</span><span class="sxs-lookup"><span data-stu-id="5a020-187">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="5a020-188">Уведомления из сообщения POST могут принадлежать разным подпискам.</span><span class="sxs-lookup"><span data-stu-id="5a020-188">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="5a020-189">Свойства уведомлений</span><span class="sxs-lookup"><span data-stu-id="5a020-189">Notification properties</span></span>

<span data-ttu-id="5a020-190">Объект уведомления содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="5a020-190">The notification object has the following properties:</span></span>

| <span data-ttu-id="5a020-191">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a020-191">Property</span></span> | <span data-ttu-id="5a020-192">Тип</span><span class="sxs-lookup"><span data-stu-id="5a020-192">Type</span></span> | <span data-ttu-id="5a020-193">Описание</span><span class="sxs-lookup"><span data-stu-id="5a020-193">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5a020-194">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="5a020-194">subscriptionId</span></span> | <span data-ttu-id="5a020-195">строка</span><span class="sxs-lookup"><span data-stu-id="5a020-195">string</span></span> | <span data-ttu-id="5a020-196">Идентификатор подписки, для которого было создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="5a020-196">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="5a020-197">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5a020-197">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="5a020-198">дата и время</span><span class="sxs-lookup"><span data-stu-id="5a020-198">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="5a020-199">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="5a020-199">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="5a020-200">clientState</span><span class="sxs-lookup"><span data-stu-id="5a020-200">clientState</span></span> | <span data-ttu-id="5a020-201">строка</span><span class="sxs-lookup"><span data-stu-id="5a020-201">string</span></span> | <span data-ttu-id="5a020-202">`clientState` — свойство, указанное в запросе на подписку (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="5a020-202">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="5a020-203">changeType</span><span class="sxs-lookup"><span data-stu-id="5a020-203">changeType</span></span> | <span data-ttu-id="5a020-204">строка</span><span class="sxs-lookup"><span data-stu-id="5a020-204">string</span></span> | <span data-ttu-id="5a020-205">Тип события, вызвавшего уведомление.</span><span class="sxs-lookup"><span data-stu-id="5a020-205">The event type that caused the notification.</span></span> <span data-ttu-id="5a020-206">Примеры: `created` при получении сообщения или `updated`, когда сообщение помечается как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="5a020-206">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="5a020-207">resource</span><span class="sxs-lookup"><span data-stu-id="5a020-207">resource</span></span> | <span data-ttu-id="5a020-208">строка</span><span class="sxs-lookup"><span data-stu-id="5a020-208">string</span></span> | <span data-ttu-id="5a020-209">Универсальный код ресурса (URI) ресурса относительно `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="5a020-209">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="5a020-210">resourceData</span><span class="sxs-lookup"><span data-stu-id="5a020-210">resourceData</span></span> | <span data-ttu-id="5a020-211">объект</span><span class="sxs-lookup"><span data-stu-id="5a020-211">object</span></span> | <span data-ttu-id="5a020-212">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="5a020-212">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="5a020-213">Например, для ресурсов Outlook `resourceData` содержит такие поля:</span><span class="sxs-lookup"><span data-stu-id="5a020-213">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="5a020-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a020-214">Property</span></span> | <span data-ttu-id="5a020-215">Тип</span><span class="sxs-lookup"><span data-stu-id="5a020-215">Type</span></span> | <span data-ttu-id="5a020-216">Описание</span><span class="sxs-lookup"><span data-stu-id="5a020-216">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5a020-217">@odata.type</span><span class="sxs-lookup"><span data-stu-id="5a020-217">@odata.type</span></span> | <span data-ttu-id="5a020-218">строка</span><span class="sxs-lookup"><span data-stu-id="5a020-218">string</span></span> | <span data-ttu-id="5a020-219">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="5a020-219">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="5a020-220">@odata.id</span><span class="sxs-lookup"><span data-stu-id="5a020-220">@odata.id</span></span> | <span data-ttu-id="5a020-221">строка</span><span class="sxs-lookup"><span data-stu-id="5a020-221">string</span></span> | <span data-ttu-id="5a020-222">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="5a020-222">The OData identifier of the object.</span></span> |
| <span data-ttu-id="5a020-223">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="5a020-223">@odata.etag</span></span> | <span data-ttu-id="5a020-224">строка</span><span class="sxs-lookup"><span data-stu-id="5a020-224">string</span></span> | <span data-ttu-id="5a020-225">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="5a020-225">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="5a020-226">id</span><span class="sxs-lookup"><span data-stu-id="5a020-226">id</span></span> | <span data-ttu-id="5a020-227">строка</span><span class="sxs-lookup"><span data-stu-id="5a020-227">string</span></span> | <span data-ttu-id="5a020-228">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="5a020-228">The identifier of the object.</span></span> |

> <span data-ttu-id="5a020-229">**Примечание.** Значение `id`, указанное в `resourceData`, действительно в момент создания уведомления.</span><span class="sxs-lookup"><span data-stu-id="5a020-229">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="5a020-230">Некоторые действия, такие как перемещение сообщения в другую папку, могут привести к недействительности `id` во время обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5a020-230">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="5a020-231">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="5a020-231">Notification example</span></span>

<span data-ttu-id="5a020-232">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления, аналогичные указанному ниже.</span><span class="sxs-lookup"><span data-stu-id="5a020-232">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="5a020-233">Обратите внимание, что поле `value` представляет собой массив объектов.</span><span class="sxs-lookup"><span data-stu-id="5a020-233">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="5a020-234">Если в очереди много уведомлений, Microsoft Graph может отправлять несколько элементов в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="5a020-234">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="5a020-235">В одном запросе уведомления могут содержаться уведомления от разных подписок.</span><span class="sxs-lookup"><span data-stu-id="5a020-235">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="5a020-236">Обработка уведомления</span><span class="sxs-lookup"><span data-stu-id="5a020-236">Processing the notification</span></span>

<span data-ttu-id="5a020-237">Необходимо обрабатывать все уведомления, полученные программой.</span><span class="sxs-lookup"><span data-stu-id="5a020-237">Each notification received by your app should be processed.</span></span> <span data-ttu-id="5a020-238">Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.</span><span class="sxs-lookup"><span data-stu-id="5a020-238">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="5a020-239">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="5a020-239">Validate the `clientState` property.</span></span> <span data-ttu-id="5a020-240">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="5a020-240">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="5a020-241">**Примечание.** Если это не так, уведомление не следует рассматривать как действительное.</span><span class="sxs-lookup"><span data-stu-id="5a020-241">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="5a020-242">Возможно уведомление создано не Microsoft Graph и отправлено незаконным субъектом.</span><span class="sxs-lookup"><span data-stu-id="5a020-242">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="5a020-243">Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="5a020-243">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="5a020-244">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="5a020-244">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="5a020-245">Отправляйте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5a020-245">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="5a020-246">Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="5a020-246">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="5a020-247">**Примечание.** Код состояния `202 - Accepted` следует отправлять, даже если свойство `clientState` не совпадает со значением, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="5a020-247">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="5a020-248">Такие действия не позволяют потенциальным незаконным субъектам обнаружить факт недоверия к их уведомлениям и воспользоваться этой информацией, чтобы угадать значение свойства `clientState`.</span><span class="sxs-lookup"><span data-stu-id="5a020-248">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="5a020-249">Повторяйте эти действия для других уведомлений в запросе.</span><span class="sxs-lookup"><span data-stu-id="5a020-249">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="5a020-250">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="5a020-250">Code samples</span></span>

<span data-ttu-id="5a020-251">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="5a020-251">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="5a020-252">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="5a020-252">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="5a020-253">Пример веб-перехватчиков Microsoft Graph для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="5a020-253">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="5a020-254">Пример веб-перехватчиков Microsoft Graph для WebJobs SDK</span><span class="sxs-lookup"><span data-stu-id="5a020-254">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="5a020-255">См. также</span><span class="sxs-lookup"><span data-stu-id="5a020-255">See also</span></span>

- [<span data-ttu-id="5a020-256">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="5a020-256">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="5a020-257">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="5a020-257">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="5a020-258">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="5a020-258">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
