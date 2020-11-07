---
title: Настройка уведомлений об изменениях в пользовательских данных
description: API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях для клиентов. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений об изменениях. С помощью этих уведомлений клиентские приложения обновляют свое состояние в случае изменений.
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 9fa210486c924fc3e29e9d3f2ddfee5422a937f9
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932593"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="3340c-105">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="3340c-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="3340c-p102">API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях для клиентов. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений об изменениях. С помощью этих уведомлений клиентские приложения обновляют свое состояние в случае изменений.</span><span class="sxs-lookup"><span data-stu-id="3340c-p102">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.</span></span>

<span data-ttu-id="3340c-p103">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates its cache and views, and so on.</span><span class="sxs-lookup"><span data-stu-id="3340c-p103">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="3340c-112">Руководство. Использование уведомлений об изменениях и функции отслеживания изменений в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3340c-112">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

<span data-ttu-id="3340c-p104">By default, change notifications do not contain resource data, other than the `id`. If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource. This article uses the **user** resource as an example for working with change notifications.</span><span class="sxs-lookup"><span data-stu-id="3340c-p104">By default, change notifications do not contain resource data, other than the `id`. If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource. This article uses the **user** resource as an example for working with change notifications.</span></span>

<span data-ttu-id="3340c-p105">An app can also subscribe to change notifications that include resource data, to avoid having to make additional API calls to access the data. Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data. For details about how to work with these notifications, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="3340c-p105">An app can also subscribe to change notifications that include resource data, to avoid having to make additional API calls to access the data. Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data. For details about how to work with these notifications, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="3340c-119">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="3340c-119">Supported resources</span></span>

<span data-ttu-id="3340c-120">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="3340c-120">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="3340c-121">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="3340c-121">Outlook [message][]</span></span>
- <span data-ttu-id="3340c-122">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="3340c-122">Outlook [event][]</span></span>
- <span data-ttu-id="3340c-123">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="3340c-123">Outlook personal [contact][]</span></span>
- <span data-ttu-id="3340c-124">[list][]</span><span class="sxs-lookup"><span data-stu-id="3340c-124">[list][]</span></span>
- <span data-ttu-id="3340c-125">[user][]</span><span class="sxs-lookup"><span data-stu-id="3340c-125">[user][]</span></span>
- <span data-ttu-id="3340c-126">[group][]</span><span class="sxs-lookup"><span data-stu-id="3340c-126">[group][]</span></span>
- <span data-ttu-id="3340c-127">Групповой [чат][] Microsoft 365 </span><span class="sxs-lookup"><span data-stu-id="3340c-127">Microsoft 365 group [conversation][]</span></span>
- <span data-ttu-id="3340c-128">Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="3340c-128">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="3340c-129">Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="3340c-129">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="3340c-130">[Оповещение][] безопасности</span><span class="sxs-lookup"><span data-stu-id="3340c-130">Security [alert][]</span></span>
- <span data-ttu-id="3340c-131">[callRecord][] в Teams</span><span class="sxs-lookup"><span data-stu-id="3340c-131">Teams [callRecord][]</span></span>
- <span data-ttu-id="3340c-132">[chatMessage][] Teams</span><span class="sxs-lookup"><span data-stu-id="3340c-132">Teams [chatMessage][]</span></span>
- <span data-ttu-id="3340c-133">Teams [presence][] (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3340c-133">Teams [presence][] (preview)</span></span>
- <span data-ttu-id="3340c-134">[printTaskDefinition][] печати</span><span class="sxs-lookup"><span data-stu-id="3340c-134">Print [printTaskDefinition][]</span></span>

<span data-ttu-id="3340c-135">Вы можете создать подписку на определенную папку Outlook, например, папку Входящие: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="3340c-135">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="3340c-136">либо на ресурс верхнего уровня: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="3340c-136">Or to a top-level resource: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, `/communications/callRecords`</span></span>

<span data-ttu-id="3340c-137">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`, `sites/{site-id}/lists/{list-id}`, `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="3340c-137">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`, `sites/{site-id}/lists/{list-id}`, `/communications/presences/{id}`</span></span>

<span data-ttu-id="3340c-138">либо на личное хранилище OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="3340c-138">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="3340c-139">либо на корневую папку диска SharePoint/OneDrive для бизнеса: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="3340c-139">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="3340c-140">либо на новое оповещение [API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="3340c-140">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="3340c-141">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="3340c-141">Azure AD resource limitations</span></span>

<span data-ttu-id="3340c-142">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения возникают ошибки.</span><span class="sxs-lookup"><span data-stu-id="3340c-142">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="3340c-143">**Примечание**. Эти ограничения не применяются к ресурсам служб, не относящихся к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3340c-143">**Note** : These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="3340c-144">Например, приложение может создать больше дополнительных подписок на ресурсы `message` или `event`, поддерживаемые службой Exchange Online в составе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3340c-144">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="3340c-145">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="3340c-145">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="3340c-146">На приложение (для сочетания всех клиентов): 50 000 подписок всего</span><span class="sxs-lookup"><span data-stu-id="3340c-146">Per app (for all tenants combined): 50,000 total subscriptions</span></span>
  - <span data-ttu-id="3340c-147">На клиента (для сочетания всех приложений): 1000 подписок всего во всех приложениях</span><span class="sxs-lookup"><span data-stu-id="3340c-147">Per tenant (for all applications combined): 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="3340c-148">На сочетание приложения и клиента: 100 подписок всего</span><span class="sxs-lookup"><span data-stu-id="3340c-148">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="3340c-149">Если какое-либо ограничение превышено, попытки создать подписку приведут к [ответу с ошибкой](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="3340c-149">When any limit is exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="3340c-150">Свойство `message` указывает, какое ограничение превышено.</span><span class="sxs-lookup"><span data-stu-id="3340c-150">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="3340c-151">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="3340c-151">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="3340c-152">Уведомления об изменениях для сущностей пользователей не поддерживаются для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3340c-152">Change notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="3340c-153">В подписках пользователей и групп существует [известная проблема](known-issues.md#change-notifications).</span><span class="sxs-lookup"><span data-stu-id="3340c-153">A [known issue](known-issues.md#change-notifications) exists with user and group subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="3340c-154">Ограничения ресурсов Outlook</span><span class="sxs-lookup"><span data-stu-id="3340c-154">Outlook resource limitations</span></span>

<span data-ttu-id="3340c-155">Если вы используете *имя участника-пользователя* на пути к ресурсу при оформлении подписки на ресурсы Outlook, например **сообщения** , **события** или **контакты** , запрос на подписку может быть не выполнен, если это имя содержит апостроф. </span><span class="sxs-lookup"><span data-stu-id="3340c-155">When subscribing to Outlook resources such as **messages** , **events** or **contacts** , if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="3340c-156">Используйте ИД GUID пользователей вместо имен участников-пользователей, чтобы избежать этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="3340c-156">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="3340c-157">Например, вместо пути к ресурсу:</span><span class="sxs-lookup"><span data-stu-id="3340c-157">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="3340c-158">Используйте:</span><span class="sxs-lookup"><span data-stu-id="3340c-158">Use:</span></span> 

`/users/{guid-user-id}/messages`

### <a name="teams-resource-limitations"></a><span data-ttu-id="3340c-159">Ограничения ресурсов Teams</span><span class="sxs-lookup"><span data-stu-id="3340c-159">Teams resource limitations</span></span>

<span data-ttu-id="3340c-160">Каждый ресурс Teams имеет различные квоты подписки.</span><span class="sxs-lookup"><span data-stu-id="3340c-160">Each Teams resource has different subscription quotas.</span></span>

- <span data-ttu-id="3340c-161">Для подписок на **callRecords** :</span><span class="sxs-lookup"><span data-stu-id="3340c-161">For subscriptions to **callRecords** :</span></span>
  - <span data-ttu-id="3340c-162">На организацию: всего 100 подписок</span><span class="sxs-lookup"><span data-stu-id="3340c-162">Per organization: 100 total subscriptions</span></span>

- <span data-ttu-id="3340c-163">Для подписок на **chatMessages** (каналы или чаты):</span><span class="sxs-lookup"><span data-stu-id="3340c-163">For subscriptions to **chatMessages** (channels or chats):</span></span>
  - <span data-ttu-id="3340c-164">На сочетание приложения и канала или чата: 1 подписка</span><span class="sxs-lookup"><span data-stu-id="3340c-164">Per app and channel or chat combination: 1 subscription</span></span>
  - <span data-ttu-id="3340c-165">На организацию: всего 10 000 подписок</span><span class="sxs-lookup"><span data-stu-id="3340c-165">Per organization: 10,000 total subscriptions</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="3340c-166">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="3340c-166">Subscription lifetime</span></span>

<span data-ttu-id="3340c-167">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="3340c-167">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="3340c-168">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="3340c-168">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="3340c-169">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="3340c-169">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="3340c-170">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="3340c-170">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="3340c-171">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="3340c-171">Apps can also unsubscribe at any time to stop getting change notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="3340c-172">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="3340c-172">Managing subscriptions</span></span>

<span data-ttu-id="3340c-173">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="3340c-173">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="3340c-174">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="3340c-174">Creating a subscription</span></span>

<span data-ttu-id="3340c-175">Чтобы начать получать уведомления об изменениях для ресурса, сначала необходимо создать подписку.</span><span class="sxs-lookup"><span data-stu-id="3340c-175">Creating a subscription is the first step to start receiving change notifications for a resource.</span></span> <span data-ttu-id="3340c-176">Процесс подписки выполняется указанным ниже образом.</span><span class="sxs-lookup"><span data-stu-id="3340c-176">The subscription process is as follows:</span></span>

1. <span data-ttu-id="3340c-177">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="3340c-177">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="3340c-178">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="3340c-178">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="3340c-179">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="3340c-179">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="3340c-180">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3340c-180">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="3340c-181">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3340c-181">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="3340c-182">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3340c-182">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="3340c-183">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления об изменениях с подписками.</span><span class="sxs-lookup"><span data-stu-id="3340c-183">The client must store the subscription ID to correlate change notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="3340c-184">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="3340c-184">Subscription request example</span></span>

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

<span data-ttu-id="3340c-185">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="3340c-185">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="3340c-186">Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="3340c-186">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="3340c-187">Свойство `resource` указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="3340c-187">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="3340c-188">Например, вы можете создать подписку на определенную почтовую папку: `me/mailFolders('inbox')/messages` или сделать это от имени пользователя с согласия администратора: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="3340c-188">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="3340c-189">Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="3340c-189">Although `clientState` is not required, you must include it to comply with our recommended change notification handling process.</span></span> <span data-ttu-id="3340c-190">Задание этого свойства позволит подтверждать, что полученные уведомления об изменениях поступают от службы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3340c-190">Setting this property will allow you to confirm that change notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="3340c-191">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3340c-191">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="3340c-192">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3340c-192">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

> <span data-ttu-id="3340c-193">**Примечание.** Любой параметр строки запроса, включенный в свойство **notificationUrl** , будет включен в HTTP-запрос POST при доставке уведомлений.</span><span class="sxs-lookup"><span data-stu-id="3340c-193">**Note:** Any query string parameter included in the **notificationUrl** property will be included in the HTTP POST request when notifications are being delivered.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="3340c-194">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="3340c-194">Notification endpoint validation</span></span>

<span data-ttu-id="3340c-195">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="3340c-195">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="3340c-196">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="3340c-196">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="3340c-197">Microsoft Graph кодирует маркер проверки и включает его в запрос POST URL-адреса уведомления:</span><span class="sxs-lookup"><span data-stu-id="3340c-197">Microsoft Graph encodes a validation token and includes it in a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

1. <span data-ttu-id="3340c-198">Клиенту необходимо правильно расшифровать URL-адрес параметра запроса`validationToken`, предоставленный на предыдущем этапе, и избегать любого HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="3340c-198">The client must properly URL decode the `validationToken` query parameter provided in the preceding step, and escape any HTML/JavaScript.</span></span>

   <span data-ttu-id="3340c-199">Рекомендуется их избегать, поскольку злоумышленники могут использовать конечную точку уведомления для атаки типа межсайтовых сценариев.</span><span class="sxs-lookup"><span data-stu-id="3340c-199">Escaping is a good practice because malicious actors can use the notification endpoint for cross-site scripting type of attacks.</span></span>

   <span data-ttu-id="3340c-200">Как правило, значение маркера проверки рассматривается как непрозрачное, так как формат маркера обычно меняется без уведомлений.</span><span class="sxs-lookup"><span data-stu-id="3340c-200">In general, treat the validation token value as opaque, as the token format can generally change without notice.</span></span> <span data-ttu-id="3340c-201">Microsoft Graph никогда не отправляет значения, содержащие код HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="3340c-201">Microsoft Graph never sends any value containing HTML or JavaScript code.</span></span>

1. <span data-ttu-id="3340c-202">В течение 10 секунд первого этапа клиент должен предоставить ответ со следующими характеристиками:</span><span class="sxs-lookup"><span data-stu-id="3340c-202">The client must provide a response with the following characteristics within 10 seconds of step 1:</span></span>

    - <span data-ttu-id="3340c-203">Код состояния `HTTP 200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3340c-203">A status code of `HTTP 200 OK`.</span></span>
    - <span data-ttu-id="3340c-204">Тип контента `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="3340c-204">A content type of `text/plain`.</span></span>
    - <span data-ttu-id="3340c-205">Основной текст, включающий маркер проверки с _расшифрованным URL-адресом_.</span><span class="sxs-lookup"><span data-stu-id="3340c-205">A body that includes the _URL decoded_ validation token.</span></span> <span data-ttu-id="3340c-206">Просто отобразите ту же строку, которая была отправлена в параметре запроса `validationToken`.</span><span class="sxs-lookup"><span data-stu-id="3340c-206">Simply reflect back the same string that was sent in the `validationToken` query parameter.</span></span>

    <span data-ttu-id="3340c-207">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="3340c-207">The client should discard the validation token after providing it in the response.</span></span>

    > <span data-ttu-id="3340c-208">**Важно!** Если клиент возвращает зашифрованный маркер проверки, проверка завершится ошибкой.</span><span class="sxs-lookup"><span data-stu-id="3340c-208">**Important:** If the client returns an encoded validation token, the validation will fail.</span></span>

<span data-ttu-id="3340c-209">Кроме того, можно использовать [коллекцию Microsoft Graph Postman](use-postman.md), чтобы убедиться в правильности реализации запроса проверки в вашей конечной точке.</span><span class="sxs-lookup"><span data-stu-id="3340c-209">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="3340c-210">Запрос **Проверка подписки** в папке **Прочее** предоставляет модульные тесты, проверяющие отклик вашей конечной точки.</span><span class="sxs-lookup"><span data-stu-id="3340c-210">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![результаты теста отклика проверки](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="3340c-212">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="3340c-212">Renewing a subscription</span></span>

<span data-ttu-id="3340c-213">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="3340c-213">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="3340c-214">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="3340c-214">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="3340c-215">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="3340c-215">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="3340c-216">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3340c-216">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="3340c-217">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="3340c-217">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="3340c-218">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="3340c-218">Deleting a subscription</span></span>

<span data-ttu-id="3340c-219">Клиент может прекратить получать уведомления об изменениях, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="3340c-219">The client can stop receiving change notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="3340c-220">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3340c-220">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="3340c-221">Уведомления об изменениях</span><span class="sxs-lookup"><span data-stu-id="3340c-221">Change notifications</span></span>

<span data-ttu-id="3340c-222">Когда клиент подписывается на изменения ресурса, Microsoft Graph отправляет запрос `POST` в URL-адрес уведомления при каждом изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="3340c-222">With a client subscribing to changes to a resource, Microsoft Graph sends a `POST` request to the notification URL whenever the resource changes.</span></span> <span data-ttu-id="3340c-223">Уведомления отправляются только при изменениях типа, указанного в подписке, например, `created`.</span><span class="sxs-lookup"><span data-stu-id="3340c-223">It sends notifications only for changes of the type that's specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="3340c-224">**Примечание.** Если клиент имеет несколько подписок, которые контролируют один ресурс и используют один URL-адрес уведомлений, Microsoft Graph может отправлять несколько уведомлений об изменениях, соответствующих разным подпискам, каждое из которых показывает идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="3340c-224">**Note:** If a client has multiple subscriptions that monitor the same resource and use the same notification URL, Microsoft Graph can send multiple change notifications that correspond to different subscriptions, each showing the corresponding subscription ID.</span></span> <span data-ttu-id="3340c-225">Уведомления об изменениях из сообщения `POST` могут принадлежать разным подпискам.</span><span class="sxs-lookup"><span data-stu-id="3340c-225">There is no guarantee that all change notifications in the `POST` request belong to a single subscription.</span></span>

### <a name="change-notification-example"></a><span data-ttu-id="3340c-226">Пример уведомления об изменениях</span><span class="sxs-lookup"><span data-stu-id="3340c-226">Change notification example</span></span>

<span data-ttu-id="3340c-227">В этом разделе указан пример уведомления для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="3340c-227">This section shows an example of a notification for a message creation.</span></span> <span data-ttu-id="3340c-228">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления об изменениях, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="3340c-228">When the user receives an email, Microsoft Graph sends a change notification as shown in the following example.</span></span>
<span data-ttu-id="3340c-229">Обратите внимание на то, что уведомление является коллекцией, представленной в поле "`value`".</span><span class="sxs-lookup"><span data-stu-id="3340c-229">Note that the notification is in a collection represented in the `value` field.</span></span> <span data-ttu-id="3340c-230">Дополнительные сведения о полезных данных уведомлений см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection)</span><span class="sxs-lookup"><span data-stu-id="3340c-230">See [changeNotificationCollection](/graph/api/resources/changenotificationcollection) for details of the notification payload.</span></span> 

<span data-ttu-id="3340c-231">При многочисленных изменениях Microsoft Graph может отправлять несколько уведомлений, соответствующих разным подпискам, в одном и том же запросе `POST`.</span><span class="sxs-lookup"><span data-stu-id="3340c-231">When many changes occur, Microsoft Graph may send multiple notifications that correspond to different subscriptions in the same `POST` request.</span></span>

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

### <a name="processing-the-change-notification"></a><span data-ttu-id="3340c-232">Обработка уведомлений об изменениях</span><span class="sxs-lookup"><span data-stu-id="3340c-232">Processing the change notification</span></span>

<span data-ttu-id="3340c-233">Процесс должен обрабатывать каждое уведомление об изменениях.</span><span class="sxs-lookup"><span data-stu-id="3340c-233">Your process should process every change notification it receives.</span></span> <span data-ttu-id="3340c-234">Ниже перечислены основные задачи, которые приложение должно выполнить для обработки таких уведомлений.</span><span class="sxs-lookup"><span data-stu-id="3340c-234">The following are the minimum tasks that your app must perform to process a change notification:</span></span>

1. <span data-ttu-id="3340c-235">Отправьте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3340c-235">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="3340c-236">Если 2хх код не будет получен, Microsoft Graph попытается опубликовать уведомление об изменении несколько раз в течение 4 часов. После этого это уведомление будет удалено.</span><span class="sxs-lookup"><span data-stu-id="3340c-236">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the change notification a number of times, for a period of about 4 hours; after that, the change notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="3340c-237">**Примечание.** Отправьте код состояния `202 - Accepted` сразу после получения уведомления об изменениях, еще перед проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="3340c-237">**Note:** Send a `202 - Accepted` status code as soon as you receive the change notification, even before validating its authenticity.</span></span> <span data-ttu-id="3340c-238">Просто подтвердите получение уведомления об изменениях, чтобы избежать ненужных повторных попыток.</span><span class="sxs-lookup"><span data-stu-id="3340c-238">You are simply acknowledging the receipt of the change notification and preventing unnecessary retries.</span></span> <span data-ttu-id="3340c-239">Текущее значение времени ожидания — 30 секунд, но это время может быть сокращено в будущем для оптимизации производительности службы.</span><span class="sxs-lookup"><span data-stu-id="3340c-239">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span> <span data-ttu-id="3340c-240">Если URL-адрес уведомления не отвечает в течение 30 секунд на более чем 10% запросов от Microsoft Graph за 10 минут, все уведомления ниже будут отложены и повторено выполнены в течение 4 часов.</span><span class="sxs-lookup"><span data-stu-id="3340c-240">If the notification URL doesn't reply within 30 seconds for more than 10% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be delayed and retried for a period of 4 hours.</span></span> <span data-ttu-id="3340c-241">Если URL-адрес уведомления не отвечает в течение 30 секунд на более чем 20% запросов от Microsoft Graph за 10 минут, все уведомления ниже будут удалены.</span><span class="sxs-lookup"><span data-stu-id="3340c-241">If a notification URL doesn't reply within 30 seconds for more than 20% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be dropped.</span></span>

1. <span data-ttu-id="3340c-242">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="3340c-242">Validate the `clientState` property.</span></span> <span data-ttu-id="3340c-243">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="3340c-243">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="3340c-244">**Примечание.** Если это не так, уведомление об изменениях не следует рассматривать как действительное.</span><span class="sxs-lookup"><span data-stu-id="3340c-244">**Note:** If this isn't true, you should not consider this a valid change notification.</span></span> <span data-ttu-id="3340c-245">Возможно оно создано не Microsoft Graph и отправлено незаконным субъектом.</span><span class="sxs-lookup"><span data-stu-id="3340c-245">It is possible that the change notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="3340c-246">Вы также можете определить, откуда поступило уведомление об изменениях, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="3340c-246">You should also investigate where the change notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="3340c-247">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="3340c-247">Update your application based on your business logic.</span></span>

<span data-ttu-id="3340c-248">Повторяйте эти действия для других уведомлений об изменениях в запросе.</span><span class="sxs-lookup"><span data-stu-id="3340c-248">Repeat for other change notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="3340c-249">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="3340c-249">Code samples</span></span>

<span data-ttu-id="3340c-250">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="3340c-250">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="3340c-251">Обучающий модуль по Microsoft Graph: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3340c-251">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="3340c-252">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="3340c-252">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [<span data-ttu-id="3340c-253">Пример веб-перехватчиков Microsoft Graph для ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="3340c-253">Microsoft Graph Webhooks Sample for ASP.NET Core</span></span>](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [<span data-ttu-id="3340c-254">Пример веб-перехватчиков Microsoft Graph для Java Spring</span><span class="sxs-lookup"><span data-stu-id="3340c-254">Microsoft Graph Webhooks Sample for Java Spring</span></span>](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a><span data-ttu-id="3340c-255">Конфигурация брандмауэра</span><span class="sxs-lookup"><span data-stu-id="3340c-255">Firewall configuration</span></span>

<span data-ttu-id="3340c-256">При необходимости можно настроить брандмауэр, который защищает URL-адрес уведомления, чтобы разрешить входящие подключения только из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3340c-256">You can optionally configure the firewall that protects your notification URL to allow inbound connections only from Microsoft Graph.</span></span> <span data-ttu-id="3340c-257">Это позволит снизить дополнительное воздействие недопустимых уведомлений об изменениях, которые отправляются на URL-адрес уведомления.</span><span class="sxs-lookup"><span data-stu-id="3340c-257">This allows you to reduce further exposure to invalid change notifications that are sent to your notification URL.</span></span> <span data-ttu-id="3340c-258">Такие недействительные уведомления об изменениях могут пытаться активировать реализуемую вами пользовательскую логику.</span><span class="sxs-lookup"><span data-stu-id="3340c-258">These invalid change notifications can be trying to trigger the custom logic that you implemented.</span></span> <span data-ttu-id="3340c-259">Полный список IP-адресов, которые используются Microsoft Graph для доставки уведомлений об изменениях, см в сведениях о[дополнительных конечных точках для Microsoft 365](/office365/enterprise/additional-office365-ip-addresses-and-urls).</span><span class="sxs-lookup"><span data-stu-id="3340c-259">For a complete list of IP addresses used by Microsoft Graph to deliver change notifications, see [additional endpoints for Microsoft 365](/office365/enterprise/additional-office365-ip-addresses-and-urls).</span></span>

> <span data-ttu-id="3340c-260">**Примечание.** Указанные IP-адреса, которые используются для доставки уведомлений об изменениях, можно обновлять в любой момент без предварительных примечаний.</span><span class="sxs-lookup"><span data-stu-id="3340c-260">**Note:** The listed IP addresses that are used to deliver change notifications can be updated at any time without notice.</span></span>

## <a name="latency"></a><span data-ttu-id="3340c-261">Задержка</span><span class="sxs-lookup"><span data-stu-id="3340c-261">Latency</span></span>

<span data-ttu-id="3340c-262">В следующей таблице указаны ожидаемые задержки между возникновением события в службе и доставкой уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="3340c-262">The following table lists the latency to expect between an event happening in the service and the delivery of the change notification.</span></span>

| <span data-ttu-id="3340c-263">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3340c-263">Resource</span></span> | <span data-ttu-id="3340c-264">Средняя задержка</span><span class="sxs-lookup"><span data-stu-id="3340c-264">Average latency</span></span> | <span data-ttu-id="3340c-265">Максимальная задержка</span><span class="sxs-lookup"><span data-stu-id="3340c-265">Maximum latency</span></span> |
|:-----|:-----|:-----|
|<span data-ttu-id="3340c-266">[callRecord][]</span><span class="sxs-lookup"><span data-stu-id="3340c-266">[callRecord][]</span></span> | <span data-ttu-id="3340c-267">Менее 15 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-267">Less than 15 minutes</span></span> | <span data-ttu-id="3340c-268">60 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-268">60 minutes</span></span> |
|<span data-ttu-id="3340c-269">[chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="3340c-269">[chatMessage][]</span></span> | <span data-ttu-id="3340c-270">Менее 10 секунд</span><span class="sxs-lookup"><span data-stu-id="3340c-270">Less than 10 seconds</span></span> | <span data-ttu-id="3340c-271">1 минута</span><span class="sxs-lookup"><span data-stu-id="3340c-271">1 minute</span></span> |
|<span data-ttu-id="3340c-272">[contact][]</span><span class="sxs-lookup"><span data-stu-id="3340c-272">[contact][]</span></span> | <span data-ttu-id="3340c-273">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="3340c-273">Unknown</span></span> | <span data-ttu-id="3340c-274">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="3340c-274">Unknown</span></span> |
|<span data-ttu-id="3340c-275">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="3340c-275">[driveItem][]</span></span> | <span data-ttu-id="3340c-276">Менее 1 минуты</span><span class="sxs-lookup"><span data-stu-id="3340c-276">Less than 1 minute</span></span> | <span data-ttu-id="3340c-277">5 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-277">5 minutes</span></span> |
|<span data-ttu-id="3340c-278">[event][]</span><span class="sxs-lookup"><span data-stu-id="3340c-278">[event][]</span></span> | <span data-ttu-id="3340c-279">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="3340c-279">Unknown</span></span> | <span data-ttu-id="3340c-280">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="3340c-280">Unknown</span></span> |
|<span data-ttu-id="3340c-281">[group][]</span><span class="sxs-lookup"><span data-stu-id="3340c-281">[group][]</span></span> | <span data-ttu-id="3340c-282">Менее 2 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-282">Less than 2 minutes</span></span> | <span data-ttu-id="3340c-283">15 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-283">15 minutes</span></span> |
|<span data-ttu-id="3340c-284">[conversation][]</span><span class="sxs-lookup"><span data-stu-id="3340c-284">[conversation][]</span></span> | <span data-ttu-id="3340c-285">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="3340c-285">Unknown</span></span> | <span data-ttu-id="3340c-286">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="3340c-286">Unknown</span></span> |
|<span data-ttu-id="3340c-287">[list][]</span><span class="sxs-lookup"><span data-stu-id="3340c-287">[list][]</span></span> | <span data-ttu-id="3340c-288">Менее 1 минуты</span><span class="sxs-lookup"><span data-stu-id="3340c-288">Less than 1 minute</span></span> | <span data-ttu-id="3340c-289">5 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-289">5 minutes</span></span> |
|<span data-ttu-id="3340c-290">[message][]</span><span class="sxs-lookup"><span data-stu-id="3340c-290">[message][]</span></span> | <span data-ttu-id="3340c-291">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="3340c-291">Unknown</span></span> | <span data-ttu-id="3340c-292">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="3340c-292">Unknown</span></span> |
|<span data-ttu-id="3340c-293">[alert][]</span><span class="sxs-lookup"><span data-stu-id="3340c-293">[alert][]</span></span> | <span data-ttu-id="3340c-294">Менее 3 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-294">Less than 3 minutes</span></span> | <span data-ttu-id="3340c-295">5 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-295">5 minutes</span></span> |
|<span data-ttu-id="3340c-296">[presence][] (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3340c-296">[presence][] (preview)</span></span> | <span data-ttu-id="3340c-297">Менее 10 секунд</span><span class="sxs-lookup"><span data-stu-id="3340c-297">Less than 10 seconds</span></span> | <span data-ttu-id="3340c-298">1 минута</span><span class="sxs-lookup"><span data-stu-id="3340c-298">1 minute</span></span> |
|<span data-ttu-id="3340c-299">[printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="3340c-299">[printTaskDefinition][]</span></span> | <span data-ttu-id="3340c-300">Менее 1 минуты</span><span class="sxs-lookup"><span data-stu-id="3340c-300">Less than 1 minute</span></span> | <span data-ttu-id="3340c-301">5 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-301">5 minutes</span></span> |
|<span data-ttu-id="3340c-302">[user][]</span><span class="sxs-lookup"><span data-stu-id="3340c-302">[user][]</span></span> | <span data-ttu-id="3340c-303">Менее 2 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-303">Less than 2 minutes</span></span> | <span data-ttu-id="3340c-304">15 минут</span><span class="sxs-lookup"><span data-stu-id="3340c-304">15 minutes</span></span> |

><span data-ttu-id="3340c-305">**Примечание.** Задержка, предусматриваемая для ресурса **alert** , применяется только после создания самого оповещения.</span><span class="sxs-lookup"><span data-stu-id="3340c-305">**Note:** The latency provided for the **alert** resource is only applicable after the alert itself has been created.</span></span> <span data-ttu-id="3340c-306">Она не включает в себя время, необходимое правилу для создания оповещения на основе данных.</span><span class="sxs-lookup"><span data-stu-id="3340c-306">It does not include the time it takes for a rule to create an alert from the data.</span></span>

## <a name="see-also"></a><span data-ttu-id="3340c-307">См. также</span><span class="sxs-lookup"><span data-stu-id="3340c-307">See also</span></span>

- [<span data-ttu-id="3340c-308">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="3340c-308">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="3340c-309">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="3340c-309">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="3340c-310">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="3340c-310">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- <span data-ttu-id="3340c-311">Тип ресурса [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="3340c-311">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) resource type</span></span>
- <span data-ttu-id="3340c-312">Тип ресурса [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="3340c-312">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) resource type</span></span>
- [<span data-ttu-id="3340c-313">Руководство по уведомлениям об изменениях и отслеживанию изменений</span><span class="sxs-lookup"><span data-stu-id="3340c-313">Change notifications and change tracking tutorial</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)
- [<span data-ttu-id="3340c-314">Уведомления жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="3340c-314">Lifecycle notifications</span></span>](/graph/concepts/webhooks-lifecycle.md)

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
[list]: /graph/api/resources/list
[printTaskDefinition]: /graph/api/resources/printtaskdefinition
