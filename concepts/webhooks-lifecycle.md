---
title: Уменьшение количества пропущенных уведомлений о подписках и изменениях
description: У приложений, подписывающихся на уведомления об изменениях, могут быть удалены их подписки, что приводит к пропуску некоторых уведомлений об изменениях. В приложениях должна быть реализована логика определения потерь и восстановления после них, а также возобновления непрерывного потока уведомлений об изменениях.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 2c8cd8d38c0e089e98bc62aa37104b979f33ab9a
ms.sourcegitcommit: 70e09ebbf67f49a0c64ab7a275e751f8a68b8696
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/27/2020
ms.locfileid: "48771764"
---
# <a name="reduce-missing-subscriptions-and-change-notifications"></a><span data-ttu-id="1d8d5-104">Уменьшение количества пропущенных уведомлений о подписках и изменениях</span><span class="sxs-lookup"><span data-stu-id="1d8d5-104">Reduce missing subscriptions and change notifications</span></span>

<span data-ttu-id="1d8d5-105">У приложений, подписывающихся на уведомления об изменениях, могут быть удалены их подписки, что приводит к пропуску некоторых уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-105">Apps subscribing to change notifications might get their subscriptions removed and miss some change notifications.</span></span> <span data-ttu-id="1d8d5-106">В приложениях должна быть реализована логика определения потерь и восстановления после них, а также возобновления непрерывного потока уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-106">Apps should implement logic to detect and recover from the loss, and resume a continuous change notification flow.</span></span>

<span data-ttu-id="1d8d5-107">Некоторые события могут приводить к удалению подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-107">Certain events can cause a subscription to be removed.</span></span> <span data-ttu-id="1d8d5-108">К таким событиям относятся:</span><span class="sxs-lookup"><span data-stu-id="1d8d5-108">These events include:</span></span>

- <span data-ttu-id="1d8d5-109">сброс пароля пользователя;</span><span class="sxs-lookup"><span data-stu-id="1d8d5-109">User's password has been reset</span></span>
- <span data-ttu-id="1d8d5-110">устройство пользователя не соответствует требованиям;</span><span class="sxs-lookup"><span data-stu-id="1d8d5-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="1d8d5-111">учетная запись пользователя отозвана.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-111">User's account has been revoked</span></span>

<span data-ttu-id="1d8d5-112">В случае такого события Microsoft Graph отправляет специальное уведомление жизненного цикла `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-112">When such an event happens, Microsoft Graph sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="1d8d5-113">Microsoft Graph также отправляет другое уведомление жизненного цикла `missed`, если уведомление об изменении не может быть доставлено в приложение.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-113">Microsoft Graph also sends another lifecycle notification, `missed`, if a change notification cannot be delivered to an app.</span></span>

<span data-ttu-id="1d8d5-114">Приложение, подписывающееся на уведомления об изменениях, должно прослушивать сигналы `subscriptionRemoved` и `missed`, и выполнить следующее:</span><span class="sxs-lookup"><span data-stu-id="1d8d5-114">An app subscribing to change notifications should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="1d8d5-115">После получения уведомления жизненного цикла `subscriptionRemoved` приложение должно повторно создать подписку, чтобы поддерживать непрерывный поток.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-115">Upon receiving a `subscriptionRemoved` lifecycle notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="1d8d5-116">При получении уведомления жизненного цикла `missed` приложение должно повторно синхронизировать данные ресурсов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-116">On receiving a `missed` lifecycle notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="1d8d5-117">Чтобы получать уведомления жизненного цикла, можно использовать существующую конечную точку **notificationUrl** , которая уже получает уведомления об изменениях, или можно зарегистрировать отдельное свойство **lifecycleNotificationUrl** для получения уведомлений жизненного цикла `subscriptionRemoved` и `missed` в отдельной конечной точке.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives change notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` lifecycle notifications in a separate endpoint.</span></span>

<span data-ttu-id="1d8d5-118">Уведомления жизненного цикла поддерживаются для подписок, созданных в следующих типах ресурсов:</span><span class="sxs-lookup"><span data-stu-id="1d8d5-118">Lifecycle notifications are supported for subscriptions created on these resource types:</span></span>

- <span data-ttu-id="1d8d5-119">[Сообщение][] Outlook</span><span class="sxs-lookup"><span data-stu-id="1d8d5-119">Outlook [message][]</span></span>
- <span data-ttu-id="1d8d5-120">[Событие][] Outlook</span><span class="sxs-lookup"><span data-stu-id="1d8d5-120">Outlook [event][]</span></span>
- <span data-ttu-id="1d8d5-121">Личный [контакт][] Outlook</span><span class="sxs-lookup"><span data-stu-id="1d8d5-121">Outlook personal [contact][]</span></span>
- <span data-ttu-id="1d8d5-122">[chatMessage][] Teams</span><span class="sxs-lookup"><span data-stu-id="1d8d5-122">Teams [chatMessage][]</span></span>

<span data-ttu-id="1d8d5-123">Для других типов ресурсов вы по-прежнему можете указать `lifecycleNotificationUrl` при создании подписки, и ваше приложение будет получать уведомления жизненного цикла при применении их ресурсом.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-123">For other resource types, you may still provide a `lifecycleNotificationUrl` when creating the subscription and your application will receive lifecycle notifications whenver the resource implements it.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="1d8d5-124">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="1d8d5-124">Creating a subscription</span></span>

<span data-ttu-id="1d8d5-125">При создании подписки необходимо указать отдельную конечную точку уведомлений с помощью свойства **lifecycleNotificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-125">When creating a subscription, you must specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="1d8d5-126">Если указана конечная точка, все текущие и будущие типы уведомлений жизненного цикла будут доставляться в нее.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-126">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="1d8d5-127">В противном случае уведомления жизненного цикла `subscriptionRemoved` и `missed` доставляться не будут.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-127">Otherwise, `subscriptionRemoved` and `missed` lifecycle notifications will not be delivered.</span></span> <span data-ttu-id="1d8d5-128">Эта конечная точка может совпадать с **notificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-128">This endpoint can be the same as the **notificationUrl** .</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="1d8d5-129">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="1d8d5-129">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2020-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> [!IMPORTANT]
> <span data-ttu-id="1d8d5-130">Используйте одинаковое имя узла (FQDN) для обоих URL-адресов уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-130">Use the same hostname (FQDN) for both notifications URLs.</span></span> 

<span data-ttu-id="1d8d5-131">Вам нужно проверить обе конечные точки, как описано в статье [Управление подписками](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-131">You need to validate both endpoints, as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span> <span data-ttu-id="1d8d5-132">Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-132">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="1d8d5-133">**Примечание.** Вы не сможете обновить (`PATCH`) существующие подписки, чтобы добавить свойство **lifecycleNotificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-133">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="1d8d5-134">Следует удалить такие существующие подписки, создать новые подписки и указать свойство **lifecycleNotificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-134">You should remove such existing subscriptions, create new subscriptions, and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="1d8d5-135">Существующие подписки без свойства **lifecycleNotificationUrl** не будут получать уведомления `subscriptionRemoved` и `missed`.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-135">Existing subscriptions without a **lifecycleNotificationUrl** property will not receive the `subscriptionRemoved` and `missed` notifications.</span></span>

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="1d8d5-136">Ответ на уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="1d8d5-136">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="1d8d5-137">Уведомление жизненного цикла `subscriptionRemoved` информирует, что подписка была удалена и следует создать ее заново, если вы хотите продолжать получение уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-137">The `subscriptionRemoved` lifecycle notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving change notifications.</span></span> 

<span data-ttu-id="1d8d5-138">Вы можете создавать длительные подписки (на 3 дня), а уведомления об изменениях начнут поступать в **notificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-138">You can create a long-lived subscription (3 days), and change notifications will start flowing to the **notificationUrl** .</span></span> <span data-ttu-id="1d8d5-139">Однако условия доступа к данным ресурса могут со временем измениться.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-139">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="1d8d5-140">Например, в службе может произойти событие, требующее от приложения повторной проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-140">For example, an event in the service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="1d8d5-141">В таком случае поток выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="1d8d5-141">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="1d8d5-142">Служба определяет, что подписка должна быть удалена из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-142">The service detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="1d8d5-143">Для этих событий отсутствует заданная периодичность.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-143">There is no set cadence for these events.</span></span> <span data-ttu-id="1d8d5-144">Для одних ресурсов они могут происходить часто, а для других — практически никогда.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-144">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="1d8d5-145">Microsoft Graph отправляет уведомление жизненного цикла `subscriptionRemoved` для **lifecycleNotificationUrl** (если указано).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-145">Microsoft Graph sends a `subscriptionRemoved` lifecycle notification to the **lifecycleNotificationUrl** (if specified).</span></span>  

3. <span data-ttu-id="1d8d5-146">Вы можете ответить на это уведомление жизненного цикла, создав новую подписку для того же ресурса.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-146">You can respond to this lifecycle notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="1d8d5-147">Для этого нужно представить допустимый маркер доступа; в некоторых случаях это означает, что приложению необходимо выполнить повторную проверку подлинности пользователя, чтобы получить новый допустимый маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-147">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="1d8d5-148">Если вы успешно создали новую подписку, возобновится поток уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-148">If you successfully create a new subscription, change notifications will start flowing again.</span></span> <span data-ttu-id="1d8d5-149">Но если вам не удалось это сделать (например, приложение не может получить допустимый маркер доступа), уведомления об изменениях не отправляются.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-149">However, if you fail (for example, the app can't obtain a valid access token), change notifications will not be sent.</span></span>

5. <span data-ttu-id="1d8d5-150">Создав новую подписку, вы можете синхронизировать данные ресурсов, чтобы выявить все отсутствующие изменения.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-150">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="1d8d5-151">Пример уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="1d8d5-151">subscriptionRemoved notification example</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "subscriptionRemoved"
    }
  ]
}
```

<span data-ttu-id="1d8d5-152">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-152">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="1d8d5-153">Поле `"lifecycleEvent": "subscriptionRemoved"` определяет это уведомление, как связанное с удалением подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-153">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="1d8d5-154">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-154">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="1d8d5-155">Это уведомление жизненного цикла не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-155">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="1d8d5-156">Как и уведомления об изменениях, уведомления жизненного цикла могут объединяться (в массиве **value** ), каждое с возможно разными значениями **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-156">Similar to change notifications, lifecycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="1d8d5-157">Обрабатывайте каждое уведомление жизненного цикла в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-157">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="1d8d5-158">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-158">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="1d8d5-159">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="1d8d5-159">Actions to take</span></span>

1. <span data-ttu-id="1d8d5-160">[Подтвердите](webhooks.md#change-notifications) получение уведомления жизненного цикла, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-160">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="1d8d5-161">[Проверьте](webhooks.md#change-notifications) подлинность уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-161">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="1d8d5-162">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-162">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="1d8d5-163">**Примечание.** Если вы используете одну из [библиотек проверки подлинности](/azure/active-directory/develop/reference-v2-libraries), они сделают это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, а также попросив пользователя войти еще раз (с помощью нового пароля).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-163">**Note:** If you're using one of the [authentication libraries](/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="1d8d5-164">Обратите внимание, что получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и вызывающей стороне больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-164">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="1d8d5-165">Создайте новую подписку с помощью стандартного процесса, описанного [здесь](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-165">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="1d8d5-166">**Примечание.** Это действие может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-166">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="1d8d5-167">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-167">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="1d8d5-168">Вы можете повторить эти действия позднее в любое время, например, когда изменятся условия доступа.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-168">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="1d8d5-169">Все изменения ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-169">Any resource changes in the time period from when the lifecycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="1d8d5-170">Приложению потребуется получить эти изменения самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-170">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="1d8d5-171">После создания новой подписки синхронизируйте все отсутствующие данные ресурсов с последнего известного момента получения уведомления об изменении для этого ресурса. Например: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="1d8d5-171">After creating the new subscription, sync any missing resource data from the last known time you received a change notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="1d8d5-172">Реагирование на пропущенные уведомления</span><span class="sxs-lookup"><span data-stu-id="1d8d5-172">Responding to missed notifications</span></span>

<span data-ttu-id="1d8d5-173">Эти сигналы сообщают, что некоторые уведомления об изменениях могли быть не доставлены.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-173">These signals inform you that some change notifications might not have been delivered.</span></span> <span data-ttu-id="1d8d5-174">Вам следует решить, пропустить или обработать эти сигналы.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-174">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="1d8d5-175">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="1d8d5-175">Notification example</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "missed"
    }
  ]
}
```

<span data-ttu-id="1d8d5-176">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-176">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="1d8d5-177">Поле `"lifecycleEvent": "missed"` определяет это в качестве сигнала о пропущенных уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-177">The `"lifecycleEvent": "missed"` field designates this as a signal about missed change notifications.</span></span> <span data-ttu-id="1d8d5-178">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-178">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="1d8d5-179">Это уведомление жизненного цикла не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-179">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="1d8d5-180">Как и уведомления об изменениях, уведомления жизненного цикла могут объединяться (в массиве **value** ), каждое с возможно разными значениями **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-180">Similar to change notifications, lifecycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="1d8d5-181">Обрабатывайте каждое уведомление жизненного цикла в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-181">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="1d8d5-182">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-182">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="1d8d5-183">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="1d8d5-183">Actions to take</span></span>

1. <span data-ttu-id="1d8d5-184">[Подтвердите](webhooks.md#change-notifications) получение уведомления жизненного цикла, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-184">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="1d8d5-185">Если вы игнорируете эти сигналы, не выполняйте других действий.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-185">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="1d8d5-186">В противном случае:</span><span class="sxs-lookup"><span data-stu-id="1d8d5-186">Otherwise:</span></span>
2. <span data-ttu-id="1d8d5-187">[Проверьте](webhooks.md#change-notifications) подлинность уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-187">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="1d8d5-188">Выполните полную повторную синхронизацию данных ресурса для выявления изменений, не доставленных в качестве уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-188">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 

## <a name="responding-to-reauthorizationrequired-notifications"></a><span data-ttu-id="1d8d5-189">Реагирование на уведомления reauthorizationRequired</span><span class="sxs-lookup"><span data-stu-id="1d8d5-189">Responding to reauthorizationRequired notifications</span></span>

<span data-ttu-id="1d8d5-190">Получив уведомление о жизненном цикле `reauthorizationRequired`, необходимо выполнить повторную авторизацию подписки, чтобы поток данных не прекращался.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-190">When you receive a `reauthorizationRequired` lifecycle notification, you must reauthorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="1d8d5-191">Вы можете создавать длительные подписки (на 3 дня), таким образом уведомления об изменениях начнут поступать в **notificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-191">You can create a long-lived subscription (3 days), which enables change notifications to flow to the **notificationUrl** .</span></span> <span data-ttu-id="1d8d5-192">В случае изменений в условия доступа Microsoft Graph может потребовать повторную авторизацию подписки, чтобы подтвердить наличие у вас доступа к данным ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-192">If the conditions of access have changed since the subscription was created, Microsoft Graph may require that you reauthorize the subscription to prove that you still have access to resource data.</span></span> <span data-ttu-id="1d8d5-193">Ниже приведены примеры изменений, влияющих на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-193">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="1d8d5-194">Администратор клиента может отозвать разрешения приложения на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-194">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="1d8d5-195">В интерактивном сценарии к пользователю, предоставляющему маркер проверки подлинности для вашего приложения, могут применяться динамические политики на основе различных факторов, например их расположения, состояния устройства или оценки риска.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-195">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="1d8d5-196">Например, если пользователь изменяет свое физическое расположение, ему может быть запрещен доступ к данным, и ваше приложение не сможет повторно авторизовать подписку.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-196">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to reauthorize the subscription.</span></span> <span data-ttu-id="1d8d5-197">Дополнительные сведения о динамических политиках, управляющих доступом, см. в статье [Политики условного доступа Azure AD](/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-197">For more information about dynamic policies that control access, see [Azure AD conditional access policies](/azure/active-directory/conditional-access/overview).</span></span> 

<span data-ttu-id="1d8d5-198">Ниже указаны шаги, которые представляют собой поток запроса авторизации для активной подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-198">The following steps represent the flow of an authorization challenge for an active subscription:</span></span>

1. <span data-ttu-id="1d8d5-199">Microsoft Graph требует повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-199">Microsoft Graph requires a subscription to be reauthorized.</span></span>
    
    <span data-ttu-id="1d8d5-200">Причины этого могут отличаться для разных ресурсов и меняться со временем.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-200">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="1d8d5-201">Необходимо ответить на событие повторной авторизации независимо от его причины.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-201">You must respond to a reauthorization event no matter what caused it.</span></span>

2. <span data-ttu-id="1d8d5-202">Microsoft Graph отправляет уведомление о запросе авторизации в **lifecycleNotificationUrl**</span><span class="sxs-lookup"><span data-stu-id="1d8d5-202">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl** .</span></span>

    <span data-ttu-id="1d8d5-203">Обратите внимание, что поток уведомлений об изменениях может некоторое время продолжаться, предоставляя вам дополнительное время для ответа.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-203">Note that the flow of change notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="1d8d5-204">Однако в конечном итоге доставка уведомлений об изменениях приостанавливается, пока вы не выполните требуемое действие.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-204">However, eventually change notification delivery pauses, until you take the required action.</span></span>

3. <span data-ttu-id="1d8d5-205">Ответьте на это уведомление жизненного цикла одним из указанных ниже двух способов.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-205">Respond to this lifecycle notification in one of two ways:</span></span>
    - <span data-ttu-id="1d8d5-206">Повторная авторизация подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-206">Reauthorize the subscription.</span></span> <span data-ttu-id="1d8d5-207">Это не продлевает срок действия подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-207">This does not extend the expiry date of the subscription.</span></span>
    - <span data-ttu-id="1d8d5-208">Возобновление подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-208">Renew the subscription.</span></span> <span data-ttu-id="1d8d5-209">Это повторно авторизует подписку и продлевает срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-209">This both reauthorizes and extends the expiry date.</span></span>

    <span data-ttu-id="1d8d5-210">Примечание. Оба действия требуют предоставление действительного маркера проверки подлинности по аналогии с [созданием новой подписки](webhooks.md#creating-a-subscription) или [продлением подписки до истечения срока ее действия](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-210">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="1d8d5-211">Если вы успешно выполнили повторную авторизацию или возобновление подписки, уведомления об изменениях продолжать поступать.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-211">If you successfully reauthorize or renew the subscription, change notifications continue.</span></span> <span data-ttu-id="1d8d5-212">В противном случае уведомления об изменениях не будут возобновлены.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-212">Otherwise, change notifications remain paused.</span></span>

### <a name="reauthorizationrequired-notification-example"></a><span data-ttu-id="1d8d5-213">Пример уведомления reauthorizationRequired</span><span class="sxs-lookup"><span data-stu-id="1d8d5-213">reauthorizationRequired notification example</span></span>

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

<span data-ttu-id="1d8d5-214">Обратите внимание на указанные ниже моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-214">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="1d8d5-215">Поле `"lifecycleEvent": "reauthorizationRequired"` назначает это уведомление запросом на авторизацию.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-215">The `"lifecycleEvent": "reauthorizationRequired"` field designates this notification as an authorization challenge.</span></span> <span data-ttu-id="1d8d5-216">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-216">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="1d8d5-217">Это уведомление жизненного цикла не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-217">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="1d8d5-218">Как и уведомления об изменениях, уведомления жизненного цикла можно объединять (в коллекции **value** ), каждое с возможно разными значениями **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-218">Similar to change notifications, you can batch lifecycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="1d8d5-219">Обрабатывайте каждое уведомление жизненного цикла в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-219">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="1d8d5-220">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-220">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="1d8d5-221">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="1d8d5-221">Actions to take</span></span>

1. <span data-ttu-id="1d8d5-222">[Подтвердите](webhooks.md#change-notifications) получение уведомления жизненного цикла, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-222">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="1d8d5-223">[Проверьте](webhooks.md#change-notifications) подлинность уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-223">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="1d8d5-224">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-224">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="1d8d5-225">**Примечание.** Если вы используете одну из [библиотек проверки подлинности](/azure/active-directory/develop/reference-v2-libraries), они сделают это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, а также попросив пользователя войти еще раз (с помощью нового пароля).</span><span class="sxs-lookup"><span data-stu-id="1d8d5-225">**Note:** If you're using one of the [authentication libraries](/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="1d8d5-226">Обратите внимание, что получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и вызывающей стороне больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-226">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="1d8d5-227">Вызовите один из двух следующих API.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-227">Call either of the following two APIs.</span></span> <span data-ttu-id="1d8d5-228">Если вызов API выполняется успешно, поток уведомлений об изменениях возобновляется.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-228">If the API call succeeds, the change notification flow resumes.</span></span>

    - <span data-ttu-id="1d8d5-229">Чтобы повторно авторизовать подписку без продления ее срока, вызовите действие `/reauthorize`:</span><span class="sxs-lookup"><span data-stu-id="1d8d5-229">Call the `/reauthorize` action to reauthorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="1d8d5-230">Чтобы одновременно возобновить и повторно авторизовать подписку, выполните обычное действие возобновления:</span><span class="sxs-lookup"><span data-stu-id="1d8d5-230">Perform a regular renew action to reauthorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="1d8d5-231">Возобновление может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-231">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="1d8d5-232">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-232">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> 
      
      <span data-ttu-id="1d8d5-233">Вы может повторить эти действия позднее в любое время и успешно выполнить их, если изменяются условия доступа.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-233">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="1d8d5-234">Все уведомления об изменении ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-234">Any notifications about resource changes that happen between the time the lifecycle notification was sent and the time when the app successfully creates the subscription again, would be lost.</span></span> <span data-ttu-id="1d8d5-235">В таких случаях приложению нужно отдельно получить эти изменения.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-235">In such cases, the app should separately fetch those changes.</span></span>

### <a name="additional-information"></a><span data-ttu-id="1d8d5-236">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="1d8d5-236">Additional information</span></span>

<span data-ttu-id="1d8d5-237">Ниже приведены сведения, которые помогут разобраться с проблемами авторизации.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-237">The following information can help you understand authorization challenges:</span></span>

- <span data-ttu-id="1d8d5-238">Запросы авторизации не отменяют необходимость возобновления подписки на изменения ресурса до истечения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-238">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="1d8d5-239">Хотя вы можете возобновить подписку при получении запроса авторизации, Microsoft Graph может не выполнять запрос для всех ваших подписок.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-239">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="1d8d5-240">Например, подписка без действий и уведомлений об изменениях, ожидающих доставки, может не создавать для приложения запросы на повторную авторизацию.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-240">For example, a subscription that does not have any activity and has no change notifications pending delivery may not signal any reauthorization challenges to your app.</span></span> <span data-ttu-id="1d8d5-241">Обязательно [возобновите подписки](webhooks.md#renewing-a-subscription) до истечения их сроков действия.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-241">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

- <span data-ttu-id="1d8d5-242">Частота запросов авторизации может изменяться.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-242">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="1d8d5-243">Не делайте предположений о частоте запросов авторизации.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-243">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="1d8d5-244">Эти уведомления жизненного цикла сообщают, когда нужно принимать действия, избавляя от отслеживания подписок, которым требуется повторная авторизация.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-244">These lifecycle notifications tell you when to take actions, saving you from having to track which subscriptions require reauthorization.</span></span> <span data-ttu-id="1d8d5-245">Будьте готовы обрабатывать запросы авторизации каждые несколько минут для всех подписок или в редких случаях лишь для некоторых своих подписок.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-245">Be ready to handle authorization challenges from once every few minutes for every subscription to rarely for only some of your subscriptions.</span></span>

## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="1d8d5-246">Готовый к изменениям код обработки уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="1d8d5-246">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="1d8d5-247">В будущем в Microsoft Graph будут добавлены другие типы уведомлений жизненного цикла подписки.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-247">In the future, Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="1d8d5-248">Они будут публиковаться в той же конечной точке: **lifecycleNotificationUrl** , но у них будет другое значение для **lifecycleEvent** , и они могут содержать немного другую схему и свойства, относящиеся к сценарию, для которого они создаются.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-248">They will be posted to the same endpoint: **lifecycleNotificationUrl** , but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="1d8d5-249">Следует реализовать свой код с готовностью к будущим изменениям, чтобы он не прерывался, когда в Microsoft Graph вводятся новые типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-249">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="1d8d5-250">Мы рекомендуем следующий подход:</span><span class="sxs-lookup"><span data-stu-id="1d8d5-250">We recommend the following approach:</span></span>

1. <span data-ttu-id="1d8d5-251">Явным образом определите каждое уведомление жизненного цикла как поддерживаемое событие с помощью свойства **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="1d8d5-251">Explicitly identify each lifecycle notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="1d8d5-252">Например, найдите свойство `"lifecycleEvent": "subscriptionRemoved"` для определения конкретного события и обработайте его.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-252">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="1d8d5-253">Обратите внимание на объявления уведомлений жизненного цикла о новых сценариях.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-253">Watch for announcements of lifecycle notifications for new scenarions.</span></span> <span data-ttu-id="1d8d5-254">В будущем могут быть доступны и другие типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-254">There might be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="1d8d5-255">В своем приложении игнорируйте любые уведомления жизненного цикла, не распознаваемые приложением, и заносите их в журнал для ознакомления.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-255">In your app, ignore any lifecycle notification that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="1d8d5-256">По своему усмотрению просматривайте соответствующую документацию о новых уведомлениях жизненного цикла и реализуйте для них нужную поддержку.</span><span class="sxs-lookup"><span data-stu-id="1d8d5-256">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="1d8d5-257">См. также</span><span class="sxs-lookup"><span data-stu-id="1d8d5-257">See also</span></span>

- [<span data-ttu-id="1d8d5-258">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="1d8d5-258">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="1d8d5-259">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="1d8d5-259">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="1d8d5-260">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="1d8d5-260">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="1d8d5-261">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="1d8d5-261">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="1d8d5-262">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="1d8d5-262">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)


[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
