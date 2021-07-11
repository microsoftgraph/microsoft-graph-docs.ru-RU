---
title: Настройка уведомлений об изменениях в пользовательских данных
description: API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях для клиентов. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений об изменениях. С помощью этих уведомлений клиентские приложения обновляют свое состояние в случае изменений.
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 5f25acf793d2b8bda00e298665ae8f9766f410b4
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366886"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="1a1ba-105">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="1a1ba-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="1a1ba-p102">API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях для клиентов. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений об изменениях. С помощью этих уведомлений клиентские приложения обновляют свое состояние в случае изменений.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-p102">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.</span></span>

<span data-ttu-id="1a1ba-p103">Приняв запрос на подписку, Microsoft Graph отправляет уведомления об изменениях на URL-адрес, указанный в подписке. Затем приложение действует в соответствии с бизнес-логикой. Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-p103">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="1a1ba-112">Руководство: Использование уведомлений об изменениях и функции отслеживания изменений в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a1ba-112">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

<span data-ttu-id="1a1ba-113">По умолчанию уведомления об изменениях не включают данные ресурсов, кроме `id`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="1a1ba-114">Если приложению требуются данные ресурса, оно может вызвать API Microsoft Graph, чтобы получить ресурс полностью.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="1a1ba-115">В этой статье описывается работа с уведомлениями об изменениях на примере ресурса **user**.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-115">This article uses the **user** resource as an example for working with change notifications.</span></span>

<span data-ttu-id="1a1ba-116">Приложение также может подписаться на уведомления об изменениях, включающие данные ресурсов, чтобы избежать необходимости дополнительного вызова API для доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additional API calls to access the data.</span></span> <span data-ttu-id="1a1ba-117">В этом случае приложению необходимо реализовать дополнительный код для обработки требований таких уведомлений, в частности, ответа на уведомления о жизненном цикле подписки, проверки подлинности уведомлений и расшифровки данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="1a1ba-118">Дополнительные сведения о работе с такими уведомлениями см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="1a1ba-118">For details about how to work with these notifications, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="1a1ba-119">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="1a1ba-119">Supported resources</span></span>

<span data-ttu-id="1a1ba-120">С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="1a1ba-120">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="1a1ba-121">Облачная печать [printer][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-121">Cloud printing [printer][]</span></span>
- <span data-ttu-id="1a1ba-122">Облачная печать [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-122">Cloud printing [printTaskDefinition][]</span></span>
- <span data-ttu-id="1a1ba-123">Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="1a1ba-123">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="1a1ba-124">Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="1a1ba-124">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="1a1ba-125">[group][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-125">[group][]</span></span>
- <span data-ttu-id="1a1ba-126">Групповой [чат][] Microsoft 365 </span><span class="sxs-lookup"><span data-stu-id="1a1ba-126">Microsoft 365 group [conversation][]</span></span>
- <span data-ttu-id="1a1ba-127">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="1a1ba-127">Outlook [event][]</span></span>
- <span data-ttu-id="1a1ba-128">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="1a1ba-128">Outlook [message][]</span></span>
- <span data-ttu-id="1a1ba-129">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="1a1ba-129">Outlook personal [contact][]</span></span>
- <span data-ttu-id="1a1ba-130">[Оповещение][] безопасности</span><span class="sxs-lookup"><span data-stu-id="1a1ba-130">Security [alert][]</span></span>
- <span data-ttu-id="1a1ba-131">[Список][] SharePoint</span><span class="sxs-lookup"><span data-stu-id="1a1ba-131">SharePoint [list][]</span></span>
- <span data-ttu-id="1a1ba-132">[callRecord][] в Teams</span><span class="sxs-lookup"><span data-stu-id="1a1ba-132">Teams [callRecord][]</span></span>
- <span data-ttu-id="1a1ba-133">[Канал][] Teams </span><span class="sxs-lookup"><span data-stu-id="1a1ba-133">Teams [channel][]</span></span>
- <span data-ttu-id="1a1ba-134">[Чат][] Teams</span><span class="sxs-lookup"><span data-stu-id="1a1ba-134">Teams [chat][]</span></span>
- <span data-ttu-id="1a1ba-135">[chatMessage][] Teams</span><span class="sxs-lookup"><span data-stu-id="1a1ba-135">Teams [chatMessage][]</span></span>
- <span data-ttu-id="1a1ba-136">[conversationMember][] в Teams</span><span class="sxs-lookup"><span data-stu-id="1a1ba-136">Teams [conversationMember][]</span></span>
- <span data-ttu-id="1a1ba-137">[Присутствие][] в Teams (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1a1ba-137">Teams [presence][] (preview)</span></span>
- <span data-ttu-id="1a1ba-138">[Команда][] Teams</span><span class="sxs-lookup"><span data-stu-id="1a1ba-138">Teams [team][]</span></span>
- <span data-ttu-id="1a1ba-139">[todoTask][] (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1a1ba-139">[todoTask][] (preview)</span></span>
- <span data-ttu-id="1a1ba-140">[пользователь][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-140">[user][]</span></span>

<span data-ttu-id="1a1ba-141">Вы можете создать подписку на определенную папку Outlook, например, папку Входящие: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="1a1ba-141">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="1a1ba-142">либо на ресурс верхнего уровня: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="1a1ba-142">Or to a top-level resource: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, `/communications/callRecords`</span></span>

<span data-ttu-id="1a1ba-143">либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`, `sites/{site-id}/lists/{list-id}`, `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="1a1ba-143">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`, `sites/{site-id}/lists/{list-id}`, `/communications/presences/{id}`</span></span>

<span data-ttu-id="1a1ba-144">либо на личное хранилище OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-144">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="1a1ba-145">либо на корневую папку диска SharePoint/OneDrive для бизнеса: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="1a1ba-145">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="1a1ba-146">либо на новое оповещение [API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="1a1ba-146">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

<span data-ttu-id="1a1ba-147">либо на задачи в списке дел пользователя: `/me/todo/lists/{todoTaskListId}/tasks`</span><span class="sxs-lookup"><span data-stu-id="1a1ba-147">Or to the tasks in a user's To Do list: `/me/todo/lists/{todoTaskListId}/tasks`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="1a1ba-148">Ограничения ресурсов Azure AD</span><span class="sxs-lookup"><span data-stu-id="1a1ba-148">Azure AD resource limitations</span></span>

<span data-ttu-id="1a1ba-149">К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения возникают ошибки.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-149">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="1a1ba-150">**Примечание**. Эти ограничения не применяются к ресурсам служб, не относящихся к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-150">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="1a1ba-151">Например, приложение может создать больше дополнительных подписок на ресурсы `message` или `event`, поддерживаемые службой Exchange Online в составе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-151">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="1a1ba-152">Квоты максимальной подписки:</span><span class="sxs-lookup"><span data-stu-id="1a1ba-152">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="1a1ba-153">На приложение (для сочетания всех клиентов): 50 000 подписок всего</span><span class="sxs-lookup"><span data-stu-id="1a1ba-153">Per app (for all tenants combined): 50,000 total subscriptions</span></span>
  - <span data-ttu-id="1a1ba-154">На клиента (для сочетания всех приложений): 1000 подписок всего во всех приложениях</span><span class="sxs-lookup"><span data-stu-id="1a1ba-154">Per tenant (for all applications combined): 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="1a1ba-155">На сочетание приложения и клиента: 100 подписок всего</span><span class="sxs-lookup"><span data-stu-id="1a1ba-155">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="1a1ba-156">Если какое-либо ограничение превышено, попытки создать подписку приведут к [ответу с ошибкой](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-156">When any limit is exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="1a1ba-157">Свойство `message` указывает, какое ограничение превышено.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-157">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="1a1ba-158">Клиенты Azure AD B2C не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-158">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="1a1ba-159">Уведомления об изменениях для сущностей пользователей не поддерживаются для личных учетных записей Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-159">Change notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="1a1ba-160">В подписках пользователей и групп существует [известная проблема](known-issues.md#change-notifications).</span><span class="sxs-lookup"><span data-stu-id="1a1ba-160">A [known issue](known-issues.md#change-notifications) exists with user and group subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="1a1ba-161">Ограничения ресурсов Outlook</span><span class="sxs-lookup"><span data-stu-id="1a1ba-161">Outlook resource limitations</span></span>

<span data-ttu-id="1a1ba-162">Если вы используете *имя участника-пользователя* на пути к ресурсу при оформлении подписки на ресурсы Outlook, например **сообщения**, **события** или **контакты**, запрос на подписку может быть не выполнен, если это имя содержит апостроф. </span><span class="sxs-lookup"><span data-stu-id="1a1ba-162">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="1a1ba-163">Используйте ИД GUID пользователей вместо имен участников-пользователей, чтобы избежать этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-163">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="1a1ba-164">Например, вместо пути к ресурсу:</span><span class="sxs-lookup"><span data-stu-id="1a1ba-164">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="1a1ba-165">Используйте:</span><span class="sxs-lookup"><span data-stu-id="1a1ba-165">Use:</span></span>

`/users/{guid-user-id}/messages`

<span data-ttu-id="1a1ba-166">Доступно не более 1000 активных подписок на почтовый ящик для всех приложений.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-166">A maximum of 1000 active subscriptions per mailbox for all applications is allowed.</span></span>

### <a name="teams-resource-limitations"></a><span data-ttu-id="1a1ba-167">Ограничения ресурсов Teams</span><span class="sxs-lookup"><span data-stu-id="1a1ba-167">Teams resource limitations</span></span>

<span data-ttu-id="1a1ba-168">Каждый ресурс Teams имеет различные квоты подписки.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-168">Each Teams resource has different subscription quotas.</span></span>

- <span data-ttu-id="1a1ba-169">Для подписок на **callRecords**:</span><span class="sxs-lookup"><span data-stu-id="1a1ba-169">For subscriptions to **callRecords**:</span></span>
  - <span data-ttu-id="1a1ba-170">На организацию: всего 100 подписок</span><span class="sxs-lookup"><span data-stu-id="1a1ba-170">Per organization: 100 total subscriptions</span></span>

- <span data-ttu-id="1a1ba-171">Для подписок на **chatMessages** (каналы или чаты):</span><span class="sxs-lookup"><span data-stu-id="1a1ba-171">For subscriptions to **chatMessages** (channels or chats):</span></span>
  - <span data-ttu-id="1a1ba-172">На сочетание приложения и канала или чата: 1 подписка</span><span class="sxs-lookup"><span data-stu-id="1a1ba-172">Per app and channel or chat combination: 1 subscription</span></span>
  - <span data-ttu-id="1a1ba-173">На организацию: всего 10 000 подписок</span><span class="sxs-lookup"><span data-stu-id="1a1ba-173">Per organization: 10,000 total subscriptions</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="1a1ba-174">Время существования подписки</span><span class="sxs-lookup"><span data-stu-id="1a1ba-174">Subscription lifetime</span></span>

<span data-ttu-id="1a1ba-175">Время существования подписок ограничено.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-175">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="1a1ba-176">Приложениям необходимо обновлять подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-176">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="1a1ba-177">В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-177">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="1a1ba-178">Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="1a1ba-178">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="1a1ba-179">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-179">Apps can also unsubscribe at any time to stop getting change notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="1a1ba-180">Управление подписками</span><span class="sxs-lookup"><span data-stu-id="1a1ba-180">Managing subscriptions</span></span>

<span data-ttu-id="1a1ba-181">Клиенты могут создавать, продлевать и удалять подписки.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-181">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="1a1ba-182">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="1a1ba-182">Creating a subscription</span></span>

<span data-ttu-id="1a1ba-p110">Чтобы начать получать уведомления об изменениях ресурса, сначала необходимо создать подписку. Это выполняется следующим образом.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-p110">Creating a subscription is the first step to start receiving change notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="1a1ba-185">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-185">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="1a1ba-186">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-186">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="1a1ba-187">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-187">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="1a1ba-188">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-188">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="1a1ba-189">Клиент отправляет маркер проверки в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-189">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="1a1ba-190">Клиент получает ответ от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-190">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="1a1ba-191">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления об изменениях с подписками.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-191">The client must store the subscription ID to correlate change notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="1a1ba-192">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="1a1ba-192">Subscription request example</span></span>

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

<span data-ttu-id="1a1ba-193">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-193">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="1a1ba-194">Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription).</span><span class="sxs-lookup"><span data-stu-id="1a1ba-194">See [subscription resource type](/graph/api/resources/subscription) for property definitions and values.</span></span>

<span data-ttu-id="1a1ba-195">Свойство `resource` указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-195">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="1a1ba-196">Например, вы можете создать подписку на определенную почтовую папку: `me/mailFolders('inbox')/messages` или сделать это от имени пользователя с согласия администратора: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-196">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="1a1ba-197">Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-197">Although `clientState` is not required, you must include it to comply with our recommended change notification handling process.</span></span> <span data-ttu-id="1a1ba-198">Задание этого свойства позволит подтверждать, что полученные уведомления об изменениях поступают от службы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-198">Setting this property will allow you to confirm that change notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="1a1ba-199">По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-199">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="1a1ba-200">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-200">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription) object in the body.</span></span>

> <span data-ttu-id="1a1ba-201">**Примечание.** Любой параметр строки запроса, включенный в свойство **notificationUrl**, будет включен в HTTP-запрос POST при доставке уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-201">**Note:** Any query string parameter included in the **notificationUrl** property will be included in the HTTP POST request when notifications are being delivered.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="1a1ba-202">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="1a1ba-202">Notification endpoint validation</span></span>

<span data-ttu-id="1a1ba-203">Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-203">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="1a1ba-204">Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="1a1ba-204">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="1a1ba-205">Microsoft Graph кодирует маркер проверки и включает его в запрос POST URL-адреса уведомления:</span><span class="sxs-lookup"><span data-stu-id="1a1ba-205">Microsoft Graph encodes a validation token and includes it in a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

1. <span data-ttu-id="1a1ba-206">Клиенту необходимо правильно расшифровать URL-адрес параметра запроса`validationToken`, предоставленный на предыдущем этапе, и избегать любого HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-206">The client must properly URL decode the `validationToken` query parameter provided in the preceding step, and escape any HTML/JavaScript.</span></span>

   <span data-ttu-id="1a1ba-207">Рекомендуется их избегать, поскольку злоумышленники могут использовать конечную точку уведомления для атаки типа межсайтовых сценариев.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-207">Escaping is a good practice because malicious actors can use the notification endpoint for cross-site scripting type of attacks.</span></span>

   <span data-ttu-id="1a1ba-208">Как правило, значение маркера проверки рассматривается как непрозрачное, так как формат маркера обычно меняется без уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-208">In general, treat the validation token value as opaque, as the token format can generally change without notice.</span></span> <span data-ttu-id="1a1ba-209">Microsoft Graph никогда не отправляет значения, содержащие код HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-209">Microsoft Graph never sends any value containing HTML or JavaScript code.</span></span>

1. <span data-ttu-id="1a1ba-210">В течение 10 секунд первого этапа клиент должен предоставить ответ со следующими характеристиками:</span><span class="sxs-lookup"><span data-stu-id="1a1ba-210">The client must provide a response with the following characteristics within 10 seconds of step 1:</span></span>

    - <span data-ttu-id="1a1ba-211">Код состояния `HTTP 200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-211">A status code of `HTTP 200 OK`.</span></span>
    - <span data-ttu-id="1a1ba-212">Тип контента `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-212">A content type of `text/plain`.</span></span>
    - <span data-ttu-id="1a1ba-213">Основной текст, включающий маркер проверки с _расшифрованным URL-адресом_.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-213">A body that includes the _URL decoded_ validation token.</span></span> <span data-ttu-id="1a1ba-214">Просто отобразите ту же строку, которая была отправлена в параметре запроса `validationToken`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-214">Simply reflect back the same string that was sent in the `validationToken` query parameter.</span></span>

    <span data-ttu-id="1a1ba-215">Клиент должен удалить маркер проверки после того, как укажет его в отклике.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-215">The client should discard the validation token after providing it in the response.</span></span>

    > <span data-ttu-id="1a1ba-216">**Важно!** Если клиент возвращает зашифрованный маркер проверки, проверка завершится ошибкой.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-216">**Important:** If the client returns an encoded validation token, the validation will fail.</span></span>

<span data-ttu-id="1a1ba-217">Кроме того, можно использовать [коллекцию Microsoft Graph Postman](use-postman.md), чтобы убедиться в правильности реализации запроса проверки в вашей конечной точке.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-217">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="1a1ba-218">Запрос **Проверка подписки** в папке **Прочее** предоставляет модульные тесты, проверяющие отклик вашей конечной точки.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-218">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![результаты теста отклика проверки](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="1a1ba-220">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="1a1ba-220">Renewing a subscription</span></span>

<span data-ttu-id="1a1ba-221">Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-221">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="1a1ba-222">Свойство `expirationDateTime` является обязательным.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-222">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="1a1ba-223">Пример возобновления подписки</span><span class="sxs-lookup"><span data-stu-id="1a1ba-223">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="1a1ba-224">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-224">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription) object in the body.</span></span> <span data-ttu-id="1a1ba-225">Объект подписки включает новое значение `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-225">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="1a1ba-226">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="1a1ba-226">Deleting a subscription</span></span>

<span data-ttu-id="1a1ba-227">Клиент может прекратить получать уведомления об изменениях, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-227">The client can stop receiving change notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="1a1ba-228">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-228">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="1a1ba-229">Уведомления об изменениях</span><span class="sxs-lookup"><span data-stu-id="1a1ba-229">Change notifications</span></span>

<span data-ttu-id="1a1ba-230">Когда клиент подписывается на изменения ресурса, Microsoft Graph отправляет запрос `POST` в URL-адрес уведомления при каждом изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-230">With a client subscribing to changes to a resource, Microsoft Graph sends a `POST` request to the notification URL whenever the resource changes.</span></span> <span data-ttu-id="1a1ba-231">Уведомления отправляются только при изменениях типа, указанного в подписке, например, `created`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-231">It sends notifications only for changes of the type that's specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="1a1ba-232">**Примечание.** Если клиент имеет несколько подписок, которые контролируют один ресурс и используют один URL-адрес уведомлений, Microsoft Graph может отправлять несколько уведомлений об изменениях, соответствующих разным подпискам, каждое из которых показывает идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-232">**Note:** If a client has multiple subscriptions that monitor the same resource and use the same notification URL, Microsoft Graph can send multiple change notifications that correspond to different subscriptions, each showing the corresponding subscription ID.</span></span> <span data-ttu-id="1a1ba-233">Уведомления об изменениях из сообщения `POST` могут принадлежать разным подпискам.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-233">There is no guarantee that all change notifications in the `POST` request belong to a single subscription.</span></span>

### <a name="change-notification-example"></a><span data-ttu-id="1a1ba-234">Пример уведомления об изменениях</span><span class="sxs-lookup"><span data-stu-id="1a1ba-234">Change notification example</span></span>

<span data-ttu-id="1a1ba-235">В этом разделе указан пример уведомления для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-235">This section shows an example of a notification for a message creation.</span></span> <span data-ttu-id="1a1ba-236">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления об изменениях, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-236">When the user receives an email, Microsoft Graph sends a change notification as shown in the following example.</span></span>
<span data-ttu-id="1a1ba-237">Обратите внимание на то, что уведомление является коллекцией, представленной в поле "`value`".</span><span class="sxs-lookup"><span data-stu-id="1a1ba-237">Note that the notification is in a collection represented in the `value` field.</span></span> <span data-ttu-id="1a1ba-238">Дополнительные сведения о полезных данных уведомлений см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection)</span><span class="sxs-lookup"><span data-stu-id="1a1ba-238">See [changeNotificationCollection](/graph/api/resources/changenotificationcollection) for details of the notification payload.</span></span> 

<span data-ttu-id="1a1ba-239">При многочисленных изменениях Microsoft Graph может отправлять несколько уведомлений, соответствующих разным подпискам, в одном и том же запросе `POST`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-239">When many changes occur, Microsoft Graph may send multiple notifications that correspond to different subscriptions in the same `POST` request.</span></span>

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

### <a name="processing-the-change-notification"></a><span data-ttu-id="1a1ba-240">Обработка уведомлений об изменениях</span><span class="sxs-lookup"><span data-stu-id="1a1ba-240">Processing the change notification</span></span>

<span data-ttu-id="1a1ba-241">Процесс должен обрабатывать каждое уведомление об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-241">Your process should process every change notification it receives.</span></span> <span data-ttu-id="1a1ba-242">Ниже перечислены основные задачи, которые приложение должно выполнить для обработки таких уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-242">The following are the minimum tasks that your app must perform to process a change notification:</span></span>

1. <span data-ttu-id="1a1ba-243">Отправьте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-243">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="1a1ba-244">Если 2хх код не будет получен, Microsoft Graph попытается опубликовать уведомление об изменении несколько раз в течение 4 часов. После этого это уведомление будет удалено.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-244">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the change notification a number of times, for a period of about 4 hours; after that, the change notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="1a1ba-245">**Примечание.** Отправьте код состояния `202 - Accepted` сразу после получения уведомления об изменениях, еще перед проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-245">**Note:** Send a `202 - Accepted` status code as soon as you receive the change notification, even before validating its authenticity.</span></span> <span data-ttu-id="1a1ba-246">Просто подтвердите получение уведомления об изменениях, чтобы избежать ненужных повторных попыток.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-246">You are simply acknowledging the receipt of the change notification and preventing unnecessary retries.</span></span> <span data-ttu-id="1a1ba-247">Текущее значение времени ожидания — 30 секунд, но это время может быть сокращено в будущем для оптимизации производительности службы.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-247">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span> <span data-ttu-id="1a1ba-248">Если URL-адрес уведомления не отвечает в течение 30 секунд на более чем 10% запросов от Microsoft Graph за 10 минут, все уведомления ниже будут отложены и повторено выполнены в течение 4 часов.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-248">If the notification URL doesn't reply within 30 seconds for more than 10% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be delayed and retried for a period of 4 hours.</span></span> <span data-ttu-id="1a1ba-249">Если URL-адрес уведомления не отвечает в течение 30 секунд на более чем 20% запросов от Microsoft Graph за 10 минут, все уведомления ниже будут удалены.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-249">If a notification URL doesn't reply within 30 seconds for more than 20% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be dropped.</span></span>

1. <span data-ttu-id="1a1ba-250">Проверьте свойство `clientState`.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-250">Validate the `clientState` property.</span></span> <span data-ttu-id="1a1ba-251">Оно должно соответствовать значению, отправленному с запросом на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-251">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="1a1ba-252">**Примечание.** Если это не так, уведомление об изменениях не следует рассматривать как действительное.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-252">**Note:** If this isn't true, you should not consider this a valid change notification.</span></span> <span data-ttu-id="1a1ba-253">Возможно оно создано не Microsoft Graph и отправлено незаконным субъектом.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-253">It is possible that the change notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="1a1ba-254">Вы также можете определить, откуда поступило уведомление об изменениях, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-254">You should also investigate where the change notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="1a1ba-255">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-255">Update your application based on your business logic.</span></span>

<span data-ttu-id="1a1ba-256">Повторяйте эти действия для других уведомлений об изменениях в запросе.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-256">Repeat for other change notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="1a1ba-257">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="1a1ba-257">Code samples</span></span>

<span data-ttu-id="1a1ba-258">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-258">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="1a1ba-259">Обучающий модуль по Microsoft Graph: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a1ba-259">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="1a1ba-260">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="1a1ba-260">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [<span data-ttu-id="1a1ba-261">Пример веб-перехватчиков Microsoft Graph для ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="1a1ba-261">Microsoft Graph Webhooks Sample for ASP.NET Core</span></span>](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [<span data-ttu-id="1a1ba-262">Пример веб-перехватчиков Microsoft Graph для Java Spring</span><span class="sxs-lookup"><span data-stu-id="1a1ba-262">Microsoft Graph Webhooks Sample for Java Spring</span></span>](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a><span data-ttu-id="1a1ba-263">Конфигурация брандмауэра</span><span class="sxs-lookup"><span data-stu-id="1a1ba-263">Firewall configuration</span></span>

<span data-ttu-id="1a1ba-264">При необходимости можно настроить брандмауэр, который защищает URL-адрес уведомления, чтобы разрешить входящие подключения только из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-264">You can optionally configure the firewall that protects your notification URL to allow inbound connections only from Microsoft Graph.</span></span> <span data-ttu-id="1a1ba-265">Это позволит снизить дополнительное воздействие недопустимых уведомлений об изменениях, которые отправляются на URL-адрес уведомления.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-265">This allows you to reduce further exposure to invalid change notifications that are sent to your notification URL.</span></span> <span data-ttu-id="1a1ba-266">Такие недействительные уведомления об изменениях могут пытаться активировать реализуемую вами пользовательскую логику.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-266">These invalid change notifications can be trying to trigger the custom logic that you implemented.</span></span> <span data-ttu-id="1a1ba-267">Полный список IP-адресов, которые используются Microsoft Graph для доставки уведомлений об изменениях, см в сведениях о[дополнительных конечных точках для Microsoft 365](/office365/enterprise/additional-office365-ip-addresses-and-urls).</span><span class="sxs-lookup"><span data-stu-id="1a1ba-267">For a complete list of IP addresses used by Microsoft Graph to deliver change notifications, see [additional endpoints for Microsoft 365](/office365/enterprise/additional-office365-ip-addresses-and-urls).</span></span>

> <span data-ttu-id="1a1ba-268">**Примечание.** Указанные IP-адреса, которые используются для доставки уведомлений об изменениях, можно обновлять в любой момент без предварительных примечаний.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-268">**Note:** The listed IP addresses that are used to deliver change notifications can be updated at any time without notice.</span></span>

## <a name="latency"></a><span data-ttu-id="1a1ba-269">Задержка</span><span class="sxs-lookup"><span data-stu-id="1a1ba-269">Latency</span></span>

<span data-ttu-id="1a1ba-270">В следующей таблице указаны ожидаемые задержки между возникновением события в службе и доставкой уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-270">The following table lists the latency to expect between an event happening in the service and the delivery of the change notification.</span></span>

| <span data-ttu-id="1a1ba-271">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1a1ba-271">Resource</span></span> | <span data-ttu-id="1a1ba-272">Средняя задержка</span><span class="sxs-lookup"><span data-stu-id="1a1ba-272">Average latency</span></span> | <span data-ttu-id="1a1ba-273">Максимальная задержка</span><span class="sxs-lookup"><span data-stu-id="1a1ba-273">Maximum latency</span></span> |
|:-----|:-----|:-----|
|<span data-ttu-id="1a1ba-274">[alert][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-274">[alert][]</span></span> | <span data-ttu-id="1a1ba-275">Менее 3 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-275">Less than 3 minutes</span></span> | <span data-ttu-id="1a1ba-276">5 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-276">5 minutes</span></span> |
|<span data-ttu-id="1a1ba-277">[callRecord][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-277">[callRecord][]</span></span> | <span data-ttu-id="1a1ba-278">Менее 15 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-278">Less than 15 minutes</span></span> | <span data-ttu-id="1a1ba-279">60 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-279">60 minutes</span></span> |
|<span data-ttu-id="1a1ba-280">[channel][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-280">[channel][]</span></span> | <span data-ttu-id="1a1ba-281">Менее 10 секунд</span><span class="sxs-lookup"><span data-stu-id="1a1ba-281">Less than 10 seconds</span></span> | <span data-ttu-id="1a1ba-282">60 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-282">60 minutes</span></span> |
|<span data-ttu-id="1a1ba-283">[chat][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-283">[chat][]</span></span> | <span data-ttu-id="1a1ba-284">Менее 10 секунд</span><span class="sxs-lookup"><span data-stu-id="1a1ba-284">Less than 10 seconds</span></span> | <span data-ttu-id="1a1ba-285">60 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-285">60 minutes</span></span> |
|<span data-ttu-id="1a1ba-286">[chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-286">[chatMessage][]</span></span> | <span data-ttu-id="1a1ba-287">Менее 10 секунд</span><span class="sxs-lookup"><span data-stu-id="1a1ba-287">Less than 10 seconds</span></span> | <span data-ttu-id="1a1ba-288">1 минута</span><span class="sxs-lookup"><span data-stu-id="1a1ba-288">1 minute</span></span> |
|<span data-ttu-id="1a1ba-289">[contact][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-289">[contact][]</span></span> | <span data-ttu-id="1a1ba-290">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="1a1ba-290">Unknown</span></span> | <span data-ttu-id="1a1ba-291">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="1a1ba-291">Unknown</span></span> |
|<span data-ttu-id="1a1ba-292">[conversation][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-292">[conversation][]</span></span> | <span data-ttu-id="1a1ba-293">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="1a1ba-293">Unknown</span></span> | <span data-ttu-id="1a1ba-294">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="1a1ba-294">Unknown</span></span> |
|<span data-ttu-id="1a1ba-295">[conversationMember][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-295">[conversationMember][]</span></span> | <span data-ttu-id="1a1ba-296">Менее 10 секунд</span><span class="sxs-lookup"><span data-stu-id="1a1ba-296">Less than 10 seconds</span></span> | <span data-ttu-id="1a1ba-297">60 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-297">60 minutes</span></span> |
|<span data-ttu-id="1a1ba-298">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-298">[driveItem][]</span></span> | <span data-ttu-id="1a1ba-299">Менее 1 минуты</span><span class="sxs-lookup"><span data-stu-id="1a1ba-299">Less than 1 minute</span></span> | <span data-ttu-id="1a1ba-300">5 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-300">5 minutes</span></span> |
|<span data-ttu-id="1a1ba-301">[event][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-301">[event][]</span></span> | <span data-ttu-id="1a1ba-302">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="1a1ba-302">Unknown</span></span> | <span data-ttu-id="1a1ba-303">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="1a1ba-303">Unknown</span></span> |
|<span data-ttu-id="1a1ba-304">[group][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-304">[group][]</span></span> | <span data-ttu-id="1a1ba-305">Менее 2 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-305">Less than 2 minutes</span></span> | <span data-ttu-id="1a1ba-306">15 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-306">15 minutes</span></span> |
|<span data-ttu-id="1a1ba-307">[list][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-307">[list][]</span></span> | <span data-ttu-id="1a1ba-308">Менее 1 минуты</span><span class="sxs-lookup"><span data-stu-id="1a1ba-308">Less than 1 minute</span></span> | <span data-ttu-id="1a1ba-309">5 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-309">5 minutes</span></span> |
|<span data-ttu-id="1a1ba-310">[message][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-310">[message][]</span></span> | <span data-ttu-id="1a1ba-311">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="1a1ba-311">Unknown</span></span> | <span data-ttu-id="1a1ba-312">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="1a1ba-312">Unknown</span></span> |
|<span data-ttu-id="1a1ba-313">[presence][] (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1a1ba-313">[presence][] (preview)</span></span> | <span data-ttu-id="1a1ba-314">Менее 10 секунд</span><span class="sxs-lookup"><span data-stu-id="1a1ba-314">Less than 10 seconds</span></span> | <span data-ttu-id="1a1ba-315">1 минута</span><span class="sxs-lookup"><span data-stu-id="1a1ba-315">1 minute</span></span> |
|<span data-ttu-id="1a1ba-316">[printer][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-316">[printer][]</span></span> | <span data-ttu-id="1a1ba-317">Менее 1 минуты</span><span class="sxs-lookup"><span data-stu-id="1a1ba-317">Less than 1 minute</span></span> | <span data-ttu-id="1a1ba-318">5 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-318">5 minutes</span></span> |
|<span data-ttu-id="1a1ba-319">[printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-319">[printTaskDefinition][]</span></span> | <span data-ttu-id="1a1ba-320">Менее 1 минуты</span><span class="sxs-lookup"><span data-stu-id="1a1ba-320">Less than 1 minute</span></span> | <span data-ttu-id="1a1ba-321">5 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-321">5 minutes</span></span> |
|<span data-ttu-id="1a1ba-322">[team][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-322">[team][]</span></span> | <span data-ttu-id="1a1ba-323">Менее 10 секунд</span><span class="sxs-lookup"><span data-stu-id="1a1ba-323">Less than 10 seconds</span></span> | <span data-ttu-id="1a1ba-324">60 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-324">60 minutes</span></span> |
|<span data-ttu-id="1a1ba-325">[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-325">[todoTask][]</span></span> | <span data-ttu-id="1a1ba-326">Менее 2 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-326">Less than 2 minutes</span></span> | <span data-ttu-id="1a1ba-327">15 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-327">15 minutes</span></span> |
|<span data-ttu-id="1a1ba-328">[user][]</span><span class="sxs-lookup"><span data-stu-id="1a1ba-328">[user][]</span></span> | <span data-ttu-id="1a1ba-329">Менее 2 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-329">Less than 2 minutes</span></span> | <span data-ttu-id="1a1ba-330">15 минут</span><span class="sxs-lookup"><span data-stu-id="1a1ba-330">15 minutes</span></span> |

><span data-ttu-id="1a1ba-331">**Примечание.** Задержка, предусматриваемая для ресурса **alert**, применяется только после создания самого оповещения.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-331">**Note:** The latency provided for the **alert** resource is only applicable after the alert itself has been created.</span></span> <span data-ttu-id="1a1ba-332">Она не включает в себя время, необходимое правилу для создания оповещения на основе данных.</span><span class="sxs-lookup"><span data-stu-id="1a1ba-332">It does not include the time it takes for a rule to create an alert from the data.</span></span>

## <a name="see-also"></a><span data-ttu-id="1a1ba-333">См. также</span><span class="sxs-lookup"><span data-stu-id="1a1ba-333">See also</span></span>

- [<span data-ttu-id="1a1ba-334">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="1a1ba-334">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true)
- [<span data-ttu-id="1a1ba-335">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="1a1ba-335">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0&preserve-view=true)
- [<span data-ttu-id="1a1ba-336">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="1a1ba-336">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0&preserve-view=true)
- <span data-ttu-id="1a1ba-337">Тип ресурса [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1a1ba-337">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta&preserve-view=true) resource type</span></span>
- <span data-ttu-id="1a1ba-338">Тип ресурса [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1a1ba-338">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta&preserve-view=true) resource type</span></span>
- [<span data-ttu-id="1a1ba-339">Руководство по уведомлениям об изменениях и отслеживанию изменений</span><span class="sxs-lookup"><span data-stu-id="1a1ba-339">Change notifications and change tracking tutorial</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)
- [<span data-ttu-id="1a1ba-340">Уведомления жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="1a1ba-340">Lifecycle notifications</span></span>](./webhooks-lifecycle.md)

[contact]: /graph/api/resources/contact
[conversation]: /graph/api/resources/conversation
[driveItem]: /graph/api/resources/driveitem
[event]: /graph/api/resources/event
[group]: /graph/api/resources/group
[message]: /graph/api/resources/message
[user]: /graph/api/resources/user
[alert]: /graph/api/resources/alert
[callRecord]: /graph/api/resources/callrecords-callrecord
[presence]: /graph/api/resources/presence
[chatMessage]: /graph/api/resources/chatmessage
[list]: /graph/api/resources/list
[printer]: /graph/api/resources/printer
[printTaskDefinition]: /graph/api/resources/printtaskdefinition
[todoTask]: /graph/api/resources/todotask
[channel]: /graph/api/resources/channel
[chat]: /graph/api/resources/chat
[conversationMember]: /graph/api/resources/conversationmember
[team]: /graph/api/resources/team
