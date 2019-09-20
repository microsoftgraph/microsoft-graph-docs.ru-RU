---
title: Уменьшение числа пропущенных подписок и уведомлений о ресурсах Outlook (предварительная версия)
description: Outlook может приостановить доставку уведомлений об изменениях из-за событий безопасности, например сброса пароля пользователя. Для обеспечения непрерывной доставки уведомлений необходимо обрабатывать специальные события жизненного цикла (`subscriptionRemoved` и `missed`).
author: piotrci
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7880216eedb6fa8757ca6e027bf2395dea516073
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053934"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a><span data-ttu-id="f6d37-104">Уменьшение числа пропущенных подписок и уведомлений о ресурсах Outlook (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f6d37-104">Reduce missing subscriptions and notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="f6d37-105">У приложений, подписывающихся на уведомления о ресурсах Outlook, могут быть удалены их подписки, что приводит к пропуску некоторых уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f6d37-105">Apps subscribing to notifications for Outlook resources may get their subscriptions removed and miss some notifications.</span></span> <span data-ttu-id="f6d37-106">В приложениях должна быть реализована логика определения потерь и восстановления после них, а также возобновления непрерывного потока уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f6d37-106">Apps should implement logic to detect and recover from the loss, and resume a continuous notification flow.</span></span>

<span data-ttu-id="f6d37-107">Некоторые события в Outlook могут приводить к удалению подписки.</span><span class="sxs-lookup"><span data-stu-id="f6d37-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="f6d37-108">К таким событиям относятся:</span><span class="sxs-lookup"><span data-stu-id="f6d37-108">These events include:</span></span>

- <span data-ttu-id="f6d37-109">сброс пароля пользователя;</span><span class="sxs-lookup"><span data-stu-id="f6d37-109">User's password has been reset</span></span>
- <span data-ttu-id="f6d37-110">устройство пользователя не соответствует требованиям;</span><span class="sxs-lookup"><span data-stu-id="f6d37-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="f6d37-111">учетная запись пользователя отозвана.</span><span class="sxs-lookup"><span data-stu-id="f6d37-111">User's account has been revoked</span></span>

<span data-ttu-id="f6d37-112">В случае такого события Outlook отправляет специальное уведомление жизненного цикла `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="f6d37-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="f6d37-113">Outlook также отправляет другое уведомление жизненного цикла `missed`, если уведомление не может быть доставлено в приложение.</span><span class="sxs-lookup"><span data-stu-id="f6d37-113">Outlook also sends another lifecycle notification, `missed`, if a notification cannot be delivered to an app.</span></span>

<span data-ttu-id="f6d37-114">Приложение, подписывающееся на уведомления о ресурсах Outlook, таких как **message** и **event**, должно прослушивать сигналы `subscriptionRemoved` и `missed`:</span><span class="sxs-lookup"><span data-stu-id="f6d37-114">An app subscribing to notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals:</span></span>

- <span data-ttu-id="f6d37-115">После получения уведомления `subscriptionRemoved` приложение должно повторно создать подписку, чтобы поддерживать непрерывный поток.</span><span class="sxs-lookup"><span data-stu-id="f6d37-115">Upon receiving a `subscriptionRemoved` notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="f6d37-116">При получении уведомления `missed` приложение должно повторно синхронизировать данные ресурсов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6d37-116">On receiving a `missed` notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="f6d37-117">Чтобы получать уведомления жизненного цикла, можно использовать существующую конечную точку **notificationUrl**, которая уже получает уведомления о ресурсе, или можно зарегистрировать отдельное свойство **lifecycleNotificationUrl** для получения уведомлений `subscriptionRemoved` и `missed` в отдельной конечной точке.</span><span class="sxs-lookup"><span data-stu-id="f6d37-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives resource notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="f6d37-118">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="f6d37-118">Creating a subscription</span></span>

<span data-ttu-id="f6d37-119">При создании подписки вы можете указать отдельную конечную точку уведомлений с помощью свойства **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-119">When creating a subscription, you can specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="f6d37-120">Если указана конечная точка, все текущие и будущие типы уведомлений жизненного цикла будут доставляться в нее.</span><span class="sxs-lookup"><span data-stu-id="f6d37-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="f6d37-121">В противном случае уведомления `subscriptionRemoved` и `missed` будут доставляться в существующую конечную точку **notificationUrl** для всех существующих подписок.</span><span class="sxs-lookup"><span data-stu-id="f6d37-121">Otherwise, `subscriptionRemoved` and `missed` notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="f6d37-122">**Примечание.** В настоящий момент свойство **lifecycleNotificationUrl** можно настроить или считать только с помощью версии `beta` интерфейсов API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6d37-122">**Note:** At the moment, the **lifecycleNotificationUrl** property can only be set or read using the `beta` version of Microsoft Graph APIs.</span></span> <span data-ttu-id="f6d37-123">Однако подписки, созданные с помощью версии `beta`, хранятся в той же рабочей среде, что и для версии `v1.0`, поэтому можно реализовать новый поток Outlook, описанный в этой статье, в дополнение к обычному использованию версии `v1.0` с другими подписками.</span><span class="sxs-lookup"><span data-stu-id="f6d37-123">However, subscriptions created using `beta` are stored in the same production environment as `v1.0` so you can implement the new Outlook flow described here in addition to your regular usage of `v1.0` with other subscriptions.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="f6d37-124">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="f6d37-124">Subscription request example</span></span>

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
 
> <span data-ttu-id="f6d37-125">**Важно!** Используйте одинаковое имя узла для обоих URL-адресов уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f6d37-125">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="f6d37-126">**Примечание.** Вам нужно проверить обе конечные точки уведомлений, как описано в [статье об универсальных уведомлениях](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="f6d37-126">**Note:** You need to validate both notification endpoints as described in [the generic notification article](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="f6d37-127">Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.</span><span class="sxs-lookup"><span data-stu-id="f6d37-127">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="f6d37-128">**Примечание.** Вы не сможете обновить (`PATCH`) существующие подписки, чтобы добавить свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-128">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="f6d37-129">Следует удалить такие существующие подписки, создать новые подписки и указать свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-129">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="f6d37-130">Существующие подписки без свойства **lifecycleNotificationUrl** получают уведомления `subscriptionRemoved` и `missed` через **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-130">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="f6d37-131">Ответ на уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="f6d37-131">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="f6d37-132">Уведомление `subscriptionRemoved` информирует, что подписка была удалена и следует создать ее заново, если вы хотите продолжать получение уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f6d37-132">The `subscriptionRemoved` notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving notifications.</span></span> 

<span data-ttu-id="f6d37-133">Вы можете создавать длительные подписки (например, на 3 дня), а уведомления о данных ресурса начнут поступать в **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-133">You can create a long-lived subscription (e.g. 3 days), and resource data notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="f6d37-134">Однако условия доступа к данным ресурса могут со временем измениться.</span><span class="sxs-lookup"><span data-stu-id="f6d37-134">However, the conditions of access to the resource data may change over time.</span></span> <span data-ttu-id="f6d37-135">Например, в службе Outlook может произойти событие, требующее от приложения повторной проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6d37-135">For example, an event in the Outlook service may occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="f6d37-136">В таком случае поток выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="f6d37-136">In such a case, the flow looks as follows:</span></span>

1. <span data-ttu-id="f6d37-137">Outlook определяет, что подписка должна быть удалена из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6d37-137">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    1. <span data-ttu-id="f6d37-138">Для этих событий отсутствует заданная периодичность.</span><span class="sxs-lookup"><span data-stu-id="f6d37-138">There is no set cadence for these events.</span></span> <span data-ttu-id="f6d37-139">Для одних ресурсов они могут происходит часто, а для других — практически никогда.</span><span class="sxs-lookup"><span data-stu-id="f6d37-139">They may occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="f6d37-140">Microsoft Graph отправляет уведомление `subscriptionRemoved` для **lifecycleNotificationUrl** (если указано) или **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-140">Microsoft Graph sends a `subscriptionRemoved` notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="f6d37-141">Вы можете ответить на это уведомление, создав новую подписку для того же ресурса.</span><span class="sxs-lookup"><span data-stu-id="f6d37-141">You can respond to this notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="f6d37-142">Для этого нужно представить допустимый маркер доступа; в некоторых случаях это означает, что приложению необходимо выполнить повторную проверку подлинности пользователя, чтобы получить новый допустимый маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="f6d37-142">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="f6d37-143">Если вы успешно создали новую подписку, возобновится поток уведомлений о ресурсах.</span><span class="sxs-lookup"><span data-stu-id="f6d37-143">If you successfully create a new subscription, resource notifications will start flowing again.</span></span> <span data-ttu-id="f6d37-144">Но если вам не удалось это сделать (например, приложение не смогло получить допустимый маркер доступа), уведомления о ресурсах не отправляются.</span><span class="sxs-lookup"><span data-stu-id="f6d37-144">However, if you fail (for example, the app could not obtain a valid access token), resource notifications will not be sent.</span></span>

5. <span data-ttu-id="f6d37-145">Создав новую подписку, вы можете синхронизировать данные ресурсов, чтобы выявить все отсутствующие изменения.</span><span class="sxs-lookup"><span data-stu-id="f6d37-145">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="f6d37-146">Пример уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="f6d37-146">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="f6d37-147">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="f6d37-147">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="f6d37-148">Поле `"lifecycleEvent": "subscriptionRemoved"` определяет это уведомление, как связанное с удалением подписки.</span><span class="sxs-lookup"><span data-stu-id="f6d37-148">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="f6d37-149">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="f6d37-149">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="f6d37-150">Это уведомление не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="f6d37-150">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="f6d37-151">Как и уведомления о ресурсах, уведомления жизненного цикла могут объединяться (в массиве **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-151">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="f6d37-152">Обрабатывайте каждое уведомление в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="f6d37-152">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="f6d37-153">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="f6d37-153">Actions to take</span></span>

1. <span data-ttu-id="f6d37-154">[Подтвердите](webhooks.md#notifications) получение уведомления, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="f6d37-154">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="f6d37-155">[Проверьте](webhooks.md#notifications) подлинность уведомления.</span><span class="sxs-lookup"><span data-stu-id="f6d37-155">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="f6d37-156">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="f6d37-156">Ensure the app has a valid access token to take the next step.</span></span> 
> <span data-ttu-id="f6d37-157">**Примечание.** Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), они сделают это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, а также попросив пользователя войти еще раз (например, с помощью нового пароля).</span><span class="sxs-lookup"><span data-stu-id="f6d37-157">**Note:** If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to login again (e.g. with a new password).</span></span> <span data-ttu-id="f6d37-158">Обратите внимание, что получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и вызывающей стороне больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6d37-158">Note that obtaining a new token may fail, since the conditions of access may have changed, and the caller may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="f6d37-159">Создайте новую подписку с помощью стандартного процесса, описанного [здесь](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="f6d37-159">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

> <span data-ttu-id="f6d37-160">**Примечание.** Это действие может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="f6d37-160">**Note:** This action may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="f6d37-161">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="f6d37-161">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="f6d37-162">Вы может повторить эти действия позднее в любое время, например, когда изменятся условия доступа.</span><span class="sxs-lookup"><span data-stu-id="f6d37-162">You may retry these actions later, at any time, for example when the conditions of access have change.</span></span> <span data-ttu-id="f6d37-163">Все изменения ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="f6d37-163">Any resource changes in the time period from when the lifecycle notification was sent, to when the app re-creates the subscription successfully, will be lost.</span></span> <span data-ttu-id="f6d37-164">Приложению потребуется получить эти изменения самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="f6d37-164">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="f6d37-165">После создания новой подписки синхронизируйте все отсутствующие данные ресурсов с последнего известного момента получения уведомления об этом ресурсе. Например: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="f6d37-165">After creating the new subscription, sync any missing resource data from the last known time you received a notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="f6d37-166">Реагирование на пропущенные уведомления</span><span class="sxs-lookup"><span data-stu-id="f6d37-166">Responding to missed notifications</span></span>

<span data-ttu-id="f6d37-167">Эти сигналы сообщают, что некоторые уведомления могли быть не доставлены.</span><span class="sxs-lookup"><span data-stu-id="f6d37-167">These signals inform you that some notifications may have not been delivered.</span></span> <span data-ttu-id="f6d37-168">Вам следует решить, пропустить или обработать эти сигналы.</span><span class="sxs-lookup"><span data-stu-id="f6d37-168">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="f6d37-169">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="f6d37-169">Notification example</span></span>

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

<span data-ttu-id="f6d37-170">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="f6d37-170">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="f6d37-171">Поле `"lifecycleEvent": "missed"` определяет это в качестве сигнала о пропущенных уведомлениях.</span><span class="sxs-lookup"><span data-stu-id="f6d37-171">The `"lifecycleEvent": "missed"` field designates this as a signal about missed notifications.</span></span> <span data-ttu-id="f6d37-172">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="f6d37-172">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="f6d37-173">Это уведомление не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="f6d37-173">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change</span></span>
- <span data-ttu-id="f6d37-174">Как и уведомления о ресурсах, уведомления жизненного цикла могут объединяться (в массиве **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-174">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="f6d37-175">Обрабатывайте каждое уведомление в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="f6d37-175">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="f6d37-176">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="f6d37-176">Actions to take</span></span>

1. <span data-ttu-id="f6d37-177">[Подтвердите](webhooks.md#notifications) получение уведомления, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="f6d37-177">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="f6d37-178">Если вы игнорируете эти сигналы, не выполняйте других действий.</span><span class="sxs-lookup"><span data-stu-id="f6d37-178">If you ignore these, signals, do nothing else.</span></span> <span data-ttu-id="f6d37-179">В противном случае:</span><span class="sxs-lookup"><span data-stu-id="f6d37-179">Otherwise:</span></span>
2. <span data-ttu-id="f6d37-180">[Проверьте](webhooks.md#notifications) подлинность уведомления.</span><span class="sxs-lookup"><span data-stu-id="f6d37-180">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="f6d37-181">Выполните полную повторную синхронизацию данных ресурса для выявления изменений, не доставленных в качестве уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f6d37-181">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="f6d37-182">Готовый к изменениям код обработки уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="f6d37-182">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="f6d37-183">В будущем в Microsoft Graph будут добавлены другие типы уведомлений жизненного цикла подписки.</span><span class="sxs-lookup"><span data-stu-id="f6d37-183">In the future Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="f6d37-184">Они будут публиковаться в той же конечной точке: **lifecycleNotificationUrl**, но у них будет другое значение для **lifecycleEvent**, и они могут содержать немного другую схему и свойства, относящиеся к сценарию, для которого они создаются.</span><span class="sxs-lookup"><span data-stu-id="f6d37-184">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and may contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="f6d37-185">Следует реализовать свой код с готовностью к будущим изменениям, чтобы он не прерывался, когда в Microsoft Graph вводятся новые типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="f6d37-185">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="f6d37-186">Мы рекомендуем следующий подход:</span><span class="sxs-lookup"><span data-stu-id="f6d37-186">We recommend the following approach:</span></span>

1. <span data-ttu-id="f6d37-187">Явным образом определите каждое уведомление как поддерживаемое событие с помощью свойства **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="f6d37-187">Explicitly identify each notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="f6d37-188">Например, найдите свойство `"lifecycleEvent": "subscriptionRemoved"` для определения конкретного события и обработайте его.</span><span class="sxs-lookup"><span data-stu-id="f6d37-188">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="f6d37-189">Просматривайте объявления об уведомлениях для новых сценариев, так как в будущем могут быть представлены дополнительные типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="f6d37-189">Watch for announcements of notifications for new scenarions, as there may be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="f6d37-190">В своем приложении игнорируйте любые события жизненного цикла, не распознаваемые приложением, и заносите их в журнал для ознакомления.</span><span class="sxs-lookup"><span data-stu-id="f6d37-190">In your app, ignore any lifecycle events that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="f6d37-191">По своему усмотрению просматривайте соответствующую документацию о новых уведомлениях жизненного цикла и реализуйте для них нужную поддержку.</span><span class="sxs-lookup"><span data-stu-id="f6d37-191">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="f6d37-192">См. также</span><span class="sxs-lookup"><span data-stu-id="f6d37-192">See also</span></span>

- [<span data-ttu-id="f6d37-193">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="f6d37-193">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="f6d37-194">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="f6d37-194">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="f6d37-195">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="f6d37-195">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="f6d37-196">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="f6d37-196">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="f6d37-197">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="f6d37-197">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
