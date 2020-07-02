---
title: Настройка уведомлений об изменениях в пользовательских данных
description: The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7db6b2498d039a4f6474b530023a9f4c0e199119
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989781"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="28e97-105">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="28e97-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="28e97-106">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients.</span><span class="sxs-lookup"><span data-stu-id="28e97-106">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="28e97-107">A client is a web service that configures its own URL to receive change notifications.</span><span class="sxs-lookup"><span data-stu-id="28e97-107">A client is a web service that configures its own URL to receive change notifications.</span></span> <span data-ttu-id="28e97-108">Client apps use change notifications to update their state upon changes.</span><span class="sxs-lookup"><span data-stu-id="28e97-108">Client apps use change notifications to update their state upon changes.</span></span>

<span data-ttu-id="28e97-109">Когда Microsoft Graph принимает запрос на подписку, он передает уведомления об изменениях URL-адресу, указанному в подписке.</span><span class="sxs-lookup"><span data-stu-id="28e97-109">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="28e97-110">Затем приложение действует в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="28e97-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="28e97-111">Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.</span><span class="sxs-lookup"><span data-stu-id="28e97-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="28e97-112">Руководство: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="28e97-112">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

<span data-ttu-id="28e97-113">По умолчанию уведомления об изменениях не включают данные ресурсов, кроме `id`.</span><span class="sxs-lookup"><span data-stu-id="28e97-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="28e97-114">Если приложению требуются данные ресурса, оно может вызвать API Microsoft Graph, чтобы получить ресурс полностью.</span><span class="sxs-lookup"><span data-stu-id="28e97-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="28e97-115">В этой статье ресурс **User** используется в качестве примера для работы с уведомлениями об изменениях.</span><span class="sxs-lookup"><span data-stu-id="28e97-115">This article uses the **user** resource as an example for working with change notifications.</span></span>

<span data-ttu-id="28e97-116">Приложение также может подписаться на уведомления об изменениях, включающие данные ресурсов, чтобы избежать необходимости дополнительного вызова API для доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="28e97-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additonal API calls to access the data.</span></span> <span data-ttu-id="28e97-117">В этом случае приложению необходимо реализовать дополнительный код для обработки требований таких уведомлений, в частности, ответа на уведомления о жизненном цикле подписки, проверки подлинности уведомлений и расшифровки данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="28e97-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="28e97-118">Другие типы ресурсов также будут поддерживать этот тип уведомлений в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="28e97-118">More resource types will support this type of notifications in the future.</span></span> <span data-ttu-id="28e97-119">Дополнительные сведения о работе с такими уведомлениями см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="28e97-119">For details about how to work with these notificatios, see [Set up change notifications that include resource data (preview)](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="28e97-120">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="28e97-120">Supported resources</span></span>

<span data-ttu-id="28e97-121">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="28e97-121">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="28e97-122">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="28e97-122">Outlook [message][]</span></span>
- <span data-ttu-id="28e97-123">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="28e97-123">Outlook [event][]</span></span>
- <span data-ttu-id="28e97-124">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="28e97-124">Outlook personal [contact][]</span></span>
- <span data-ttu-id="28e97-125">[user][]</span><span class="sxs-lookup"><span data-stu-id="28e97-125">[user][]</span></span>
- <span data-ttu-id="28e97-126">[group][]</span><span class="sxs-lookup"><span data-stu-id="28e97-126">[group][]</span></span>
- <span data-ttu-id="28e97-127">[Беседа][] группы (майкрософт) 365</span><span class="sxs-lookup"><span data-stu-id="28e97-127">Microsoft 365 group [conversation][]</span></span>
- <span data-ttu-id="28e97-128">Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="28e97-128">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="28e97-129">Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="28e97-129">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="28e97-130">[Оповещение][] безопасности</span><span class="sxs-lookup"><span data-stu-id="28e97-130">Security [alert][]</span></span>
- <span data-ttu-id="28e97-131">[Каллрекорд][] Teams</span><span class="sxs-lookup"><span data-stu-id="28e97-131">Teams [callRecord][]</span></span>
- <span data-ttu-id="28e97-132">Teams [chatMessage][] (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="28e97-132">Teams [chatMessage][] (preview)</span></span>

<span data-ttu-id="28e97-133">Например, вы можете создать подписку на определенную папку Outlook, например, папку Входящие: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="28e97-133">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="28e97-134">Или на ресурс верхнего уровня:,, `/me/messages` `/me/contacts` ,, `/me/events` `users` `groups` или`/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="28e97-134">Or to a top-level resource: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, or `/communications/callRecords`</span></span>

<span data-ttu-id="28e97-135">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`;</span><span class="sxs-lookup"><span data-stu-id="28e97-135">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="28e97-136">либо на личное хранилище OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="28e97-136">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="28e97-137">либо на корневую папку диска SharePoint/OneDrive для бизнеса: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="28e97-137">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="28e97-138">либо на новое оповещение [API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="28e97-138">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="28e97-139">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="28e97-139">Azure AD resource limitations</span></span>

<span data-ttu-id="28e97-140">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения возникают ошибки.</span><span class="sxs-lookup"><span data-stu-id="28e97-140">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="28e97-141">**Примечание**. Эти ограничения не применяются к ресурсам служб, не относящихся к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28e97-141">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="28e97-142">Например, приложение может создать больше дополнительных подписок на ресурсы `message` или `event`, поддерживаемые службой Exchange Online в составе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e97-142">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="28e97-143">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="28e97-143">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="28e97-144">Для каждого приложения (для всех клиентов): 50 000 всего подписок</span><span class="sxs-lookup"><span data-stu-id="28e97-144">Per app (for all tenants combined): 50,000 total subscriptions</span></span>
  - <span data-ttu-id="28e97-145">Для каждого клиента (для всех приложений в совокупности): 1000 всего подписок для всех приложений</span><span class="sxs-lookup"><span data-stu-id="28e97-145">Per tenant (for all applications combined): 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="28e97-146">На сочетание приложения и клиента: 100 подписок всего</span><span class="sxs-lookup"><span data-stu-id="28e97-146">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="28e97-147">При превышении какого-либо ограничения попытки создать подписку приведут к возникновению [ошибки](errors.md)  -  `403 Forbidden` .</span><span class="sxs-lookup"><span data-stu-id="28e97-147">When any limit is exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="28e97-148">Свойство `message` указывает, какое ограничение превышено.</span><span class="sxs-lookup"><span data-stu-id="28e97-148">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="28e97-149">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="28e97-149">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="28e97-150">Уведомление чангфе для пользовательских сущностей не поддерживается для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="28e97-150">Changfe notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="28e97-151">В подписках пользователей и групп существует [известная проблема](known-issues.md#change-notifications).</span><span class="sxs-lookup"><span data-stu-id="28e97-151">A [known issue](known-issues.md#change-notifications) exists with user and group subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="28e97-152">Ограничения ресурсов Outlook</span><span class="sxs-lookup"><span data-stu-id="28e97-152">Outlook resource limitations</span></span>

<span data-ttu-id="28e97-153">Если вы используете *имя участника-пользователя* на пути к ресурсу при оформлении подписки на ресурсы Outlook, например **сообщения**, **события** или **контакты**, запрос на подписку может быть не выполнен, если это имя содержит апостроф. </span><span class="sxs-lookup"><span data-stu-id="28e97-153">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="28e97-154">Используйте ИД GUID пользователей вместо имен участников-пользователей, чтобы избежать этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="28e97-154">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="28e97-155">Например, вместо пути к ресурсу:</span><span class="sxs-lookup"><span data-stu-id="28e97-155">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="28e97-156">Используйте:</span><span class="sxs-lookup"><span data-stu-id="28e97-156">Use:</span></span> 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a><span data-ttu-id="28e97-157">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="28e97-157">Subscription lifetime</span></span>

<span data-ttu-id="28e97-158">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="28e97-158">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="28e97-159">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="28e97-159">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="28e97-160">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="28e97-160">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="28e97-161">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="28e97-161">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="28e97-162">Кроме того, приложения могут отменять подписку в любое время, чтобы остановить получение уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="28e97-162">Apps can also unsubscribe at any time to stop getting change notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="28e97-163">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="28e97-163">Managing subscriptions</span></span>

<span data-ttu-id="28e97-164">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="28e97-164">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="28e97-165">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="28e97-165">Creating a subscription</span></span>

<span data-ttu-id="28e97-166">Creating a subscription is the first step to start receiving change notifications for a resource.</span><span class="sxs-lookup"><span data-stu-id="28e97-166">Creating a subscription is the first step to start receiving change notifications for a resource.</span></span> <span data-ttu-id="28e97-167">The subscription process is as follows:</span><span class="sxs-lookup"><span data-stu-id="28e97-167">The subscription process is as follows:</span></span>

1. <span data-ttu-id="28e97-168">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="28e97-168">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="28e97-169">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="28e97-169">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="28e97-170">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="28e97-170">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="28e97-171">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="28e97-171">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="28e97-172">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e97-172">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="28e97-173">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e97-173">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="28e97-174">Клиент должен хранить идентификатор подписки, чтобы сопоставить уведомления об изменениях с подпиской.</span><span class="sxs-lookup"><span data-stu-id="28e97-174">The client must store the subscription ID to correlate change notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="28e97-175">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="28e97-175">Subscription request example</span></span>

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

<span data-ttu-id="28e97-176">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="28e97-176">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="28e97-177">Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="28e97-177">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="28e97-178">Свойство `resource` указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="28e97-178">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="28e97-179">Например, вы можете создать подписку на определенную почтовую папку: `me/mailFolders('inbox')/messages` или сделать это от имени пользователя с согласия администратора: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="28e97-179">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="28e97-180">Хотя `clientState` это не обязательно, необходимо включить его в соответствии с рекомендуемым процессом обработки уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="28e97-180">Although `clientState` is not required, you must include it to comply with our recommended change notification handling process.</span></span> <span data-ttu-id="28e97-181">Задание этого свойства позволяет подтвердить, что уведомления об изменениях, получаемые от службы Microsoft Graph, вы можете подтвердить.</span><span class="sxs-lookup"><span data-stu-id="28e97-181">Setting this property will allow you to confirm that change notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="28e97-182">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e97-182">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="28e97-183">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28e97-183">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="28e97-184">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="28e97-184">Notification endpoint validation</span></span>

<span data-ttu-id="28e97-185">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="28e97-185">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="28e97-186">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="28e97-186">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="28e97-187">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="28e97-187">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="28e97-188">**Важно!** Так как `validationToken` — это параметр запроса, он должен декодироваться клиентом согласно правилам кодирования HTTP.</span><span class="sxs-lookup"><span data-stu-id="28e97-188">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="28e97-189">Если клиент не декодирует маркер и использует закодированное значение на следующем шаге (ответ), конечная точка не пройдет проверку.</span><span class="sxs-lookup"><span data-stu-id="28e97-189">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="28e97-190">Кроме того, клиент должен рассматривать значение маркера как непрозрачное, так как формат маркера может измениться в будущем без уведомления.</span><span class="sxs-lookup"><span data-stu-id="28e97-190">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="28e97-191">В течение 10 секунд клиент должен предоставить ответ со следующими характеристиками:</span><span class="sxs-lookup"><span data-stu-id="28e97-191">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="28e97-192">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="28e97-192">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="28e97-193">Необходимый тип контента — `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="28e97-193">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="28e97-194">Текст должен содержать маркер проверки, предоставленный Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e97-194">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="28e97-195">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="28e97-195">The client should discard the validation token after providing it in the response.</span></span>

<span data-ttu-id="28e97-196">Кроме того, можно использовать [коллекцию Microsoft Graph Postman](use-postman.md), чтобы убедиться в правильности реализации запроса проверки в вашей конечной точке.</span><span class="sxs-lookup"><span data-stu-id="28e97-196">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="28e97-197">Запрос **Проверка подписки** в папке **Прочее** предоставляет модульные тесты, проверяющие отклик вашей конечной точки.</span><span class="sxs-lookup"><span data-stu-id="28e97-197">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![результаты теста отклика проверки](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="28e97-199">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="28e97-199">Renewing a subscription</span></span>

<span data-ttu-id="28e97-200">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="28e97-200">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="28e97-201">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="28e97-201">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="28e97-202">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="28e97-202">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="28e97-203">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28e97-203">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="28e97-204">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="28e97-204">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="28e97-205">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="28e97-205">Deleting a subscription</span></span>

<span data-ttu-id="28e97-206">Клиент может прекратить получать уведомления об изменениях, удалив подписку с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="28e97-206">The client can stop receiving change notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="28e97-207">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="28e97-207">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="28e97-208">Уведомления об изменениях</span><span class="sxs-lookup"><span data-stu-id="28e97-208">Change notifications</span></span>

<span data-ttu-id="28e97-209">Если клиент выполняет подписку на изменения ресурса, Microsoft Graph отправляет `POST` запрос на URL-адрес уведомлений при каждом изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="28e97-209">With a client subscribing to changes to a resource, Microsoft Graph sends a `POST` request to the notification URL whenever the resource changes.</span></span> <span data-ttu-id="28e97-210">Он отправляет уведомления только для тех изменений типа, которые указаны в подписке, например `created` .</span><span class="sxs-lookup"><span data-stu-id="28e97-210">It sends notifications only for changes of the type that's specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="28e97-211">**Примечание:** Если клиент имеет несколько подписок, контролирующих один и тот же URL-адрес уведомления, Microsoft Graph может отправлять несколько уведомлений об изменениях, соответствующих разным подпискам, каждый из которых отображает соответствующий идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="28e97-211">**Note:** If a client has multiple subscriptions that monitor the same resource and use the same notification URL, Microsoft Graph can send multiple change notifications that correspond to different subscriptions, each showing the corresponding subscription ID.</span></span> <span data-ttu-id="28e97-212">Нет гарантии, что все уведомления об изменениях в `POST` запросе принадлежат одной подписке.</span><span class="sxs-lookup"><span data-stu-id="28e97-212">There is no guarantee that all change notifications in the `POST` request belong to a single subscription.</span></span>

### <a name="change-notification-example"></a><span data-ttu-id="28e97-213">Пример уведомления об изменении</span><span class="sxs-lookup"><span data-stu-id="28e97-213">Change notification example</span></span>

<span data-ttu-id="28e97-214">В этом разделе представлен пример уведомления для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="28e97-214">This section shows an example of a notification for a message creation.</span></span> <span data-ttu-id="28e97-215">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомление об изменении, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="28e97-215">When the user receives an email, Microsoft Graph sends a change notification as shown in the following example.</span></span>
<span data-ttu-id="28e97-216">Обратите внимание, что уведомление представлено в коллекции, представленной в `value` поле.</span><span class="sxs-lookup"><span data-stu-id="28e97-216">Note that the notification is in a collection represented in the `value` field.</span></span> <span data-ttu-id="28e97-217">Сведения о полезных данных уведомления можно найти в [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection) .</span><span class="sxs-lookup"><span data-stu-id="28e97-217">See [changeNotificationCollection](/graph/api/resources/changenotificationcollection) for details of the notification payload.</span></span> 

<span data-ttu-id="28e97-218">При возникновении большого количества изменений Microsoft Graph может отправлять несколько уведомлений, соответствующих разным подпискам в одном `POST` запросе.</span><span class="sxs-lookup"><span data-stu-id="28e97-218">When many changes occur, Microsoft Graph may send multiple notifications that correspond to different subscriptions in the same `POST` request.</span></span>

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
      "sequenceNumber": 10,
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

### <a name="processing-the-change-notification"></a><span data-ttu-id="28e97-219">Обработка уведомления об изменении</span><span class="sxs-lookup"><span data-stu-id="28e97-219">Processing the change notification</span></span>

<span data-ttu-id="28e97-220">Процесс должен обрабатывать каждое уведомление об изменении, которое он получает.</span><span class="sxs-lookup"><span data-stu-id="28e97-220">Your process should process every change notification it receives.</span></span> <span data-ttu-id="28e97-221">Ниже приведены минимальные задачи, которые приложение должно выполнить для обработки уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="28e97-221">The following are the minimum tasks that your app must perform to process a change notification:</span></span>

1. <span data-ttu-id="28e97-222">Отправьте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e97-222">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="28e97-223">Если Microsoft Graph не получает код класса 2xx, он попытается опубликовать уведомление об изменении несколько раз в течение 4 часов; После этого уведомление об изменении будет удалено и не будет доставлено.</span><span class="sxs-lookup"><span data-stu-id="28e97-223">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the change notification a number of times, for a period of about 4 hours; after that, the change notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="28e97-224">**Примечание:** Отправьте код состояния сразу же после `202 - Accepted` получения уведомления об изменении, даже перед проверкой его подлинности.</span><span class="sxs-lookup"><span data-stu-id="28e97-224">**Note:** Send a `202 - Accepted` status code as soon as you receive the change notification, even before validating its authenticity.</span></span> <span data-ttu-id="28e97-225">Вы просто подтверждаете получение уведомления об изменении и предотвратите ненужные попытки.</span><span class="sxs-lookup"><span data-stu-id="28e97-225">You are simply acknowledging the receipt of the change notification and preventing unnecessary retries.</span></span> <span data-ttu-id="28e97-226">Текущее значение времени ожидания — 30 секунд, но это время может быть сокращено в будущем для оптимизации производительности службы.</span><span class="sxs-lookup"><span data-stu-id="28e97-226">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span> <span data-ttu-id="28e97-227">Если URL-адрес уведомления не отвечает в течение 30 секунд для более чем 10% запросов от Microsoft Graph за 10 минут, все следующие уведомления будут задержаны и повторены в течение 4 часов.</span><span class="sxs-lookup"><span data-stu-id="28e97-227">If the notification URL doesn't reply within 30 seconds for more than 10% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be delayed and retried for a period of 4 hours.</span></span> <span data-ttu-id="28e97-228">Если URL-адрес уведомления не отвечает в течение 30 секунд за более 20% запросов от Microsoft Graph за 10 минут, будут удалены все следующие уведомления.</span><span class="sxs-lookup"><span data-stu-id="28e97-228">If a notification URL doesn't reply within 30 seconds for more than 20% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be dropped.</span></span>

1. <span data-ttu-id="28e97-229">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="28e97-229">Validate the `clientState` property.</span></span> <span data-ttu-id="28e97-230">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="28e97-230">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="28e97-231">**Примечание:** Если это не так, вы не должны считать это действительное уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="28e97-231">**Note:** If this isn't true, you should not consider this a valid change notification.</span></span> <span data-ttu-id="28e97-232">Возможно, что уведомление об изменении не получено из Microsoft Graph и может быть отправлено фальшивым субъектом.</span><span class="sxs-lookup"><span data-stu-id="28e97-232">It is possible that the change notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="28e97-233">Кроме того, следует проверить, откуда поступило уведомление об изменении, и предпринять соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="28e97-233">You should also investigate where the change notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="28e97-234">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="28e97-234">Update your application based on your business logic.</span></span>

<span data-ttu-id="28e97-235">Повторите эти действия для других уведомлений об изменении в запросе.</span><span class="sxs-lookup"><span data-stu-id="28e97-235">Repeat for other change notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="28e97-236">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="28e97-236">Code samples</span></span>

<span data-ttu-id="28e97-237">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="28e97-237">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="28e97-238">Обучающий модуль по Microsoft Graph: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="28e97-238">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="28e97-239">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="28e97-239">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [<span data-ttu-id="28e97-240">Пример веб-перехватчиков Microsoft Graph для ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="28e97-240">Microsoft Graph Webhooks Sample for ASP.NET Core</span></span>](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [<span data-ttu-id="28e97-241">Пример веб-перехватчиков Microsoft Graph для Java Spring</span><span class="sxs-lookup"><span data-stu-id="28e97-241">Microsoft Graph Webhooks Sample for Java Spring</span></span>](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a><span data-ttu-id="28e97-242">Конфигурация брандмауэра</span><span class="sxs-lookup"><span data-stu-id="28e97-242">Firewall configuration</span></span>

<span data-ttu-id="28e97-243">При необходимости можно настроить брандмауэр, защищающий URL-адрес уведомлений, чтобы разрешить входящие подключения только из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e97-243">You can optionally configure the firewall that protects your notification URL to allow inbound connections only from Microsoft Graph.</span></span> <span data-ttu-id="28e97-244">Это позволяет уменьшить риск недопустимых уведомлений об изменениях, отправляемых на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="28e97-244">This allows you to reduce further exposure to invalid change notifications that are sent to your notification URL.</span></span> <span data-ttu-id="28e97-245">Эти недопустимые уведомления об изменении могут пытаться активировать реализованную пользовательскую логику.</span><span class="sxs-lookup"><span data-stu-id="28e97-245">These invalid change notifications can be trying to trigger the custom logic that you implemented.</span></span> <span data-ttu-id="28e97-246">Полный список IP-адресов, используемых Microsoft Graph для доставки уведомлений об изменениях, приведен в разделе [дополнительные конечные точки для microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span><span class="sxs-lookup"><span data-stu-id="28e97-246">For a complete list of IP addresses used by Microsoft Graph to deliver change notifications, see [additional endpoints for Microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span></span>

> <span data-ttu-id="28e97-247">**Примечание:** Указанные IP-адреса, используемые для доставки уведомлений об изменениях, можно обновить в любое время без уведомления.</span><span class="sxs-lookup"><span data-stu-id="28e97-247">**Note:** The listed IP addresses that are used to deliver change notifications can be updated at any time without notice.</span></span>

## <a name="see-also"></a><span data-ttu-id="28e97-248">См. также</span><span class="sxs-lookup"><span data-stu-id="28e97-248">See also</span></span>

- [<span data-ttu-id="28e97-249">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="28e97-249">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="28e97-250">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="28e97-250">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="28e97-251">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="28e97-251">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- <span data-ttu-id="28e97-252">Тип ресурса [чанженотификатион](/graph/api/resources/changenotification?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="28e97-252">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) resource type</span></span>
- <span data-ttu-id="28e97-253">Тип ресурса [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="28e97-253">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) resource type</span></span>
- [<span data-ttu-id="28e97-254">Руководство по изменениям уведомлений и отслеживания изменений</span><span class="sxs-lookup"><span data-stu-id="28e97-254">Change notifications and change tracking tutorial</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)
- [<span data-ttu-id="28e97-255">Уведомления в жизненном цикле (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="28e97-255">Lifecycle notifications (preview)</span></span>](/graph/concepts/webhooks-outlook-authz.md)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
