---
title: Настройка уведомлений об изменениях в пользовательских данных
description: API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: fda8f362d3554f535012bc058ae4a0c7d5ddcfc7
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082352"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="9e17a-105">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="9e17a-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="9e17a-p102">API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние в случае изменений.</span><span class="sxs-lookup"><span data-stu-id="9e17a-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="9e17a-109">Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке.</span><span class="sxs-lookup"><span data-stu-id="9e17a-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="9e17a-110">Затем приложение действует в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="9e17a-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="9e17a-111">Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.</span><span class="sxs-lookup"><span data-stu-id="9e17a-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="9e17a-112">Создание приложения веб-перехватчика с помощью .NET Core</span><span class="sxs-lookup"><span data-stu-id="9e17a-112">Build a webhook app with .NET Core</span></span>](/graph/tutorials/change-notifications)

<span data-ttu-id="9e17a-113">По умолчанию уведомления об изменениях не включают данные ресурсов, кроме `id`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="9e17a-114">Если приложению требуются данные ресурса, оно может вызвать API Microsoft Graph, чтобы получить ресурс полностью.</span><span class="sxs-lookup"><span data-stu-id="9e17a-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="9e17a-115">В этой статье описывается работа с уведомлениями на примере ресурса **user**.</span><span class="sxs-lookup"><span data-stu-id="9e17a-115">This article uses the **user** resource as an example for working with notifications.</span></span>

<span data-ttu-id="9e17a-116">Приложение также может подписаться на уведомления об изменениях, включающие данные ресурсов, чтобы избежать необходимости дополнительного вызова API для доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="9e17a-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additonal API calls to access the data.</span></span> <span data-ttu-id="9e17a-117">В этом случае приложению необходимо реализовать дополнительный код для обработки требований таких уведомлений, в частности, ответа на уведомления о жизненном цикле подписки, проверки подлинности уведомлений и расшифровки данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9e17a-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="9e17a-118">Другие типы ресурсов также будут поддерживать этот тип уведомлений в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="9e17a-118">More resource types will support this type of notifications in the future.</span></span> <span data-ttu-id="9e17a-119">Дополнительные сведения о работе с такими уведомлениями см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="9e17a-119">For details about how to work with these notificatios, see [Set up change notifications that include resource data (preview)](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="9e17a-120">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="9e17a-120">Supported resources</span></span>

<span data-ttu-id="9e17a-121">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="9e17a-121">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="9e17a-122">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="9e17a-122">Outlook [message][]</span></span>
- <span data-ttu-id="9e17a-123">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="9e17a-123">Outlook [event][]</span></span>
- <span data-ttu-id="9e17a-124">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="9e17a-124">Outlook personal [contact][]</span></span>
- <span data-ttu-id="9e17a-125">[user][]</span><span class="sxs-lookup"><span data-stu-id="9e17a-125">[user][]</span></span>
- <span data-ttu-id="9e17a-126">[group][]</span><span class="sxs-lookup"><span data-stu-id="9e17a-126">[group][]</span></span>
- <span data-ttu-id="9e17a-127">Групповой [чат][] Office 365 </span><span class="sxs-lookup"><span data-stu-id="9e17a-127">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="9e17a-128">Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="9e17a-128">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="9e17a-129">Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="9e17a-129">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="9e17a-130">[Оповещение][] безопасности</span><span class="sxs-lookup"><span data-stu-id="9e17a-130">Security [alert][]</span></span>
- <span data-ttu-id="9e17a-131">Teams [callRecord][] (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9e17a-131">Teams [callRecord][] (preview)</span></span>

<span data-ttu-id="9e17a-132">Например, вы можете создать подписку на определенную папку Outlook, например, папку Входящие: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="9e17a-132">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="9e17a-133">либо на ресурс верхнего уровня: `me/messages`, `me/contacts`, `me/events`, `users` или `groups`;</span><span class="sxs-lookup"><span data-stu-id="9e17a-133">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="9e17a-134">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`;</span><span class="sxs-lookup"><span data-stu-id="9e17a-134">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="9e17a-135">либо на личное хранилище OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-135">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="9e17a-136">либо на корневую папку диска SharePoint/OneDrive для бизнеса: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="9e17a-136">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="9e17a-137">либо на новое оповещение [API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="9e17a-137">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="9e17a-138">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="9e17a-138">Azure AD resource limitations</span></span>

<span data-ttu-id="9e17a-139">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения возникают ошибки.</span><span class="sxs-lookup"><span data-stu-id="9e17a-139">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="9e17a-140">**Примечание**. Эти ограничения не применяются к ресурсам служб, не относящихся к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9e17a-140">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="9e17a-141">Например, приложение может создать больше дополнительных подписок на ресурсы `message` или `event`, поддерживаемые службой Exchange Online в составе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9e17a-141">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="9e17a-142">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="9e17a-142">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="9e17a-143">На приложение: 50 000 подписок всего</span><span class="sxs-lookup"><span data-stu-id="9e17a-143">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="9e17a-144">На клиента: 1000 подписок всего во всех приложениях</span><span class="sxs-lookup"><span data-stu-id="9e17a-144">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="9e17a-145">На сочетание приложения и клиента: 100 подписок всего</span><span class="sxs-lookup"><span data-stu-id="9e17a-145">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="9e17a-146">Если ограничения превышены, попытки создать подписку приведут к [ответу с ошибкой](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-146">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="9e17a-147">Свойство `message` указывает, какое ограничение превышено.</span><span class="sxs-lookup"><span data-stu-id="9e17a-147">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="9e17a-148">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="9e17a-148">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="9e17a-149">Уведомления для сущностей пользователей не поддерживаются для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9e17a-149">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="9e17a-150">В подписках пользователей существует [известная проблема](graph/concepts/known-issues#change-notifications).</span><span class="sxs-lookup"><span data-stu-id="9e17a-150">A [Known issue](graph/concepts/known-issues#change-notifications) exists with user subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="9e17a-151">Ограничения ресурсов Outlook</span><span class="sxs-lookup"><span data-stu-id="9e17a-151">Outlook resource limitations</span></span>

<span data-ttu-id="9e17a-152">Если вы используете *имя участника-пользователя* на пути к ресурсу при оформлении подписки на ресурсы Outlook, например **сообщения**, **события** или **контакты**, запрос на подписку может быть не выполнен, если это имя содержит апостроф. </span><span class="sxs-lookup"><span data-stu-id="9e17a-152">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="9e17a-153">Используйте ИД GUID пользователей вместо имен участников-пользователей, чтобы избежать этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="9e17a-153">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="9e17a-154">Например, вместо пути к ресурсу:</span><span class="sxs-lookup"><span data-stu-id="9e17a-154">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="9e17a-155">Используйте:</span><span class="sxs-lookup"><span data-stu-id="9e17a-155">Use:</span></span> 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a><span data-ttu-id="9e17a-156">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="9e17a-156">Subscription lifetime</span></span>

<span data-ttu-id="9e17a-157">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="9e17a-157">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="9e17a-158">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="9e17a-158">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="9e17a-159">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="9e17a-159">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="9e17a-160">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="9e17a-160">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="9e17a-161">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="9e17a-161">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="9e17a-162">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="9e17a-162">Managing subscriptions</span></span>

<span data-ttu-id="9e17a-163">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="9e17a-163">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="9e17a-164">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="9e17a-164">Creating a subscription</span></span>

<span data-ttu-id="9e17a-p110">Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="9e17a-p110">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="9e17a-167">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="9e17a-167">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="9e17a-168">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="9e17a-168">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="9e17a-169">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="9e17a-169">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="9e17a-170">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9e17a-170">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="9e17a-171">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9e17a-171">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="9e17a-172">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9e17a-172">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="9e17a-173">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления с подписками.</span><span class="sxs-lookup"><span data-stu-id="9e17a-173">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="9e17a-174">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="9e17a-174">Subscription request example</span></span>

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

<span data-ttu-id="9e17a-175">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-175">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="9e17a-176">Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="9e17a-176">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="9e17a-177">Свойство `resource` указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="9e17a-177">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="9e17a-178">Например, вы можете создать подписку на определенную почтовую папку: `me/mailFolders('inbox')/messages` или сделать это от имени пользователя с согласия администратора: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-178">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="9e17a-179">Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="9e17a-179">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="9e17a-180">Задание этого свойства позволит подтверждать, что полученные уведомления поступают от службы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9e17a-180">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="9e17a-181">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9e17a-181">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="9e17a-182">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9e17a-182">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="9e17a-183">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="9e17a-183">Notification endpoint validation</span></span>

<span data-ttu-id="9e17a-184">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="9e17a-184">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="9e17a-185">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="9e17a-185">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="9e17a-186">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="9e17a-186">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="9e17a-187">**Важно!** Так как `validationToken` — это параметр запроса, он должен декодироваться клиентом согласно правилам кодирования HTTP.</span><span class="sxs-lookup"><span data-stu-id="9e17a-187">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="9e17a-188">Если клиент не декодирует маркер и использует закодированное значение на следующем шаге (ответ), конечная точка не пройдет проверку.</span><span class="sxs-lookup"><span data-stu-id="9e17a-188">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="9e17a-189">Кроме того, клиент должен рассматривать значение маркера как непрозрачное, так как формат маркера может измениться в будущем без уведомления.</span><span class="sxs-lookup"><span data-stu-id="9e17a-189">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="9e17a-190">В течение 10 секунд клиент должен предоставить ответ со следующими характеристиками:</span><span class="sxs-lookup"><span data-stu-id="9e17a-190">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="9e17a-191">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="9e17a-191">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="9e17a-192">Необходимый тип контента — `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-192">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="9e17a-193">Текст должен содержать маркер проверки, предоставленный Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9e17a-193">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="9e17a-194">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="9e17a-194">The client should discard the validation token after providing it in the response.</span></span>

<span data-ttu-id="9e17a-195">Кроме того, можно использовать [коллекцию Microsoft Graph Postman](use-postman.md), чтобы убедиться в правильности реализации запроса проверки в вашей конечной точке.</span><span class="sxs-lookup"><span data-stu-id="9e17a-195">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="9e17a-196">Запрос **Проверка подписки** в папке **Прочее** предоставляет модульные тесты, проверяющие отклик вашей конечной точки.</span><span class="sxs-lookup"><span data-stu-id="9e17a-196">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![результаты теста отклика проверки](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="9e17a-198">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="9e17a-198">Renewing a subscription</span></span>

<span data-ttu-id="9e17a-199">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="9e17a-199">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="9e17a-200">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="9e17a-200">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="9e17a-201">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="9e17a-201">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="9e17a-202">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9e17a-202">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="9e17a-203">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-203">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="9e17a-204">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="9e17a-204">Deleting a subscription</span></span>

<span data-ttu-id="9e17a-205">Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="9e17a-205">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="9e17a-206">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-206">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="9e17a-207">Уведомления</span><span class="sxs-lookup"><span data-stu-id="9e17a-207">Notifications</span></span>

<span data-ttu-id="9e17a-208">После создания подписки клиент начнет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="9e17a-208">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="9e17a-209">При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="9e17a-209">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="9e17a-210">Уведомления отправляются только при изменениях типа, указанного в подписке, например, `created`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-210">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="9e17a-211">**Примечание.** Если вы используете несколько подписок, которые отслеживают один тип ресурса и имеют один URL-адрес уведомлений, может быть отправлено сообщение POST, содержащее несколько уведомлений с разными идентификаторами подписок.</span><span class="sxs-lookup"><span data-stu-id="9e17a-211">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="9e17a-212">Уведомления из сообщения POST могут принадлежать разным подпискам.</span><span class="sxs-lookup"><span data-stu-id="9e17a-212">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="9e17a-213">Свойства уведомлений</span><span class="sxs-lookup"><span data-stu-id="9e17a-213">Notification properties</span></span>

<span data-ttu-id="9e17a-214">Объект уведомления содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="9e17a-214">The notification object has the following properties:</span></span>

| <span data-ttu-id="9e17a-215">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e17a-215">Property</span></span> | <span data-ttu-id="9e17a-216">Тип</span><span class="sxs-lookup"><span data-stu-id="9e17a-216">Type</span></span> | <span data-ttu-id="9e17a-217">Описание</span><span class="sxs-lookup"><span data-stu-id="9e17a-217">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="9e17a-218">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="9e17a-218">subscriptionId</span></span> | <span data-ttu-id="9e17a-219">строка</span><span class="sxs-lookup"><span data-stu-id="9e17a-219">string</span></span> | <span data-ttu-id="9e17a-220">Идентификатор подписки, для которого было создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="9e17a-220">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="9e17a-221">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9e17a-221">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="9e17a-222">дата и время</span><span class="sxs-lookup"><span data-stu-id="9e17a-222">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="9e17a-223">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="9e17a-223">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="9e17a-224">clientState</span><span class="sxs-lookup"><span data-stu-id="9e17a-224">clientState</span></span> | <span data-ttu-id="9e17a-225">строка</span><span class="sxs-lookup"><span data-stu-id="9e17a-225">string</span></span> | <span data-ttu-id="9e17a-226">`clientState` — свойство, указанное в запросе на подписку (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="9e17a-226">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="9e17a-227">changeType</span><span class="sxs-lookup"><span data-stu-id="9e17a-227">changeType</span></span> | <span data-ttu-id="9e17a-228">строка</span><span class="sxs-lookup"><span data-stu-id="9e17a-228">string</span></span> | <span data-ttu-id="9e17a-229">Тип события, вызвавшего уведомление.</span><span class="sxs-lookup"><span data-stu-id="9e17a-229">The event type that caused the notification.</span></span> <span data-ttu-id="9e17a-230">Примеры: `created` при получении сообщения или `updated`, когда сообщение помечается как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="9e17a-230">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="9e17a-231">resource</span><span class="sxs-lookup"><span data-stu-id="9e17a-231">resource</span></span> | <span data-ttu-id="9e17a-232">строка</span><span class="sxs-lookup"><span data-stu-id="9e17a-232">string</span></span> | <span data-ttu-id="9e17a-233">Универсальный код ресурса (URI) ресурса относительно `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-233">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="9e17a-234">resourceData</span><span class="sxs-lookup"><span data-stu-id="9e17a-234">resourceData</span></span> | <span data-ttu-id="9e17a-235">объект</span><span class="sxs-lookup"><span data-stu-id="9e17a-235">object</span></span> | <span data-ttu-id="9e17a-236">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="9e17a-236">The content of this property depends on the type of resource being subscribed to.</span></span> |
| <span data-ttu-id="9e17a-237">tenantId</span><span class="sxs-lookup"><span data-stu-id="9e17a-237">tenantId</span></span> | <span data-ttu-id="9e17a-238">string</span><span class="sxs-lookup"><span data-stu-id="9e17a-238">string</span></span> | <span data-ttu-id="9e17a-239">Идентификатор клиента, на основе которого получено уведомление.</span><span class="sxs-lookup"><span data-stu-id="9e17a-239">The ID of the tenant the notification originated from.</span></span> |

<span data-ttu-id="9e17a-240">Например, для ресурсов Outlook `resourceData` содержит такие поля:</span><span class="sxs-lookup"><span data-stu-id="9e17a-240">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="9e17a-241">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e17a-241">Property</span></span> | <span data-ttu-id="9e17a-242">Тип</span><span class="sxs-lookup"><span data-stu-id="9e17a-242">Type</span></span> | <span data-ttu-id="9e17a-243">Описание</span><span class="sxs-lookup"><span data-stu-id="9e17a-243">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="9e17a-244">@odata.type</span><span class="sxs-lookup"><span data-stu-id="9e17a-244">@odata.type</span></span> | <span data-ttu-id="9e17a-245">строка</span><span class="sxs-lookup"><span data-stu-id="9e17a-245">string</span></span> | <span data-ttu-id="9e17a-246">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="9e17a-246">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="9e17a-247">@odata.id</span><span class="sxs-lookup"><span data-stu-id="9e17a-247">@odata.id</span></span> | <span data-ttu-id="9e17a-248">строка</span><span class="sxs-lookup"><span data-stu-id="9e17a-248">string</span></span> | <span data-ttu-id="9e17a-249">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="9e17a-249">The OData identifier of the object.</span></span> |
| <span data-ttu-id="9e17a-250">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="9e17a-250">@odata.etag</span></span> | <span data-ttu-id="9e17a-251">строка</span><span class="sxs-lookup"><span data-stu-id="9e17a-251">string</span></span> | <span data-ttu-id="9e17a-252">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="9e17a-252">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="9e17a-253">id</span><span class="sxs-lookup"><span data-stu-id="9e17a-253">id</span></span> | <span data-ttu-id="9e17a-254">строка</span><span class="sxs-lookup"><span data-stu-id="9e17a-254">string</span></span> | <span data-ttu-id="9e17a-255">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="9e17a-255">The identifier of the object.</span></span> |

> <span data-ttu-id="9e17a-256">**Примечание.** Значение `id`, указанное в `resourceData`, действительно в момент создания уведомления.</span><span class="sxs-lookup"><span data-stu-id="9e17a-256">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="9e17a-257">Некоторые действия, такие как перемещение сообщения в другую папку, могут привести к недействительности `id` во время обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="9e17a-257">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="9e17a-258">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="9e17a-258">Notification example</span></span>

<span data-ttu-id="9e17a-259">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления, аналогичные указанному ниже.</span><span class="sxs-lookup"><span data-stu-id="9e17a-259">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
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

<span data-ttu-id="9e17a-260">Обратите внимание, что поле `value` представляет собой массив объектов.</span><span class="sxs-lookup"><span data-stu-id="9e17a-260">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="9e17a-261">Если в очереди много уведомлений, Microsoft Graph может отправлять несколько элементов в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="9e17a-261">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="9e17a-262">В одном запросе уведомления могут содержаться уведомления от разных подписок.</span><span class="sxs-lookup"><span data-stu-id="9e17a-262">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="9e17a-263">Обработка уведомления</span><span class="sxs-lookup"><span data-stu-id="9e17a-263">Processing the notification</span></span>

<span data-ttu-id="9e17a-264">Необходимо обрабатывать все уведомления, полученные программой.</span><span class="sxs-lookup"><span data-stu-id="9e17a-264">Each notification received by your app should be processed.</span></span> <span data-ttu-id="9e17a-265">Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.</span><span class="sxs-lookup"><span data-stu-id="9e17a-265">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="9e17a-266">Отправьте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9e17a-266">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="9e17a-267">Если 2хх код не будет получен, Microsoft Graph попытается опубликовать уведомление несколько раз в течение 4 часов. После этого уведомление будет удалено.</span><span class="sxs-lookup"><span data-stu-id="9e17a-267">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the notification a number of times, for a period of about 4 hours; after that, the notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="9e17a-268">**Примечание.** Отправьте код состояния `202 - Accepted` сразу после получения уведомления, еще перед проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="9e17a-268">**Note:** Send a `202 - Accepted` status code as soon as you receive the notification, even before validating its authenticity.</span></span> <span data-ttu-id="9e17a-269">Просто подтвердите получение уведомления, чтобы избежать ненужных повторных попыток.  </span><span class="sxs-lookup"><span data-stu-id="9e17a-269">You are simply acknowledging the receipt of the notification and preventing unnecessary retries.</span></span> <span data-ttu-id="9e17a-270">Текущее значение времени ожидания — 30 секунд, но это время может быть сокращено в будущем для оптимизации производительности службы.</span><span class="sxs-lookup"><span data-stu-id="9e17a-270">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span>

1. <span data-ttu-id="9e17a-271">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="9e17a-271">Validate the `clientState` property.</span></span> <span data-ttu-id="9e17a-272">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="9e17a-272">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="9e17a-273">**Примечание.** Если это не так, уведомление не следует рассматривать как действительное.</span><span class="sxs-lookup"><span data-stu-id="9e17a-273">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="9e17a-274">Возможно уведомление создано не Microsoft Graph и отправлено незаконным субъектом.</span><span class="sxs-lookup"><span data-stu-id="9e17a-274">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="9e17a-275">Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="9e17a-275">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="9e17a-276">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="9e17a-276">Update your application based on your business logic.</span></span>

<span data-ttu-id="9e17a-277">Повторяйте эти действия для других уведомлений в запросе.</span><span class="sxs-lookup"><span data-stu-id="9e17a-277">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="9e17a-278">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="9e17a-278">Code samples</span></span>

<span data-ttu-id="9e17a-279">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="9e17a-279">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="9e17a-280">Обучающий модуль по Microsoft Graph: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9e17a-280">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="9e17a-281">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="9e17a-281">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="9e17a-282">Пример веб-перехватчиков Microsoft Graph для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="9e17a-282">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="9e17a-283">Пример веб-перехватчиков Microsoft Graph для WebJobs SDK</span><span class="sxs-lookup"><span data-stu-id="9e17a-283">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="9e17a-284">См. также</span><span class="sxs-lookup"><span data-stu-id="9e17a-284">See also</span></span>

- [<span data-ttu-id="9e17a-285">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="9e17a-285">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="9e17a-286">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="9e17a-286">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="9e17a-287">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="9e17a-287">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="9e17a-288">Учебник по уведомлениям об изменениях</span><span class="sxs-lookup"><span data-stu-id="9e17a-288">Change notifications tutorial</span></span>](/graph/tutorials/change-notifications)
- [<span data-ttu-id="9e17a-289">Уведомления в жизненном цикле (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9e17a-289">Lifecycle notifications (preview)</span></span>](/graph/concepts/webhooks-outlook-authz.md)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-beta
