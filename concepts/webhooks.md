---
title: Настройка уведомлений об изменениях в пользовательских данных
description: API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 3bffab081e8f9520890f6bfe7c690b9258cd3dee
ms.sourcegitcommit: 7bf9885c8769c5dfe2614a98ba6d7cc297ae564c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2019
ms.locfileid: "34182092"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="24557-105">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="24557-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="24557-p102">API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.</span><span class="sxs-lookup"><span data-stu-id="24557-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="24557-109">Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке.</span><span class="sxs-lookup"><span data-stu-id="24557-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="24557-110">Затем приложение действует в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="24557-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="24557-111">Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.</span><span class="sxs-lookup"><span data-stu-id="24557-111">For example, it fetches more data, updates its cache and views, etc.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="24557-112">Создание приложения веб-перехватчика с помощью .NET Core</span><span class="sxs-lookup"><span data-stu-id="24557-112">Build a webhook app with .NET Core</span></span>](/graph/tutorials/change-notifications)

## <a name="supported-resources"></a><span data-ttu-id="24557-113">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="24557-113">Supported resources</span></span>

<span data-ttu-id="24557-114">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="24557-114">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="24557-115">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="24557-115">Outlook [message][]</span></span>
- <span data-ttu-id="24557-116">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="24557-116">Outlook [event][]</span></span>
- <span data-ttu-id="24557-117">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="24557-117">Outlook personal [contact][]</span></span>
- <span data-ttu-id="24557-118">[user][]</span><span class="sxs-lookup"><span data-stu-id="24557-118">[user][]</span></span>
- <span data-ttu-id="24557-119">[group][]</span><span class="sxs-lookup"><span data-stu-id="24557-119">[group][]</span></span>
- <span data-ttu-id="24557-120">Групповой [чат][] Office 365 </span><span class="sxs-lookup"><span data-stu-id="24557-120">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="24557-121">Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="24557-121">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="24557-122">Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="24557-122">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="24557-123">[Оповещение][] безопасности</span><span class="sxs-lookup"><span data-stu-id="24557-123">Security [alert][]</span></span>

<span data-ttu-id="24557-124">Например, вы можете создать подписку на определенную папку Outlook, например, папку Входящие: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="24557-124">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="24557-125">либо на ресурс верхнего уровня: `me/messages`, `me/contacts`, `me/events`, `users` или `groups`;</span><span class="sxs-lookup"><span data-stu-id="24557-125">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="24557-126">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`;</span><span class="sxs-lookup"><span data-stu-id="24557-126">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="24557-127">либо на личное хранилище OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="24557-127">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="24557-128">либо на корневую папку диска SharePoint/OneDrive для бизнеса: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="24557-128">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="24557-129">либо на новое оповещение [API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="24557-129">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="24557-130">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="24557-130">Azure AD resource limitations</span></span>

<span data-ttu-id="24557-131">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения возникают ошибки.</span><span class="sxs-lookup"><span data-stu-id="24557-131">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="24557-132">**Примечание**. Эти ограничения не применяются к ресурсам служб, не относящихся к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24557-132">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="24557-133">Например, приложение может создать больше дополнительных подписок на ресурсы `message` или `event`, поддерживаемые службой Exchange Online в составе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24557-133">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="24557-134">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="24557-134">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="24557-135">На приложение: 50 000 подписок всего</span><span class="sxs-lookup"><span data-stu-id="24557-135">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="24557-136">На клиента: 1000 подписок всего во всех приложениях</span><span class="sxs-lookup"><span data-stu-id="24557-136">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="24557-137">На сочетание приложения и клиента: 100 подписок всего</span><span class="sxs-lookup"><span data-stu-id="24557-137">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="24557-138">Если ограничения превышены, попытки создать подписку приведут к [ответу с ошибкой](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="24557-138">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="24557-139">Свойство `message` указывает, какое ограничение превышено.</span><span class="sxs-lookup"><span data-stu-id="24557-139">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="24557-140">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="24557-140">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="24557-141">Уведомления для сущностей пользователей не поддерживаются для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="24557-141">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="24557-142">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="24557-142">Subscription lifetime</span></span>

<span data-ttu-id="24557-143">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="24557-143">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="24557-144">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="24557-144">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="24557-145">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="24557-145">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="24557-146">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="24557-146">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="24557-147">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="24557-147">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="24557-148">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="24557-148">Managing subscriptions</span></span>

<span data-ttu-id="24557-149">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="24557-149">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="24557-150">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="24557-150">Creating a subscription</span></span>

<span data-ttu-id="24557-p107">Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="24557-p107">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="24557-153">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="24557-153">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="24557-154">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="24557-154">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="24557-155">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="24557-155">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="24557-156">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="24557-156">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="24557-157">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24557-157">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="24557-158">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24557-158">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="24557-159">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления с подписками.</span><span class="sxs-lookup"><span data-stu-id="24557-159">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="24557-160">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="24557-160">Subscription request example</span></span>

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

<span data-ttu-id="24557-161">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="24557-161">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="24557-162">Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="24557-162">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="24557-163">Свойство `resource` указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="24557-163">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="24557-164">Например, вы можете создать подписку на определенную почтовую папку: `me/mailFolders('inbox')/messages` или сделать это от имени пользователя с согласия администратора: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="24557-164">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="24557-165">Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="24557-165">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="24557-166">Задание этого свойства позволит подтверждать, что полученные уведомления поступают от службы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24557-166">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="24557-167">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24557-167">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="24557-168">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24557-168">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="24557-169">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="24557-169">Notification endpoint validation</span></span>

<span data-ttu-id="24557-170">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="24557-170">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="24557-171">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="24557-171">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="24557-172">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="24557-172">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="24557-173">**Важно!** Так как `validationToken` — это параметр запроса, он должен декодироваться клиентом согласно правилам кодирования HTTP.</span><span class="sxs-lookup"><span data-stu-id="24557-173">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="24557-174">Если клиент не декодирует маркер и использует закодированное значение на следующем шаге (ответ), конечная точка не пройдет проверку.</span><span class="sxs-lookup"><span data-stu-id="24557-174">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="24557-175">Кроме того, клиент должен рассматривать значение маркера как непрозрачное, так как формат маркера может измениться в будущем без уведомления.</span><span class="sxs-lookup"><span data-stu-id="24557-175">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="24557-176">В течение 10 секунд клиент должен предоставить ответ со следующими характеристиками:</span><span class="sxs-lookup"><span data-stu-id="24557-176">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="24557-177">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="24557-177">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="24557-178">Необходимый тип контента — `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="24557-178">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="24557-179">Текст должен содержать маркер проверки, предоставленный Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24557-179">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="24557-180">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="24557-180">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="24557-181">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="24557-181">Renewing a subscription</span></span>

<span data-ttu-id="24557-182">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="24557-182">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="24557-183">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="24557-183">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="24557-184">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="24557-184">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="24557-185">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24557-185">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="24557-186">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="24557-186">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="24557-187">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="24557-187">Deleting a subscription</span></span>

<span data-ttu-id="24557-188">Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="24557-188">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="24557-189">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="24557-189">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="24557-190">Уведомления</span><span class="sxs-lookup"><span data-stu-id="24557-190">Notifications</span></span>

<span data-ttu-id="24557-191">После создания подписки клиент начнет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="24557-191">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="24557-192">При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="24557-192">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="24557-193">Уведомления отправляются только при изменениях типа, указанного в подписке, например, `created`.</span><span class="sxs-lookup"><span data-stu-id="24557-193">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="24557-194">**Примечание.** Если вы используете несколько подписок, которые отслеживают один тип ресурса и имеют один URL-адрес уведомлений, может быть отправлено сообщение POST, содержащее несколько уведомлений с разными идентификаторами подписок.</span><span class="sxs-lookup"><span data-stu-id="24557-194">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="24557-195">Уведомления из сообщения POST могут принадлежать разным подпискам.</span><span class="sxs-lookup"><span data-stu-id="24557-195">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="24557-196">Свойства уведомлений</span><span class="sxs-lookup"><span data-stu-id="24557-196">Notification properties</span></span>

<span data-ttu-id="24557-197">Объект уведомления содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="24557-197">The notification object has the following properties:</span></span>

| <span data-ttu-id="24557-198">Свойство</span><span class="sxs-lookup"><span data-stu-id="24557-198">Property</span></span> | <span data-ttu-id="24557-199">Тип</span><span class="sxs-lookup"><span data-stu-id="24557-199">Type</span></span> | <span data-ttu-id="24557-200">Описание</span><span class="sxs-lookup"><span data-stu-id="24557-200">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="24557-201">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="24557-201">subscriptionId</span></span> | <span data-ttu-id="24557-202">строка</span><span class="sxs-lookup"><span data-stu-id="24557-202">string</span></span> | <span data-ttu-id="24557-203">Идентификатор подписки, для которого было создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="24557-203">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="24557-204">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="24557-204">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="24557-205">дата и время</span><span class="sxs-lookup"><span data-stu-id="24557-205">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="24557-206">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="24557-206">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="24557-207">clientState</span><span class="sxs-lookup"><span data-stu-id="24557-207">clientState</span></span> | <span data-ttu-id="24557-208">строка</span><span class="sxs-lookup"><span data-stu-id="24557-208">string</span></span> | <span data-ttu-id="24557-209">`clientState` — свойство, указанное в запросе на подписку (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="24557-209">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="24557-210">changeType</span><span class="sxs-lookup"><span data-stu-id="24557-210">changeType</span></span> | <span data-ttu-id="24557-211">строка</span><span class="sxs-lookup"><span data-stu-id="24557-211">string</span></span> | <span data-ttu-id="24557-212">Тип события, вызвавшего уведомление.</span><span class="sxs-lookup"><span data-stu-id="24557-212">The event type that caused the notification.</span></span> <span data-ttu-id="24557-213">Примеры: `created` при получении сообщения или `updated`, когда сообщение помечается как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="24557-213">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="24557-214">resource</span><span class="sxs-lookup"><span data-stu-id="24557-214">resource</span></span> | <span data-ttu-id="24557-215">строка</span><span class="sxs-lookup"><span data-stu-id="24557-215">string</span></span> | <span data-ttu-id="24557-216">Универсальный код ресурса (URI) ресурса относительно `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="24557-216">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="24557-217">resourceData</span><span class="sxs-lookup"><span data-stu-id="24557-217">resourceData</span></span> | <span data-ttu-id="24557-218">объект</span><span class="sxs-lookup"><span data-stu-id="24557-218">object</span></span> | <span data-ttu-id="24557-219">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="24557-219">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="24557-220">Например, для ресурсов Outlook `resourceData` содержит такие поля:</span><span class="sxs-lookup"><span data-stu-id="24557-220">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="24557-221">Свойство</span><span class="sxs-lookup"><span data-stu-id="24557-221">Property</span></span> | <span data-ttu-id="24557-222">Тип</span><span class="sxs-lookup"><span data-stu-id="24557-222">Type</span></span> | <span data-ttu-id="24557-223">Описание</span><span class="sxs-lookup"><span data-stu-id="24557-223">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="24557-224">@odata.type</span><span class="sxs-lookup"><span data-stu-id="24557-224">@odata.type</span></span> | <span data-ttu-id="24557-225">строка</span><span class="sxs-lookup"><span data-stu-id="24557-225">string</span></span> | <span data-ttu-id="24557-226">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="24557-226">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="24557-227">@odata.id</span><span class="sxs-lookup"><span data-stu-id="24557-227">@odata.id</span></span> | <span data-ttu-id="24557-228">строка</span><span class="sxs-lookup"><span data-stu-id="24557-228">string</span></span> | <span data-ttu-id="24557-229">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="24557-229">The OData identifier of the object.</span></span> |
| <span data-ttu-id="24557-230">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="24557-230">@odata.etag</span></span> | <span data-ttu-id="24557-231">строка</span><span class="sxs-lookup"><span data-stu-id="24557-231">string</span></span> | <span data-ttu-id="24557-232">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="24557-232">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="24557-233">id</span><span class="sxs-lookup"><span data-stu-id="24557-233">id</span></span> | <span data-ttu-id="24557-234">строка</span><span class="sxs-lookup"><span data-stu-id="24557-234">string</span></span> | <span data-ttu-id="24557-235">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="24557-235">The identifier of the object.</span></span> |

> <span data-ttu-id="24557-236">**Примечание.** Значение `id`, указанное в `resourceData`, действительно в момент создания уведомления.</span><span class="sxs-lookup"><span data-stu-id="24557-236">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="24557-237">Некоторые действия, такие как перемещение сообщения в другую папку, могут привести к недействительности `id` во время обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="24557-237">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="24557-238">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="24557-238">Notification example</span></span>

<span data-ttu-id="24557-239">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления, аналогичные указанному ниже.</span><span class="sxs-lookup"><span data-stu-id="24557-239">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="24557-240">Обратите внимание, что поле `value` представляет собой массив объектов.</span><span class="sxs-lookup"><span data-stu-id="24557-240">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="24557-241">Если в очереди много уведомлений, Microsoft Graph может отправлять несколько элементов в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="24557-241">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="24557-242">В одном запросе уведомления могут содержаться уведомления от разных подписок.</span><span class="sxs-lookup"><span data-stu-id="24557-242">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="24557-243">Обработка уведомления</span><span class="sxs-lookup"><span data-stu-id="24557-243">Processing the notification</span></span>

<span data-ttu-id="24557-244">Необходимо обрабатывать все уведомления, полученные программой.</span><span class="sxs-lookup"><span data-stu-id="24557-244">Each notification received by your app should be processed.</span></span> <span data-ttu-id="24557-245">Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.</span><span class="sxs-lookup"><span data-stu-id="24557-245">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="24557-246">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="24557-246">Validate the `clientState` property.</span></span> <span data-ttu-id="24557-247">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="24557-247">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="24557-248">**Примечание.** Если это не так, уведомление не следует рассматривать как действительное.</span><span class="sxs-lookup"><span data-stu-id="24557-248">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="24557-249">Возможно уведомление создано не Microsoft Graph и отправлено незаконным субъектом.</span><span class="sxs-lookup"><span data-stu-id="24557-249">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="24557-250">Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="24557-250">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="24557-251">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="24557-251">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="24557-252">Отправляйте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24557-252">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="24557-253">Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="24557-253">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="24557-254">**Примечание.** Код состояния `202 - Accepted` следует отправлять, даже если свойство `clientState` не совпадает со значением, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="24557-254">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="24557-255">Такие действия не позволяют потенциальным незаконным субъектам обнаружить факт недоверия к их уведомлениям и воспользоваться этой информацией, чтобы угадать значение свойства `clientState`.</span><span class="sxs-lookup"><span data-stu-id="24557-255">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="24557-256">Повторяйте эти действия для других уведомлений в запросе.</span><span class="sxs-lookup"><span data-stu-id="24557-256">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="24557-257">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="24557-257">Code samples</span></span>

<span data-ttu-id="24557-258">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="24557-258">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="24557-259">Обучающий модуль по Microsoft Graph: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="24557-259">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="24557-260">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="24557-260">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="24557-261">Пример веб-перехватчиков Microsoft Graph для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="24557-261">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="24557-262">Пример веб-перехватчиков Microsoft Graph для WebJobs SDK</span><span class="sxs-lookup"><span data-stu-id="24557-262">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="24557-263">См. также</span><span class="sxs-lookup"><span data-stu-id="24557-263">See also</span></span>

- [<span data-ttu-id="24557-264">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="24557-264">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="24557-265">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="24557-265">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="24557-266">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="24557-266">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="24557-267">Учебник по уведомлениям об изменениях</span><span class="sxs-lookup"><span data-stu-id="24557-267">Change notifications tutorial</span></span>](/graph/tutorials/change-notifications)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
