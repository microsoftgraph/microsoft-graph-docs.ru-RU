---
title: Настройка уведомлений об изменениях в пользовательских данных
description: API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.
author: piotrci
ms.openlocfilehash: 6af6f3c54a7956d6a505c88bfc82fc8233dccdad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337046"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="be35d-105">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="be35d-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="be35d-p102">API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.</span><span class="sxs-lookup"><span data-stu-id="be35d-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="be35d-109">Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке.</span><span class="sxs-lookup"><span data-stu-id="be35d-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="be35d-110">Затем приложение действует в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="be35d-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="be35d-111">Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.</span><span class="sxs-lookup"><span data-stu-id="be35d-111">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="be35d-112">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="be35d-112">Supported resources</span></span>

<span data-ttu-id="be35d-113">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="be35d-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="be35d-114">Сообщения</span><span class="sxs-lookup"><span data-stu-id="be35d-114">Messages</span></span>
- <span data-ttu-id="be35d-115">События</span><span class="sxs-lookup"><span data-stu-id="be35d-115">Events</span></span>
- <span data-ttu-id="be35d-116">Контакты</span><span class="sxs-lookup"><span data-stu-id="be35d-116">Contacts</span></span>
- <span data-ttu-id="be35d-117">пользователи;</span><span class="sxs-lookup"><span data-stu-id="be35d-117">Users</span></span>
- <span data-ttu-id="be35d-118">Группы</span><span class="sxs-lookup"><span data-stu-id="be35d-118">Groups</span></span>
- <span data-ttu-id="be35d-119">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="be35d-119">Group conversations</span></span>
- <span data-ttu-id="be35d-120">Контент с общим доступом в OneDrive, включая диски, сопоставленные с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="be35d-120">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="be35d-121">Личные папки пользователя в OneDrive</span><span class="sxs-lookup"><span data-stu-id="be35d-121">User's personal OneDrive folders</span></span>
- <span data-ttu-id="be35d-122">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="be35d-122">Security Alerts</span></span>

<span data-ttu-id="be35d-123">Например, вы можете создать подписку на определенную папку: `me/mailFolders('inbox')/messages`;</span><span class="sxs-lookup"><span data-stu-id="be35d-123">For instance, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="be35d-124">либо на ресурс верхнего уровня: `me/messages`, `me/contacts`, `me/events`, `users` или `groups`;</span><span class="sxs-lookup"><span data-stu-id="be35d-124">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="be35d-125">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`;</span><span class="sxs-lookup"><span data-stu-id="be35d-125">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="be35d-126">либо на диск SharePoint/OneDrive для бизнеса: `/drive/root`;</span><span class="sxs-lookup"><span data-stu-id="be35d-126">Or to a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="be35d-127">либо на личный OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="be35d-127">Or to a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="be35d-128">либо на новое [оповещение API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`.</span><span class="sxs-lookup"><span data-stu-id="be35d-128">Or to a new [Security API alert](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="be35d-129">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="be35d-129">Azure AD resource limitations</span></span>

<span data-ttu-id="be35d-130">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения могут возникать ошибки.</span><span class="sxs-lookup"><span data-stu-id="be35d-130">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="be35d-131">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="be35d-131">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="be35d-132">На приложение: 50 000 подписок всего</span><span class="sxs-lookup"><span data-stu-id="be35d-132">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="be35d-133">На клиента: 35 подписок всего во всех приложениях</span><span class="sxs-lookup"><span data-stu-id="be35d-133">Per tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="be35d-134">На сочетание приложения и клиента: 7 подписок всего</span><span class="sxs-lookup"><span data-stu-id="be35d-134">Per app and tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="be35d-135">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="be35d-135">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="be35d-136">Уведомления для сущностей пользователей не поддерживаются для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="be35d-136">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="be35d-137">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="be35d-137">Subscription lifetime</span></span>

<span data-ttu-id="be35d-138">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="be35d-138">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="be35d-139">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="be35d-139">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="be35d-140">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="be35d-140">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="be35d-141">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="be35d-141">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="be35d-142">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="be35d-142">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="be35d-143">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="be35d-143">Managing subscriptions</span></span>

<span data-ttu-id="be35d-144">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="be35d-144">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="be35d-145">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="be35d-145">Creating a subscription</span></span>

<span data-ttu-id="be35d-p105">Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="be35d-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="be35d-148">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="be35d-148">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="be35d-149">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="be35d-149">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="be35d-150">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="be35d-150">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="be35d-151">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="be35d-151">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="be35d-152">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="be35d-152">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="be35d-153">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="be35d-153">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="be35d-154">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления с подписками.</span><span class="sxs-lookup"><span data-stu-id="be35d-154">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="be35d-155">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="be35d-155">Subscription request example</span></span>

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

<span data-ttu-id="be35d-156">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="be35d-156">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="be35d-157">Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="be35d-157">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="be35d-158">Свойство `resource` указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="be35d-158">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="be35d-159">Например, вы можете создать подписку на определенную почтовую папку: `me/mailFolders('inbox')/messages` или сделать это от имени пользователя с согласия администратора: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="be35d-159">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="be35d-160">Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="be35d-160">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="be35d-161">Задание этого свойства позволит подтверждать, что полученные уведомления поступают от службы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="be35d-161">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="be35d-162">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="be35d-162">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="be35d-163">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be35d-163">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="be35d-164">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="be35d-164">Notification endpoint validation</span></span>

<span data-ttu-id="be35d-165">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="be35d-165">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="be35d-166">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="be35d-166">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="be35d-167">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="be35d-167">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="be35d-168">**Важно!** Так как `validationToken` — это параметр запроса, он должен декодироваться клиентом согласно правилам кодирования HTTP.</span><span class="sxs-lookup"><span data-stu-id="be35d-168">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="be35d-169">Если клиент не декодирует маркер и использует закодированное значение на следующем шаге (ответ), конечная точка не пройдет проверку.</span><span class="sxs-lookup"><span data-stu-id="be35d-169">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="be35d-170">Кроме того, клиент должен рассматривать значение маркера как непрозрачное, так как формат маркера может измениться в будущем без уведомления.</span><span class="sxs-lookup"><span data-stu-id="be35d-170">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="be35d-171">В течение 10 секунд клиент должен предоставить ответ со следующими характеристиками:</span><span class="sxs-lookup"><span data-stu-id="be35d-171">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="be35d-172">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="be35d-172">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="be35d-173">Необходимый тип контента — `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="be35d-173">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="be35d-174">Текст должен содержать маркер проверки, предоставленный Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="be35d-174">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="be35d-175">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="be35d-175">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="be35d-176">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="be35d-176">Renewing a subscription</span></span>

<span data-ttu-id="be35d-177">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="be35d-177">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="be35d-178">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="be35d-178">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="be35d-179">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="be35d-179">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="be35d-180">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be35d-180">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="be35d-181">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="be35d-181">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="be35d-182">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="be35d-182">Deleting a subscription</span></span>

<span data-ttu-id="be35d-183">Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="be35d-183">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="be35d-184">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="be35d-184">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="be35d-185">Уведомления</span><span class="sxs-lookup"><span data-stu-id="be35d-185">Notifications</span></span>

<span data-ttu-id="be35d-186">После создания подписки клиент начнет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="be35d-186">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="be35d-187">При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="be35d-187">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="be35d-188">Уведомления отправляются только при изменениях типа, указанного в подписке, например, `created`.</span><span class="sxs-lookup"><span data-stu-id="be35d-188">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="be35d-189">**Примечание.** Если вы используете несколько подписок, которые отслеживают один тип ресурса и имеют один URL-адрес уведомлений, может быть отправлено сообщение POST, содержащее несколько уведомлений с разными идентификаторами подписок.</span><span class="sxs-lookup"><span data-stu-id="be35d-189">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="be35d-190">Уведомления из сообщения POST могут принадлежать разным подпискам.</span><span class="sxs-lookup"><span data-stu-id="be35d-190">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="be35d-191">Свойства уведомлений</span><span class="sxs-lookup"><span data-stu-id="be35d-191">Notification properties</span></span>

<span data-ttu-id="be35d-192">Объект уведомления содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="be35d-192">The notification object has the following properties:</span></span>

| <span data-ttu-id="be35d-193">Свойство</span><span class="sxs-lookup"><span data-stu-id="be35d-193">Property</span></span> | <span data-ttu-id="be35d-194">Тип</span><span class="sxs-lookup"><span data-stu-id="be35d-194">Type</span></span> | <span data-ttu-id="be35d-195">Описание</span><span class="sxs-lookup"><span data-stu-id="be35d-195">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="be35d-196">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="be35d-196">subscriptionId</span></span> | <span data-ttu-id="be35d-197">строка</span><span class="sxs-lookup"><span data-stu-id="be35d-197">string</span></span> | <span data-ttu-id="be35d-198">Идентификатор подписки, для которого было создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="be35d-198">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="be35d-199">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="be35d-199">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="be35d-200">дата и время</span><span class="sxs-lookup"><span data-stu-id="be35d-200">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="be35d-201">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="be35d-201">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="be35d-202">clientState</span><span class="sxs-lookup"><span data-stu-id="be35d-202">clientState</span></span> | <span data-ttu-id="be35d-203">строка</span><span class="sxs-lookup"><span data-stu-id="be35d-203">string</span></span> | <span data-ttu-id="be35d-204">`clientState` — свойство, указанное в запросе на подписку (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="be35d-204">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="be35d-205">changeType</span><span class="sxs-lookup"><span data-stu-id="be35d-205">changeType</span></span> | <span data-ttu-id="be35d-206">строка</span><span class="sxs-lookup"><span data-stu-id="be35d-206">string</span></span> | <span data-ttu-id="be35d-207">Тип события, вызвавшего уведомление.</span><span class="sxs-lookup"><span data-stu-id="be35d-207">The event type that caused the notification.</span></span> <span data-ttu-id="be35d-208">Примеры: `created` при получении сообщения или `updated`, когда сообщение помечается как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="be35d-208">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="be35d-209">resource</span><span class="sxs-lookup"><span data-stu-id="be35d-209">resource</span></span> | <span data-ttu-id="be35d-210">строка</span><span class="sxs-lookup"><span data-stu-id="be35d-210">string</span></span> | <span data-ttu-id="be35d-211">Универсальный код ресурса (URI) ресурса относительно `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="be35d-211">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="be35d-212">resourceData</span><span class="sxs-lookup"><span data-stu-id="be35d-212">resourceData</span></span> | <span data-ttu-id="be35d-213">объект</span><span class="sxs-lookup"><span data-stu-id="be35d-213">object</span></span> | <span data-ttu-id="be35d-214">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="be35d-214">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="be35d-215">Например, для ресурсов Outlook `resourceData` содержит такие поля:</span><span class="sxs-lookup"><span data-stu-id="be35d-215">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="be35d-216">Свойство</span><span class="sxs-lookup"><span data-stu-id="be35d-216">Property</span></span> | <span data-ttu-id="be35d-217">Тип</span><span class="sxs-lookup"><span data-stu-id="be35d-217">Type</span></span> | <span data-ttu-id="be35d-218">Описание</span><span class="sxs-lookup"><span data-stu-id="be35d-218">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="be35d-219">@odata.type</span><span class="sxs-lookup"><span data-stu-id="be35d-219">@odata.type</span></span> | <span data-ttu-id="be35d-220">строка</span><span class="sxs-lookup"><span data-stu-id="be35d-220">string</span></span> | <span data-ttu-id="be35d-221">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="be35d-221">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="be35d-222">@odata.id</span><span class="sxs-lookup"><span data-stu-id="be35d-222">@odata.id</span></span> | <span data-ttu-id="be35d-223">строка</span><span class="sxs-lookup"><span data-stu-id="be35d-223">string</span></span> | <span data-ttu-id="be35d-224">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="be35d-224">The OData identifier of the object.</span></span> |
| <span data-ttu-id="be35d-225">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="be35d-225">@odata.etag</span></span> | <span data-ttu-id="be35d-226">строка</span><span class="sxs-lookup"><span data-stu-id="be35d-226">string</span></span> | <span data-ttu-id="be35d-227">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="be35d-227">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="be35d-228">id</span><span class="sxs-lookup"><span data-stu-id="be35d-228">id</span></span> | <span data-ttu-id="be35d-229">строка</span><span class="sxs-lookup"><span data-stu-id="be35d-229">string</span></span> | <span data-ttu-id="be35d-230">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="be35d-230">The identifier of the object.</span></span> |

> <span data-ttu-id="be35d-231">**Примечание.** Значение `id`, указанное в `resourceData`, действительно в момент создания уведомления.</span><span class="sxs-lookup"><span data-stu-id="be35d-231">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="be35d-232">Некоторые действия, такие как перемещение сообщения в другую папку, могут привести к недействительности `id` во время обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="be35d-232">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="be35d-233">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="be35d-233">Notification example</span></span>

<span data-ttu-id="be35d-234">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления, аналогичные указанному ниже.</span><span class="sxs-lookup"><span data-stu-id="be35d-234">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="be35d-235">Обратите внимание, что поле `value` представляет собой массив объектов.</span><span class="sxs-lookup"><span data-stu-id="be35d-235">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="be35d-236">Если в очереди много уведомлений, Microsoft Graph может отправлять несколько элементов в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="be35d-236">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="be35d-237">В одном запросе уведомления могут содержаться уведомления от разных подписок.</span><span class="sxs-lookup"><span data-stu-id="be35d-237">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="be35d-238">Обработка уведомления</span><span class="sxs-lookup"><span data-stu-id="be35d-238">Processing the notification</span></span>

<span data-ttu-id="be35d-239">Необходимо обрабатывать все уведомления, полученные программой.</span><span class="sxs-lookup"><span data-stu-id="be35d-239">Each notification received by your app should be processed.</span></span> <span data-ttu-id="be35d-240">Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.</span><span class="sxs-lookup"><span data-stu-id="be35d-240">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="be35d-241">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="be35d-241">Validate the `clientState` property.</span></span> <span data-ttu-id="be35d-242">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="be35d-242">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="be35d-243">**Примечание.** Если это не так, уведомление не следует рассматривать как действительное.</span><span class="sxs-lookup"><span data-stu-id="be35d-243">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="be35d-244">Возможно уведомление создано не Microsoft Graph и отправлено незаконным субъектом.</span><span class="sxs-lookup"><span data-stu-id="be35d-244">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="be35d-245">Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="be35d-245">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="be35d-246">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="be35d-246">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="be35d-247">Отправляйте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="be35d-247">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="be35d-248">Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="be35d-248">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="be35d-249">**Примечание.** Код состояния `202 - Accepted` следует отправлять, даже если свойство `clientState` не совпадает со значением, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="be35d-249">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="be35d-250">Такие действия не позволяют потенциальным незаконным субъектам обнаружить факт недоверия к их уведомлениям и воспользоваться этой информацией, чтобы угадать значение свойства `clientState`.</span><span class="sxs-lookup"><span data-stu-id="be35d-250">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="be35d-251">Повторяйте эти действия для других уведомлений в запросе.</span><span class="sxs-lookup"><span data-stu-id="be35d-251">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="be35d-252">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="be35d-252">Code samples</span></span>

<span data-ttu-id="be35d-253">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="be35d-253">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="be35d-254">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="be35d-254">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="be35d-255">Пример веб-перехватчиков Microsoft Graph для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="be35d-255">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="be35d-256">Пример веб-перехватчиков Microsoft Graph для WebJobs SDK</span><span class="sxs-lookup"><span data-stu-id="be35d-256">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="be35d-257">См. также</span><span class="sxs-lookup"><span data-stu-id="be35d-257">See also</span></span>

- [<span data-ttu-id="be35d-258">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="be35d-258">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="be35d-259">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="be35d-259">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="be35d-260">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="be35d-260">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
