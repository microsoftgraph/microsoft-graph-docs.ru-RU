---
title: Уменьшение числа пропущенных подписок и уведомлений о ресурсах Outlook (предварительная версия)
description: Outlook может приостановить доставку уведомлений об изменениях из-за событий безопасности, например сброса пароля пользователя. Для обеспечения непрерывной доставки уведомлений необходимо обрабатывать специальные события жизненного цикла (`subscriptionRemoved` и `missed`).
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 481dbee58a5ee761816e05c88d44e115da736035
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216842"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a><span data-ttu-id="65ded-104">Уменьшение числа пропущенных подписок и уведомлений о ресурсах Outlook (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="65ded-104">Reduce missing subscriptions and notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="65ded-105">У приложений, подписывающихся на уведомления о ресурсах Outlook, могут быть удалены их подписки, что приводит к пропуску некоторых уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65ded-105">Apps subscribing to notifications for Outlook resources might get their subscriptions removed and miss some notifications.</span></span> <span data-ttu-id="65ded-106">В приложениях должна быть реализована логика определения потерь и восстановления после них, а также возобновления непрерывного потока уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65ded-106">Apps should implement logic to detect and recover from the loss, and resume a continuous notification flow.</span></span>

<span data-ttu-id="65ded-107">Некоторые события в Outlook могут приводить к удалению подписки.</span><span class="sxs-lookup"><span data-stu-id="65ded-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="65ded-108">К таким событиям относятся:</span><span class="sxs-lookup"><span data-stu-id="65ded-108">These events include:</span></span>

- <span data-ttu-id="65ded-109">сброс пароля пользователя;</span><span class="sxs-lookup"><span data-stu-id="65ded-109">User's password has been reset</span></span>
- <span data-ttu-id="65ded-110">устройство пользователя не соответствует требованиям;</span><span class="sxs-lookup"><span data-stu-id="65ded-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="65ded-111">учетная запись пользователя отозвана.</span><span class="sxs-lookup"><span data-stu-id="65ded-111">User's account has been revoked</span></span>

<span data-ttu-id="65ded-112">В случае такого события Outlook отправляет специальное уведомление жизненного цикла, `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="65ded-112">When such an event happens, Outlook sends a special life cycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="65ded-113">Outlook также отправляет другое уведомление жизненного цикла, `missed`, если уведомление не может быть доставлено в приложение.</span><span class="sxs-lookup"><span data-stu-id="65ded-113">Outlook also sends another life cycle notification, `missed`, if a notification cannot be delivered to an app.</span></span>

<span data-ttu-id="65ded-114">Приложение, подписывающееся на уведомления о ресурсах Outlook, таких как **message** и **event**, должно прослушивать сигналы `subscriptionRemoved` и `missed`, и выполнить следующее:</span><span class="sxs-lookup"><span data-stu-id="65ded-114">An app subscribing to notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="65ded-115">После получения уведомления `subscriptionRemoved` приложение должно повторно создать подписку, чтобы поддерживать непрерывный поток.</span><span class="sxs-lookup"><span data-stu-id="65ded-115">Upon receiving a `subscriptionRemoved` notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="65ded-116">При получении уведомления `missed` приложение должно повторно синхронизировать данные ресурсов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65ded-116">On receiving a `missed` notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="65ded-117">Чтобы получать уведомления жизненного цикла, можно использовать существующую конечную точку **notificationUrl**, которая уже получает уведомления о ресурсе, или можно зарегистрировать отдельное свойство **lifecycleNotificationUrl** для получения уведомлений `subscriptionRemoved` и `missed` в отдельной конечной точке.</span><span class="sxs-lookup"><span data-stu-id="65ded-117">To receive life cycle notifications, you can use the existing **notificationUrl** endpoint that already receives resource notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="65ded-118">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="65ded-118">Creating a subscription</span></span>

<span data-ttu-id="65ded-119">При создании подписки вы можете указать отдельную конечную точку уведомлений с помощью свойства **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="65ded-119">When creating a subscription, you can specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="65ded-120">Если указана конечная точка, все текущие и будущие типы уведомлений жизненного цикла будут доставляться в нее.</span><span class="sxs-lookup"><span data-stu-id="65ded-120">If you specify the endpoint, all current and future types of life cycle notifications will be delivered there.</span></span> <span data-ttu-id="65ded-121">В противном случае уведомления `subscriptionRemoved` и `missed` будут доставляться в существующую конечную точку **notificationUrl** для всех существующих подписок.</span><span class="sxs-lookup"><span data-stu-id="65ded-121">Otherwise, `subscriptionRemoved` and `missed` notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="65ded-122">**Примечание.** Свойство **lifecycleNotificationUrl** можно настроить или считать только с помощью интерфейсов API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65ded-122">**Note:** The **lifecycleNotificationUrl** property can only be set or read using Microsoft Graph beta APIs.</span></span> <span data-ttu-id="65ded-123">Однако подписки, созданные с помощью бета-версий API, хранятся в той же рабочей среде, что и подписки, созданные с помощью версии 1.0, поэтому можно реализовать новый поток Outlook в дополнение к вашим подпискам, создаваемым с помощью версии API 1.0.</span><span class="sxs-lookup"><span data-stu-id="65ded-123">However, subscriptions created using beta APIs are stored in the same production environment as those created using v1.0, so you can implement the new Outlook flow in addition to your subscriptions creating using v1.0 APIs.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="65ded-124">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="65ded-124">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2019-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> <span data-ttu-id="65ded-125">**Важно!** Используйте одинаковое имя узла для обоих URL-адресов уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65ded-125">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="65ded-126">**Примечание.** Вам нужно проверить обе конечные точки уведомлений, как описано в статье [Управление подписками](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="65ded-126">**Note:** You need to validate both notification endpoints as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="65ded-127">Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.</span><span class="sxs-lookup"><span data-stu-id="65ded-127">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="65ded-128">**Примечание.** Вы не сможете обновить (`PATCH`) существующие подписки, чтобы добавить свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="65ded-128">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="65ded-129">Следует удалить такие существующие подписки, создать новые подписки и указать свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="65ded-129">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="65ded-130">Существующие подписки без свойства **lifecycleNotificationUrl** получают уведомления `subscriptionRemoved` и `missed` через **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="65ded-130">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="65ded-131">Ответ на уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="65ded-131">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="65ded-132">Уведомление `subscriptionRemoved` информирует, что подписка была удалена и следует создать ее заново, если вы хотите продолжать получение уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65ded-132">The `subscriptionRemoved` notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving notifications.</span></span> 

<span data-ttu-id="65ded-133">Вы можете создавать длительные подписки (на 3 дня), а уведомления о данных ресурса начнут поступать в **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="65ded-133">You can create a long-lived subscription (3 days), and resource data notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="65ded-134">Однако условия доступа к данным ресурса могут со временем измениться.</span><span class="sxs-lookup"><span data-stu-id="65ded-134">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="65ded-135">Например, в службе Outlook может произойти событие, требующее от приложения повторной проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="65ded-135">For example, an event in the Outlook service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="65ded-136">В таком случае поток выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="65ded-136">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="65ded-137">Outlook определяет, что подписка должна быть удалена из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65ded-137">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="65ded-138">Для этих событий отсутствует заданная периодичность.</span><span class="sxs-lookup"><span data-stu-id="65ded-138">There is no set cadence for these events.</span></span> <span data-ttu-id="65ded-139">Для одних ресурсов они могут происходить часто, а для других — практически никогда.</span><span class="sxs-lookup"><span data-stu-id="65ded-139">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="65ded-140">Microsoft Graph отправляет уведомление `subscriptionRemoved` для **lifecycleNotificationUrl** (если указано) или **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="65ded-140">Microsoft Graph sends a `subscriptionRemoved` notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="65ded-141">Вы можете ответить на это уведомление, создав новую подписку для того же ресурса.</span><span class="sxs-lookup"><span data-stu-id="65ded-141">You can respond to this notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="65ded-142">Для этого нужно представить допустимый маркер доступа; в некоторых случаях это означает, что приложению необходимо выполнить повторную проверку подлинности пользователя, чтобы получить новый допустимый маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="65ded-142">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="65ded-143">Если вы успешно создали новую подписку, возобновится поток уведомлений о ресурсах.</span><span class="sxs-lookup"><span data-stu-id="65ded-143">If you successfully create a new subscription, resource notifications will start flowing again.</span></span> <span data-ttu-id="65ded-144">Но если вам не удалось это сделать (например, приложение не может получить допустимый маркер доступа), уведомления о ресурсах не отправляются.</span><span class="sxs-lookup"><span data-stu-id="65ded-144">However, if you fail (for example, the app can't obtain a valid access token), resource notifications will not be sent.</span></span>

5. <span data-ttu-id="65ded-145">Создав новую подписку, вы можете синхронизировать данные ресурсов, чтобы выявить все отсутствующие изменения.</span><span class="sxs-lookup"><span data-stu-id="65ded-145">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="65ded-146">Пример уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="65ded-146">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="65ded-147">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="65ded-147">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="65ded-148">Поле `"lifecycleEvent": "subscriptionRemoved"` определяет это уведомление, как связанное с удалением подписки.</span><span class="sxs-lookup"><span data-stu-id="65ded-148">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="65ded-149">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="65ded-149">Other types of life cycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="65ded-150">Это уведомление не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="65ded-150">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="65ded-151">Как и уведомления о ресурсах, уведомления жизненного цикла могут объединяться (в массиве **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="65ded-151">Similar to resource notifications, life cycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="65ded-152">Обрабатывайте каждое уведомление в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="65ded-152">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="65ded-153">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="65ded-153">Actions to take</span></span>

1. <span data-ttu-id="65ded-154">[Подтвердите](webhooks.md#notifications) получение уведомления, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="65ded-154">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="65ded-155">[Проверьте](webhooks.md#notifications) подлинность уведомления.</span><span class="sxs-lookup"><span data-stu-id="65ded-155">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="65ded-156">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="65ded-156">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="65ded-157">**Примечание.** Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), они сделают это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, а также попросив пользователя войти еще раз (с помощью нового пароля).</span><span class="sxs-lookup"><span data-stu-id="65ded-157">**Note:** If you're using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="65ded-158">Обратите внимание, что получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и вызывающей стороне больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="65ded-158">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="65ded-159">Создайте новую подписку с помощью стандартного процесса, описанного [здесь](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="65ded-159">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="65ded-160">**Примечание.** Это действие может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="65ded-160">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="65ded-161">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="65ded-161">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="65ded-162">Вы можете повторить эти действия позднее в любое время, например, когда изменятся условия доступа.</span><span class="sxs-lookup"><span data-stu-id="65ded-162">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="65ded-163">Все изменения ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="65ded-163">Any resource changes in the time period from when the life cycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="65ded-164">Приложению потребуется получить эти изменения самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="65ded-164">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="65ded-165">После создания новой подписки синхронизируйте все отсутствующие данные ресурсов с последнего известного момента получения уведомления об этом ресурсе. Например: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="65ded-165">After creating the new subscription, sync any missing resource data from the last known time you received a notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="65ded-166">Реагирование на пропущенные уведомления</span><span class="sxs-lookup"><span data-stu-id="65ded-166">Responding to missed notifications</span></span>

<span data-ttu-id="65ded-167">Эти сигналы сообщают, что некоторые уведомления могли быть не доставлены.</span><span class="sxs-lookup"><span data-stu-id="65ded-167">These signals inform you that some notifications might not have been delivered.</span></span> <span data-ttu-id="65ded-168">Вам следует решить, пропустить или обработать эти сигналы.</span><span class="sxs-lookup"><span data-stu-id="65ded-168">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="65ded-169">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="65ded-169">Notification example</span></span>

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

<span data-ttu-id="65ded-170">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="65ded-170">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="65ded-171">Поле `"lifecycleEvent": "missed"` определяет это в качестве сигнала о пропущенных уведомлениях.</span><span class="sxs-lookup"><span data-stu-id="65ded-171">The `"lifecycleEvent": "missed"` field designates this as a signal about missed notifications.</span></span> <span data-ttu-id="65ded-172">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="65ded-172">Other types of life cycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="65ded-173">Это уведомление не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="65ded-173">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="65ded-174">Как и уведомления о ресурсах, уведомления жизненного цикла могут объединяться (в массиве **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="65ded-174">Similar to resource notifications, life cycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="65ded-175">Обрабатывайте каждое уведомление в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="65ded-175">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="65ded-176">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="65ded-176">Actions to take</span></span>

1. <span data-ttu-id="65ded-177">[Подтвердите](webhooks.md#notifications) получение уведомления, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="65ded-177">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="65ded-178">Если вы игнорируете эти сигналы, не выполняйте других действий.</span><span class="sxs-lookup"><span data-stu-id="65ded-178">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="65ded-179">В противном случае:</span><span class="sxs-lookup"><span data-stu-id="65ded-179">Otherwise:</span></span>
2. <span data-ttu-id="65ded-180">[Проверьте](webhooks.md#notifications) подлинность уведомления.</span><span class="sxs-lookup"><span data-stu-id="65ded-180">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="65ded-181">Выполните полную повторную синхронизацию данных ресурса для выявления изменений, не доставленных в качестве уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65ded-181">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-life-cycle-notifications"></a><span data-ttu-id="65ded-182">Готовый к изменениям код обработки уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="65ded-182">Future-proof the code handling life cycle notifications</span></span>

<span data-ttu-id="65ded-183">В будущем в Microsoft Graph будут добавлены другие типы уведомлений жизненного цикла подписки.</span><span class="sxs-lookup"><span data-stu-id="65ded-183">In the future, Microsoft Graph will add more types of subscription life cycle notifications.</span></span> <span data-ttu-id="65ded-184">Они будут публиковаться в той же конечной точке: **lifecycleNotificationUrl**, но у них будет другое значение для **lifecycleEvent**, и они могут содержать немного другую схему и свойства, относящиеся к сценарию, для которого они создаются.</span><span class="sxs-lookup"><span data-stu-id="65ded-184">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="65ded-185">Следует реализовать свой код с готовностью к будущим изменениям, чтобы он не прерывался, когда в Microsoft Graph вводятся новые типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="65ded-185">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of life cycle notifications.</span></span> <span data-ttu-id="65ded-186">Мы рекомендуем следующий подход:</span><span class="sxs-lookup"><span data-stu-id="65ded-186">We recommend the following approach:</span></span>

1. <span data-ttu-id="65ded-187">Явным образом определите каждое уведомление как поддерживаемое событие с помощью свойства **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="65ded-187">Explicitly identify each notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="65ded-188">Например, найдите свойство `"lifecycleEvent": "subscriptionRemoved"` для определения конкретного события и обработайте его.</span><span class="sxs-lookup"><span data-stu-id="65ded-188">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="65ded-189">Обратите внимание на объявления о новых сценариях.</span><span class="sxs-lookup"><span data-stu-id="65ded-189">Watch for announcements of notifications for new scenarions.</span></span> <span data-ttu-id="65ded-190">В будущем могут быть доступны и другие типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="65ded-190">There might be more types of life cycle notifications in the future.</span></span>

3. <span data-ttu-id="65ded-191">В своем приложении игнорируйте любые события жизненного цикла, не распознаваемые приложением, и заносите их в журнал для ознакомления.</span><span class="sxs-lookup"><span data-stu-id="65ded-191">In your app, ignore any life cycle events that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="65ded-192">По своему усмотрению просматривайте соответствующую документацию о новых уведомлениях жизненного цикла и реализуйте для них нужную поддержку.</span><span class="sxs-lookup"><span data-stu-id="65ded-192">At your discretion, look up the related documentation for new life cycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="65ded-193">См. также</span><span class="sxs-lookup"><span data-stu-id="65ded-193">See also</span></span>

- [<span data-ttu-id="65ded-194">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="65ded-194">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="65ded-195">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="65ded-195">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="65ded-196">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="65ded-196">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="65ded-197">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="65ded-197">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="65ded-198">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="65ded-198">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
