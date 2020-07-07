---
title: Настройка уведомлений об изменениях в пользовательских данных
description: The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 47c4357a59b02322769433fb82d0e9fe02fc1aae
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050927"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="607f7-105">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="607f7-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="607f7-106">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients.</span><span class="sxs-lookup"><span data-stu-id="607f7-106">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="607f7-107">A client is a web service that configures its own URL to receive change notifications.</span><span class="sxs-lookup"><span data-stu-id="607f7-107">A client is a web service that configures its own URL to receive change notifications.</span></span> <span data-ttu-id="607f7-108">Client apps use change notifications to update their state upon changes.</span><span class="sxs-lookup"><span data-stu-id="607f7-108">Client apps use change notifications to update their state upon changes.</span></span>

<span data-ttu-id="607f7-109">Когда Microsoft Graph принимает запрос на подписку, он передает уведомления об изменениях URL-адресу, указанному в подписке.</span><span class="sxs-lookup"><span data-stu-id="607f7-109">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="607f7-110">Затем приложение действует в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="607f7-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="607f7-111">Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.</span><span class="sxs-lookup"><span data-stu-id="607f7-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="607f7-112">Руководство: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="607f7-112">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

<span data-ttu-id="607f7-113">По умолчанию уведомления об изменениях не включают данные ресурсов, кроме `id`.</span><span class="sxs-lookup"><span data-stu-id="607f7-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="607f7-114">Если приложению требуются данные ресурса, оно может вызвать API Microsoft Graph, чтобы получить ресурс полностью.</span><span class="sxs-lookup"><span data-stu-id="607f7-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="607f7-115">В этой статье ресурс **User** используется в качестве примера для работы с уведомлениями об изменениях.</span><span class="sxs-lookup"><span data-stu-id="607f7-115">This article uses the **user** resource as an example for working with change notifications.</span></span>

<span data-ttu-id="607f7-116">Приложение также может подписаться на уведомления об изменениях, включающие данные ресурсов, чтобы избежать необходимости дополнительного вызова API для доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="607f7-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additonal API calls to access the data.</span></span> <span data-ttu-id="607f7-117">В этом случае приложению необходимо реализовать дополнительный код для обработки требований таких уведомлений, в частности, ответа на уведомления о жизненном цикле подписки, проверки подлинности уведомлений и расшифровки данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="607f7-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="607f7-118">Другие типы ресурсов также будут поддерживать этот тип уведомлений в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="607f7-118">More resource types will support this type of notifications in the future.</span></span> <span data-ttu-id="607f7-119">Дополнительные сведения о работе с такими уведомлениями см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="607f7-119">For details about how to work with these notificatios, see [Set up change notifications that include resource data (preview)](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="607f7-120">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="607f7-120">Supported resources</span></span>

<span data-ttu-id="607f7-121">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="607f7-121">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="607f7-122">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="607f7-122">Outlook [message][]</span></span>
- <span data-ttu-id="607f7-123">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="607f7-123">Outlook [event][]</span></span>
- <span data-ttu-id="607f7-124">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="607f7-124">Outlook personal [contact][]</span></span>
- <span data-ttu-id="607f7-125">[user][]</span><span class="sxs-lookup"><span data-stu-id="607f7-125">[user][]</span></span>
- <span data-ttu-id="607f7-126">[group][]</span><span class="sxs-lookup"><span data-stu-id="607f7-126">[group][]</span></span>
- <span data-ttu-id="607f7-127">[Беседа][] группы (майкрософт) 365</span><span class="sxs-lookup"><span data-stu-id="607f7-127">Microsoft 365 group [conversation][]</span></span>
- <span data-ttu-id="607f7-128">Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="607f7-128">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="607f7-129">Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="607f7-129">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="607f7-130">[Оповещение][] безопасности</span><span class="sxs-lookup"><span data-stu-id="607f7-130">Security [alert][]</span></span>
- <span data-ttu-id="607f7-131">[Каллрекорд][] Teams</span><span class="sxs-lookup"><span data-stu-id="607f7-131">Teams [callRecord][]</span></span>
- <span data-ttu-id="607f7-132">Teams [chatMessage][] (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="607f7-132">Teams [chatMessage][] (preview)</span></span>
- <span data-ttu-id="607f7-133">[Присутствие][] в Teams (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="607f7-133">Teams [presence][] (preview)</span></span>

<span data-ttu-id="607f7-134">Например, вы можете создать подписку на определенную папку Outlook, например, папку Входящие: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="607f7-134">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="607f7-135">Или на ресурс верхнего уровня:,, `/me/messages` ,,, `/me/contacts` `/me/events` `users` `groups` `/communications/callRecords` , или`/communications/presences`</span><span class="sxs-lookup"><span data-stu-id="607f7-135">Or to a top-level resource: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, `/communications/callRecords`, or `/communications/presences`</span></span>

<span data-ttu-id="607f7-136">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`;</span><span class="sxs-lookup"><span data-stu-id="607f7-136">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="607f7-137">либо на личное хранилище OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="607f7-137">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="607f7-138">либо на корневую папку диска SharePoint/OneDrive для бизнеса: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="607f7-138">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="607f7-139">либо на новое оповещение [API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="607f7-139">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="607f7-140">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="607f7-140">Azure AD resource limitations</span></span>

<span data-ttu-id="607f7-141">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения возникают ошибки.</span><span class="sxs-lookup"><span data-stu-id="607f7-141">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="607f7-142">**Примечание**. Эти ограничения не применяются к ресурсам служб, не относящихся к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="607f7-142">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="607f7-143">Например, приложение может создать больше дополнительных подписок на ресурсы `message` или `event`, поддерживаемые службой Exchange Online в составе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="607f7-143">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="607f7-144">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="607f7-144">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="607f7-145">Для каждого приложения (для всех клиентов): 50 000 всего подписок</span><span class="sxs-lookup"><span data-stu-id="607f7-145">Per app (for all tenants combined): 50,000 total subscriptions</span></span>
  - <span data-ttu-id="607f7-146">Для каждого клиента (для всех приложений в совокупности): 1000 всего подписок для всех приложений</span><span class="sxs-lookup"><span data-stu-id="607f7-146">Per tenant (for all applications combined): 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="607f7-147">На сочетание приложения и клиента: 100 подписок всего</span><span class="sxs-lookup"><span data-stu-id="607f7-147">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="607f7-148">При превышении какого-либо ограничения попытки создать подписку приведут к возникновению [ошибки](errors.md)  -  `403 Forbidden` .</span><span class="sxs-lookup"><span data-stu-id="607f7-148">When any limit is exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="607f7-149">Свойство `message` указывает, какое ограничение превышено.</span><span class="sxs-lookup"><span data-stu-id="607f7-149">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="607f7-150">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="607f7-150">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="607f7-151">Уведомление чангфе для пользовательских сущностей не поддерживается для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="607f7-151">Changfe notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="607f7-152">В подписках пользователей и групп существует [известная проблема](known-issues.md#change-notifications).</span><span class="sxs-lookup"><span data-stu-id="607f7-152">A [known issue](known-issues.md#change-notifications) exists with user and group subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="607f7-153">Ограничения ресурсов Outlook</span><span class="sxs-lookup"><span data-stu-id="607f7-153">Outlook resource limitations</span></span>

<span data-ttu-id="607f7-154">Если вы используете *имя участника-пользователя* на пути к ресурсу при оформлении подписки на ресурсы Outlook, например **сообщения**, **события** или **контакты**, запрос на подписку может быть не выполнен, если это имя содержит апостроф. </span><span class="sxs-lookup"><span data-stu-id="607f7-154">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="607f7-155">Используйте ИД GUID пользователей вместо имен участников-пользователей, чтобы избежать этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="607f7-155">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="607f7-156">Например, вместо пути к ресурсу:</span><span class="sxs-lookup"><span data-stu-id="607f7-156">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="607f7-157">Используйте:</span><span class="sxs-lookup"><span data-stu-id="607f7-157">Use:</span></span> 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a><span data-ttu-id="607f7-158">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="607f7-158">Subscription lifetime</span></span>

<span data-ttu-id="607f7-159">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="607f7-159">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="607f7-160">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="607f7-160">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="607f7-161">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="607f7-161">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="607f7-162">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="607f7-162">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="607f7-163">Кроме того, приложения могут отменять подписку в любое время, чтобы остановить получение уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="607f7-163">Apps can also unsubscribe at any time to stop getting change notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="607f7-164">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="607f7-164">Managing subscriptions</span></span>

<span data-ttu-id="607f7-165">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="607f7-165">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="607f7-166">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="607f7-166">Creating a subscription</span></span>

<span data-ttu-id="607f7-167">Создание подписки — это первый шаг к началу получения уведомлений об изменениях для ресурса.</span><span class="sxs-lookup"><span data-stu-id="607f7-167">Creating a subscription is the first step to start receiving change notifications for a resource.</span></span> <span data-ttu-id="607f7-168">Это происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="607f7-168">The subscription process is as follows:</span></span>

1. <span data-ttu-id="607f7-169">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="607f7-169">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="607f7-170">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="607f7-170">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="607f7-171">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="607f7-171">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="607f7-172">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="607f7-172">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="607f7-173">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="607f7-173">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="607f7-174">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="607f7-174">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="607f7-175">Клиент должен хранить идентификатор подписки, чтобы сопоставить уведомления об изменениях с подпиской.</span><span class="sxs-lookup"><span data-stu-id="607f7-175">The client must store the subscription ID to correlate change notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="607f7-176">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="607f7-176">Subscription request example</span></span>

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

<span data-ttu-id="607f7-177">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="607f7-177">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="607f7-178">Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="607f7-178">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="607f7-179">Свойство `resource` указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="607f7-179">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="607f7-180">Например, вы можете создать подписку на определенную почтовую папку: `me/mailFolders('inbox')/messages` или сделать это от имени пользователя с согласия администратора: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="607f7-180">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="607f7-181">Хотя `clientState` это не обязательно, необходимо включить его в соответствии с рекомендуемым процессом обработки уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="607f7-181">Although `clientState` is not required, you must include it to comply with our recommended change notification handling process.</span></span> <span data-ttu-id="607f7-182">Задание этого свойства позволяет подтвердить, что уведомления об изменениях, получаемые от службы Microsoft Graph, вы можете подтвердить.</span><span class="sxs-lookup"><span data-stu-id="607f7-182">Setting this property will allow you to confirm that change notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="607f7-183">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="607f7-183">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="607f7-184">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="607f7-184">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="607f7-185">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="607f7-185">Notification endpoint validation</span></span>

<span data-ttu-id="607f7-186">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="607f7-186">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="607f7-187">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="607f7-187">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="607f7-188">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="607f7-188">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="607f7-189">**Важно!** Так как `validationToken` — это параметр запроса, он должен декодироваться клиентом согласно правилам кодирования HTTP.</span><span class="sxs-lookup"><span data-stu-id="607f7-189">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="607f7-190">Если клиент не декодирует маркер и использует закодированное значение на следующем шаге (ответ), конечная точка не пройдет проверку.</span><span class="sxs-lookup"><span data-stu-id="607f7-190">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="607f7-191">Кроме того, клиент должен рассматривать значение маркера как непрозрачное, так как формат маркера может измениться в будущем без уведомления.</span><span class="sxs-lookup"><span data-stu-id="607f7-191">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="607f7-192">В течение 10 секунд клиент должен предоставить ответ со следующими характеристиками:</span><span class="sxs-lookup"><span data-stu-id="607f7-192">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="607f7-193">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="607f7-193">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="607f7-194">Необходимый тип контента — `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="607f7-194">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="607f7-195">Текст должен содержать маркер проверки, предоставленный Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="607f7-195">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="607f7-196">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="607f7-196">The client should discard the validation token after providing it in the response.</span></span>

<span data-ttu-id="607f7-197">Кроме того, можно использовать [коллекцию Microsoft Graph Postman](use-postman.md), чтобы убедиться в правильности реализации запроса проверки в вашей конечной точке.</span><span class="sxs-lookup"><span data-stu-id="607f7-197">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="607f7-198">Запрос **Проверка подписки** в папке **Прочее** предоставляет модульные тесты, проверяющие отклик вашей конечной точки.</span><span class="sxs-lookup"><span data-stu-id="607f7-198">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![результаты теста отклика проверки](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="607f7-200">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="607f7-200">Renewing a subscription</span></span>

<span data-ttu-id="607f7-201">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="607f7-201">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="607f7-202">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="607f7-202">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="607f7-203">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="607f7-203">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="607f7-204">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="607f7-204">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="607f7-205">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="607f7-205">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="607f7-206">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="607f7-206">Deleting a subscription</span></span>

<span data-ttu-id="607f7-207">Клиент может прекратить получать уведомления об изменениях, удалив подписку с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="607f7-207">The client can stop receiving change notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="607f7-208">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="607f7-208">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="607f7-209">Уведомления об изменениях</span><span class="sxs-lookup"><span data-stu-id="607f7-209">Change notifications</span></span>

<span data-ttu-id="607f7-210">Если клиент выполняет подписку на изменения ресурса, Microsoft Graph отправляет `POST` запрос на URL-адрес уведомлений при каждом изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="607f7-210">With a client subscribing to changes to a resource, Microsoft Graph sends a `POST` request to the notification URL whenever the resource changes.</span></span> <span data-ttu-id="607f7-211">Он отправляет уведомления только для тех изменений типа, которые указаны в подписке, например `created` .</span><span class="sxs-lookup"><span data-stu-id="607f7-211">It sends notifications only for changes of the type that's specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="607f7-212">**Примечание:** Если клиент имеет несколько подписок, контролирующих один и тот же URL-адрес уведомления, Microsoft Graph может отправлять несколько уведомлений об изменениях, соответствующих разным подпискам, каждый из которых отображает соответствующий идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="607f7-212">**Note:** If a client has multiple subscriptions that monitor the same resource and use the same notification URL, Microsoft Graph can send multiple change notifications that correspond to different subscriptions, each showing the corresponding subscription ID.</span></span> <span data-ttu-id="607f7-213">Нет гарантии, что все уведомления об изменениях в `POST` запросе принадлежат одной подписке.</span><span class="sxs-lookup"><span data-stu-id="607f7-213">There is no guarantee that all change notifications in the `POST` request belong to a single subscription.</span></span>

### <a name="change-notification-example"></a><span data-ttu-id="607f7-214">Пример уведомления об изменении</span><span class="sxs-lookup"><span data-stu-id="607f7-214">Change notification example</span></span>

<span data-ttu-id="607f7-215">В этом разделе представлен пример уведомления для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="607f7-215">This section shows an example of a notification for a message creation.</span></span> <span data-ttu-id="607f7-216">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомление об изменении, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="607f7-216">When the user receives an email, Microsoft Graph sends a change notification as shown in the following example.</span></span>
<span data-ttu-id="607f7-217">Обратите внимание, что уведомление представлено в коллекции, представленной в `value` поле.</span><span class="sxs-lookup"><span data-stu-id="607f7-217">Note that the notification is in a collection represented in the `value` field.</span></span> <span data-ttu-id="607f7-218">Сведения о полезных данных уведомления можно найти в [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection) .</span><span class="sxs-lookup"><span data-stu-id="607f7-218">See [changeNotificationCollection](/graph/api/resources/changenotificationcollection) for details of the notification payload.</span></span> 

<span data-ttu-id="607f7-219">При возникновении большого количества изменений Microsoft Graph может отправлять несколько уведомлений, соответствующих разным подпискам в одном `POST` запросе.</span><span class="sxs-lookup"><span data-stu-id="607f7-219">When many changes occur, Microsoft Graph may send multiple notifications that correspond to different subscriptions in the same `POST` request.</span></span>

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
      "subscriptionId":"{subscription_guid}",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@{tenant_guid}/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@{tenant_guid}/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"{long_id_string}"
      }
    }
  ]
}
```

### <a name="processing-the-change-notification"></a><span data-ttu-id="607f7-220">Обработка уведомления об изменении</span><span class="sxs-lookup"><span data-stu-id="607f7-220">Processing the change notification</span></span>

<span data-ttu-id="607f7-221">Процесс должен обрабатывать каждое уведомление об изменении, которое он получает.</span><span class="sxs-lookup"><span data-stu-id="607f7-221">Your process should process every change notification it receives.</span></span> <span data-ttu-id="607f7-222">Ниже приведены минимальные задачи, которые приложение должно выполнить для обработки уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="607f7-222">The following are the minimum tasks that your app must perform to process a change notification:</span></span>

1. <span data-ttu-id="607f7-223">Отправьте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="607f7-223">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="607f7-224">Если Microsoft Graph не получает код класса 2xx, он попытается опубликовать уведомление об изменении несколько раз в течение 4 часов; После этого уведомление об изменении будет удалено и не будет доставлено.</span><span class="sxs-lookup"><span data-stu-id="607f7-224">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the change notification a number of times, for a period of about 4 hours; after that, the change notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="607f7-225">**Примечание:** Отправьте код состояния сразу же после `202 - Accepted` получения уведомления об изменении, даже перед проверкой его подлинности.</span><span class="sxs-lookup"><span data-stu-id="607f7-225">**Note:** Send a `202 - Accepted` status code as soon as you receive the change notification, even before validating its authenticity.</span></span> <span data-ttu-id="607f7-226">Вы просто подтверждаете получение уведомления об изменении и предотвратите ненужные попытки.</span><span class="sxs-lookup"><span data-stu-id="607f7-226">You are simply acknowledging the receipt of the change notification and preventing unnecessary retries.</span></span> <span data-ttu-id="607f7-227">Текущее значение времени ожидания — 30 секунд, но это время может быть сокращено в будущем для оптимизации производительности службы.</span><span class="sxs-lookup"><span data-stu-id="607f7-227">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span> <span data-ttu-id="607f7-228">Если URL-адрес уведомления не отвечает в течение 30 секунд для более чем 10% запросов от Microsoft Graph за 10 минут, все следующие уведомления будут задержаны и повторены в течение 4 часов.</span><span class="sxs-lookup"><span data-stu-id="607f7-228">If the notification URL doesn't reply within 30 seconds for more than 10% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be delayed and retried for a period of 4 hours.</span></span> <span data-ttu-id="607f7-229">Если URL-адрес уведомления не отвечает в течение 30 секунд за более 20% запросов от Microsoft Graph за 10 минут, будут удалены все следующие уведомления.</span><span class="sxs-lookup"><span data-stu-id="607f7-229">If a notification URL doesn't reply within 30 seconds for more than 20% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be dropped.</span></span>

1. <span data-ttu-id="607f7-230">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="607f7-230">Validate the `clientState` property.</span></span> <span data-ttu-id="607f7-231">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="607f7-231">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="607f7-232">**Примечание:** Если это не так, вы не должны считать это действительное уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="607f7-232">**Note:** If this isn't true, you should not consider this a valid change notification.</span></span> <span data-ttu-id="607f7-233">Возможно, что уведомление об изменении не получено из Microsoft Graph и может быть отправлено фальшивым субъектом.</span><span class="sxs-lookup"><span data-stu-id="607f7-233">It is possible that the change notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="607f7-234">Кроме того, следует проверить, откуда поступило уведомление об изменении, и предпринять соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="607f7-234">You should also investigate where the change notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="607f7-235">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="607f7-235">Update your application based on your business logic.</span></span>

<span data-ttu-id="607f7-236">Повторите эти действия для других уведомлений об изменении в запросе.</span><span class="sxs-lookup"><span data-stu-id="607f7-236">Repeat for other change notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="607f7-237">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="607f7-237">Code samples</span></span>

<span data-ttu-id="607f7-238">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="607f7-238">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="607f7-239">Обучающий модуль по Microsoft Graph: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="607f7-239">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="607f7-240">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="607f7-240">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [<span data-ttu-id="607f7-241">Пример веб-перехватчиков Microsoft Graph для ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="607f7-241">Microsoft Graph Webhooks Sample for ASP.NET Core</span></span>](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [<span data-ttu-id="607f7-242">Пример веб-перехватчиков Microsoft Graph для Java Spring</span><span class="sxs-lookup"><span data-stu-id="607f7-242">Microsoft Graph Webhooks Sample for Java Spring</span></span>](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a><span data-ttu-id="607f7-243">Конфигурация брандмауэра</span><span class="sxs-lookup"><span data-stu-id="607f7-243">Firewall configuration</span></span>

<span data-ttu-id="607f7-244">При необходимости можно настроить брандмауэр, защищающий URL-адрес уведомлений, чтобы разрешить входящие подключения только из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="607f7-244">You can optionally configure the firewall that protects your notification URL to allow inbound connections only from Microsoft Graph.</span></span> <span data-ttu-id="607f7-245">Это позволяет уменьшить риск недопустимых уведомлений об изменениях, отправляемых на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="607f7-245">This allows you to reduce further exposure to invalid change notifications that are sent to your notification URL.</span></span> <span data-ttu-id="607f7-246">Эти недопустимые уведомления об изменении могут пытаться активировать реализованную пользовательскую логику.</span><span class="sxs-lookup"><span data-stu-id="607f7-246">These invalid change notifications can be trying to trigger the custom logic that you implemented.</span></span> <span data-ttu-id="607f7-247">Полный список IP-адресов, используемых Microsoft Graph для доставки уведомлений об изменениях, приведен в разделе [дополнительные конечные точки для microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span><span class="sxs-lookup"><span data-stu-id="607f7-247">For a complete list of IP addresses used by Microsoft Graph to deliver change notifications, see [additional endpoints for Microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span></span>

> <span data-ttu-id="607f7-248">**Примечание:** Указанные IP-адреса, используемые для доставки уведомлений об изменениях, можно обновить в любое время без уведомления.</span><span class="sxs-lookup"><span data-stu-id="607f7-248">**Note:** The listed IP addresses that are used to deliver change notifications can be updated at any time without notice.</span></span>

## <a name="see-also"></a><span data-ttu-id="607f7-249">См. также</span><span class="sxs-lookup"><span data-stu-id="607f7-249">See also</span></span>

- [<span data-ttu-id="607f7-250">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="607f7-250">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="607f7-251">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="607f7-251">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="607f7-252">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="607f7-252">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- <span data-ttu-id="607f7-253">Тип ресурса [чанженотификатион](/graph/api/resources/changenotification?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="607f7-253">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) resource type</span></span>
- <span data-ttu-id="607f7-254">Тип ресурса [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="607f7-254">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) resource type</span></span>
- [<span data-ttu-id="607f7-255">Руководство по изменениям уведомлений и отслеживания изменений</span><span class="sxs-lookup"><span data-stu-id="607f7-255">Change notifications and change tracking tutorial</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)
- [<span data-ttu-id="607f7-256">Уведомления в жизненном цикле (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="607f7-256">Lifecycle notifications (preview)</span></span>](/graph/concepts/webhooks-outlook-authz.md)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-1.0
[presence]: /graph/api/resources/presence
[chatMessage]: /graph/api/resources/chatmessage
