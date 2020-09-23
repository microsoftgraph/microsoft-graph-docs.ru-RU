---
title: Уменьшение числа пропущенных подписок и уведомлений об изменениях для ресурсов Outlook (предварительная версия)
description: Outlook может приостановить доставку уведомлений об изменениях из-за событий безопасности, например сброса пароля пользователя. Для обеспечения непрерывной доставки уведомлений об изменениях необходимо обрабатывать специальные события жизненного цикла (`subscriptionRemoved` и `missed`).
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 5e3dae04534029d657699150caf2f2a8e4d38cde
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193157"
---
# <a name="reduce-missing-subscriptions-and-change-notifications-for-outlook-resources-preview"></a><span data-ttu-id="4a75e-104">Уменьшение числа пропущенных подписок и уведомлений об изменениях для ресурсов Outlook (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4a75e-104">Reduce missing subscriptions and change notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="4a75e-105">У приложений, подписывающихся на уведомления об изменениях для ресурсов Outlook, могут быть удалены их подписки, что приводит к пропуску некоторых уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="4a75e-105">Apps subscribing to change notifications for Outlook resources might get their subscriptions removed and miss some change notifications.</span></span> <span data-ttu-id="4a75e-106">В приложениях должна быть реализована логика определения потерь и восстановления после них, а также возобновления непрерывного потока уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="4a75e-106">Apps should implement logic to detect and recover from the loss, and resume a continuous change notification flow.</span></span>

<span data-ttu-id="4a75e-107">Некоторые события в Outlook могут приводить к удалению подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="4a75e-108">К таким событиям относятся:</span><span class="sxs-lookup"><span data-stu-id="4a75e-108">These events include:</span></span>

- <span data-ttu-id="4a75e-109">сброс пароля пользователя;</span><span class="sxs-lookup"><span data-stu-id="4a75e-109">User's password has been reset</span></span>
- <span data-ttu-id="4a75e-110">устройство пользователя не соответствует требованиям;</span><span class="sxs-lookup"><span data-stu-id="4a75e-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="4a75e-111">учетная запись пользователя отозвана.</span><span class="sxs-lookup"><span data-stu-id="4a75e-111">User's account has been revoked</span></span>

<span data-ttu-id="4a75e-112">В случае такого события Outlook отправляет специальное уведомление жизненного цикла `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="4a75e-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="4a75e-113">Outlook также отправляет другое уведомление жизненного цикла `missed`, если уведомление об изменении не может быть доставлено в приложение.</span><span class="sxs-lookup"><span data-stu-id="4a75e-113">Outlook also sends another lifecycle notification, `missed`, if a change notification cannot be delivered to an app.</span></span>

<span data-ttu-id="4a75e-114">Приложение, подписывающееся на уведомления об изменениях для ресурсов Outlook, таких как **message** и **event**, должно прослушивать сигналы `subscriptionRemoved` и `missed`, и выполнить следующее:</span><span class="sxs-lookup"><span data-stu-id="4a75e-114">An app subscribing to change notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="4a75e-115">После получения уведомления жизненного цикла `subscriptionRemoved` приложение должно повторно создать подписку, чтобы поддерживать непрерывный поток.</span><span class="sxs-lookup"><span data-stu-id="4a75e-115">Upon receiving a `subscriptionRemoved` lifecycle notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="4a75e-116">При получении уведомления жизненного цикла `missed` приложение должно повторно синхронизировать данные ресурсов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4a75e-116">On receiving a `missed` lifecycle notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="4a75e-117">Чтобы получать уведомления жизненного цикла, можно использовать существующую конечную точку **notificationUrl**, которая уже получает уведомления об изменениях, или можно зарегистрировать отдельное свойство **lifecycleNotificationUrl** для получения уведомлений жизненного цикла `subscriptionRemoved` и `missed` в отдельной конечной точке.</span><span class="sxs-lookup"><span data-stu-id="4a75e-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives change notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` lifecycle notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="4a75e-118">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="4a75e-118">Creating a subscription</span></span>

<span data-ttu-id="4a75e-119">При создании подписки необходимо указать отдельную конечную точку уведомлений с помощью свойства **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-119">When creating a subscription, you must specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="4a75e-120">Если указана конечная точка, все текущие и будущие типы уведомлений жизненного цикла будут доставляться в нее.</span><span class="sxs-lookup"><span data-stu-id="4a75e-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="4a75e-121">В противном случае уведомления жизненного цикла `subscriptionRemoved` и `missed` доставляться не будут.</span><span class="sxs-lookup"><span data-stu-id="4a75e-121">Otherwise, `subscriptionRemoved` and `missed` lifecycle notifications will not be delivered.</span></span>

> <span data-ttu-id="4a75e-122">**Примечание.** Свойство **lifecycleNotificationUrl** можно настроить или считать только с помощью интерфейсов API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4a75e-122">**Note:** The **lifecycleNotificationUrl** property can only be set or read using Microsoft Graph beta APIs.</span></span> <span data-ttu-id="4a75e-123">Однако подписки, созданные с помощью бета-версий API, хранятся в той же рабочей среде, что и подписки, созданные с помощью версии 1.0, поэтому можно реализовать новый поток Outlook в дополнение к вашим подпискам, создаваемым с помощью версии API 1.0.</span><span class="sxs-lookup"><span data-stu-id="4a75e-123">However, subscriptions created using beta APIs are stored in the same production environment as those created using v1.0, so you can implement the new Outlook flow in addition to your subscriptions creating using v1.0 APIs.</span></span>

> <span data-ttu-id="4a75e-124">Подписки, созданные с помощью версии API 1.0, будут получать уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="4a75e-124">Subscriptions created via the v1.0 APIs will receive lifecycle notifications.</span></span> 

### <a name="subscription-request-example"></a><span data-ttu-id="4a75e-125">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="4a75e-125">Subscription request example</span></span>

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
 
> <span data-ttu-id="4a75e-126">**Важно!** Используйте одинаковое имя узла для обоих URL-адресов уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4a75e-126">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="4a75e-127">**Примечание.** Вам нужно проверить обе конечные точки, как описано в статье [Управление подписками](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="4a75e-127">**Note:** You need to validate both endpoints as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="4a75e-128">Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.</span><span class="sxs-lookup"><span data-stu-id="4a75e-128">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="4a75e-129">**Примечание.** Вы не сможете обновить (`PATCH`) существующие подписки, чтобы добавить свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-129">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="4a75e-130">Следует удалить такие существующие подписки, создать новые подписки и указать свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-130">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="4a75e-131">Существующие подписки без свойства **lifecycleNotificationUrl** не будут получать `subscriptionRemoved` и `missed`.</span><span class="sxs-lookup"><span data-stu-id="4a75e-131">Existing subscriptions without **lifecycleNotificationUrl** property will not receive the `subscriptionRemoved` and `missed`.</span></span>

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="4a75e-132">Ответ на уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="4a75e-132">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="4a75e-133">Уведомление жизненного цикла `subscriptionRemoved` информирует, что подписка была удалена и следует создать ее заново, если вы хотите продолжать получение уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="4a75e-133">The `subscriptionRemoved` lifecycle notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving change notifications.</span></span> 

<span data-ttu-id="4a75e-134">Вы можете создавать длительные подписки (на 3 дня), а уведомления об изменениях начнут поступать в **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-134">You can create a long-lived subscription (3 days), and change notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="4a75e-135">Однако условия доступа к данным ресурса могут со временем измениться.</span><span class="sxs-lookup"><span data-stu-id="4a75e-135">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="4a75e-136">Например, в службе Outlook может произойти событие, требующее от приложения повторной проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="4a75e-136">For example, an event in the Outlook service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="4a75e-137">В таком случае поток выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="4a75e-137">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="4a75e-138">Outlook определяет, что подписка должна быть удалена из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4a75e-138">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="4a75e-139">Для этих событий отсутствует заданная периодичность.</span><span class="sxs-lookup"><span data-stu-id="4a75e-139">There is no set cadence for these events.</span></span> <span data-ttu-id="4a75e-140">Для одних ресурсов они могут происходить часто, а для других — практически никогда.</span><span class="sxs-lookup"><span data-stu-id="4a75e-140">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="4a75e-141">Microsoft Graph отправляет уведомление жизненного цикла `subscriptionRemoved` для **lifecycleNotificationUrl** (если указано).</span><span class="sxs-lookup"><span data-stu-id="4a75e-141">Microsoft Graph sends a `subscriptionRemoved` lifecycle notification to the **lifecycleNotificationUrl** (if specified).</span></span>  

3. <span data-ttu-id="4a75e-142">Вы можете ответить на это уведомление жизненного цикла, создав новую подписку для того же ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a75e-142">You can respond to this lifecycle notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="4a75e-143">Для этого нужно представить допустимый маркер доступа; в некоторых случаях это означает, что приложению необходимо выполнить повторную проверку подлинности пользователя, чтобы получить новый допустимый маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="4a75e-143">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="4a75e-144">Если вы успешно создали новую подписку, возобновится поток уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="4a75e-144">If you successfully create a new subscription, change notifications will start flowing again.</span></span> <span data-ttu-id="4a75e-145">Но если вам не удалось это сделать (например, приложение не может получить допустимый маркер доступа), уведомления об изменениях не отправляются.</span><span class="sxs-lookup"><span data-stu-id="4a75e-145">However, if you fail (for example, the app can't obtain a valid access token), change notifications will not be sent.</span></span>

5. <span data-ttu-id="4a75e-146">Создав новую подписку, вы можете синхронизировать данные ресурсов, чтобы выявить все отсутствующие изменения.</span><span class="sxs-lookup"><span data-stu-id="4a75e-146">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="4a75e-147">Пример уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="4a75e-147">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="4a75e-148">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="4a75e-148">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="4a75e-149">Поле `"lifecycleEvent": "subscriptionRemoved"` определяет это уведомление, как связанное с удалением подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-149">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="4a75e-150">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="4a75e-150">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="4a75e-151">Это уведомление жизненного цикла не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-151">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="4a75e-152">Как и уведомления об изменениях, уведомления жизненного цикла могут объединяться (в массиве **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-152">Similar to change notifications, lifecycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="4a75e-153">Обрабатывайте каждое уведомление жизненного цикла в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="4a75e-153">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="4a75e-154">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="4a75e-154">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="4a75e-155">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="4a75e-155">Actions to take</span></span>

1. <span data-ttu-id="4a75e-156">[Подтвердите](webhooks.md#change-notifications) получение уведомления жизненного цикла, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="4a75e-156">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="4a75e-157">[Проверьте](webhooks.md#change-notifications) подлинность уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="4a75e-157">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="4a75e-158">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="4a75e-158">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="4a75e-159">**Примечание.** Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), они сделают это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, а также попросив пользователя войти еще раз (с помощью нового пароля).</span><span class="sxs-lookup"><span data-stu-id="4a75e-159">**Note:** If you're using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="4a75e-160">Обратите внимание, что получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и вызывающей стороне больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a75e-160">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="4a75e-161">Создайте новую подписку с помощью стандартного процесса, описанного [здесь](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="4a75e-161">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="4a75e-162">**Примечание.** Это действие может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="4a75e-162">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="4a75e-163">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-163">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="4a75e-164">Вы можете повторить эти действия позднее в любое время, например, когда изменятся условия доступа.</span><span class="sxs-lookup"><span data-stu-id="4a75e-164">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="4a75e-165">Все изменения ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="4a75e-165">Any resource changes in the time period from when the lifecycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="4a75e-166">Приложению потребуется получить эти изменения самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="4a75e-166">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="4a75e-167">После создания новой подписки синхронизируйте все отсутствующие данные ресурсов с последнего известного момента получения уведомления об изменении для этого ресурса. Например: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="4a75e-167">After creating the new subscription, sync any missing resource data from the last known time you received a change notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="4a75e-168">Реагирование на пропущенные уведомления</span><span class="sxs-lookup"><span data-stu-id="4a75e-168">Responding to missed notifications</span></span>

<span data-ttu-id="4a75e-169">Эти сигналы сообщают, что некоторые уведомления об изменениях могли быть не доставлены.</span><span class="sxs-lookup"><span data-stu-id="4a75e-169">These signals inform you that some change notifications might not have been delivered.</span></span> <span data-ttu-id="4a75e-170">Вам следует решить, пропустить или обработать эти сигналы.</span><span class="sxs-lookup"><span data-stu-id="4a75e-170">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="4a75e-171">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="4a75e-171">Notification example</span></span>

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

<span data-ttu-id="4a75e-172">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="4a75e-172">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="4a75e-173">Поле `"lifecycleEvent": "missed"` определяет это в качестве сигнала о пропущенных уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="4a75e-173">The `"lifecycleEvent": "missed"` field designates this as a signal about missed change notifications.</span></span> <span data-ttu-id="4a75e-174">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="4a75e-174">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="4a75e-175">Это уведомление жизненного цикла не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-175">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="4a75e-176">Как и уведомления об изменениях, уведомления жизненного цикла могут объединяться (в массиве **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-176">Similar to change notifications, lifecycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="4a75e-177">Обрабатывайте каждое уведомление жизненного цикла в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="4a75e-177">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="4a75e-178">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="4a75e-178">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="4a75e-179">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="4a75e-179">Actions to take</span></span>

1. <span data-ttu-id="4a75e-180">[Подтвердите](webhooks.md#change-notifications) получение уведомления жизненного цикла, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="4a75e-180">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="4a75e-181">Если вы игнорируете эти сигналы, не выполняйте других действий.</span><span class="sxs-lookup"><span data-stu-id="4a75e-181">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="4a75e-182">В противном случае:</span><span class="sxs-lookup"><span data-stu-id="4a75e-182">Otherwise:</span></span>
2. <span data-ttu-id="4a75e-183">[Проверьте](webhooks.md#change-notifications) подлинность уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="4a75e-183">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="4a75e-184">Выполните полную повторную синхронизацию данных ресурса для выявления изменений, не доставленных в качестве уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4a75e-184">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 

## <a name="responding-to-reauthorizationrequired-notifications"></a><span data-ttu-id="4a75e-185">Реагирование на уведомления reauthorizationRequired</span><span class="sxs-lookup"><span data-stu-id="4a75e-185">Responding to reauthorizationRequired notifications</span></span>

<span data-ttu-id="4a75e-186">Получив уведомление о жизненном цикле `reauthorizationRequired`, необходимо выполнить повторную авторизацию подписки, чтобы поток данных не прекращался.</span><span class="sxs-lookup"><span data-stu-id="4a75e-186">When you receive a `reauthorizationRequired` lifecycle notification, you must reauthorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="4a75e-187">Вы можете создавать длительные подписки (на 3 дня), таким образом уведомления об изменениях начнут поступать в **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-187">You can create a long-lived subscription (3 days), which enables change notifications to flow to the **notificationUrl**.</span></span> <span data-ttu-id="4a75e-188">В случае изменений в условия доступа Microsoft Graph может потребовать повторную авторизацию подписки, чтобы подтвердить наличие у вас доступа к данным ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a75e-188">If the conditions of access have changed since the subscription was created, Microsoft Graph may require that you reauthorize the subscription to prove that you still have access to resource data.</span></span> <span data-ttu-id="4a75e-189">Ниже приведены примеры изменений, влияющих на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="4a75e-189">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="4a75e-190">Администратор клиента может отозвать разрешения приложения на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a75e-190">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="4a75e-191">В интерактивном сценарии к пользователю, предоставляющему маркер проверки подлинности для вашего приложения, могут применяться динамические политики на основе различных факторов, например их расположения, состояния устройства или оценки риска.</span><span class="sxs-lookup"><span data-stu-id="4a75e-191">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="4a75e-192">Например, если пользователь изменяет свое физическое расположение, ему может быть запрещен доступ к данным, и ваше приложение не сможет повторно авторизовать подписку.</span><span class="sxs-lookup"><span data-stu-id="4a75e-192">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to reauthorize the subscription.</span></span> <span data-ttu-id="4a75e-193">Дополнительные сведения о динамических политиках, управляющих доступом, см. в статье [Политики условного доступа Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="4a75e-193">For more information about dynamic policies that control access, see [Azure AD conditional access policies](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span></span> 

<span data-ttu-id="4a75e-194">Ниже указаны шаги, которые представляют собой поток запроса авторизации для активной подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-194">The following steps represent the flow of an authorization challenge for an active subscription:</span></span>

1. <span data-ttu-id="4a75e-195">Microsoft Graph требует повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-195">Microsoft Graph requires a subscription to be reauthorized.</span></span>
    
    <span data-ttu-id="4a75e-196">Причины этого могут отличаться для разных ресурсов и меняться со временем.</span><span class="sxs-lookup"><span data-stu-id="4a75e-196">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="4a75e-197">Необходимо ответить на событие повторной авторизации независимо от его причины.</span><span class="sxs-lookup"><span data-stu-id="4a75e-197">You must respond to a reauthorization event no matter what caused it.</span></span>

2. <span data-ttu-id="4a75e-198">Microsoft Graph отправляет уведомление о запросе авторизации в **lifecycleNotificationUrl**</span><span class="sxs-lookup"><span data-stu-id="4a75e-198">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**.</span></span>

    <span data-ttu-id="4a75e-199">Обратите внимание, что поток уведомлений об изменениях может некоторое время продолжаться, предоставляя вам дополнительное время для ответа.</span><span class="sxs-lookup"><span data-stu-id="4a75e-199">Note that the flow of change notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="4a75e-200">Однако в конечном итоге доставка уведомлений об изменениях приостанавливается, пока вы не выполните требуемое действие.</span><span class="sxs-lookup"><span data-stu-id="4a75e-200">However, eventually change notification delivery pauses, until you take the required action.</span></span>

3. <span data-ttu-id="4a75e-201">Ответьте на это уведомление жизненного цикла одним из указанных ниже двух способов.</span><span class="sxs-lookup"><span data-stu-id="4a75e-201">Respond to this lifecycle notification in one of two ways:</span></span>
    - <span data-ttu-id="4a75e-202">Повторная авторизация подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-202">Reauthorize the subscription.</span></span> <span data-ttu-id="4a75e-203">Это не продлевает срок действия подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-203">This does not extend the expiry date of the subscription.</span></span>
    - <span data-ttu-id="4a75e-204">Возобновление подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-204">Renew the subscription.</span></span> <span data-ttu-id="4a75e-205">Это повторно авторизует подписку и продлевает срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="4a75e-205">This both reauthorizes and extends the expiry date.</span></span>

    <span data-ttu-id="4a75e-206">Примечание. Оба действия требуют предоставление действительного маркера проверки подлинности по аналогии с [созданием новой подписки](webhooks.md#creating-a-subscription) или [продлением подписки до истечения срока ее действия](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="4a75e-206">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="4a75e-207">Если вы успешно выполнили повторную авторизацию или возобновление подписки, уведомления об изменениях продолжать поступать.</span><span class="sxs-lookup"><span data-stu-id="4a75e-207">If you successfully reauthorize or renew the subscription, change notifications continue.</span></span> <span data-ttu-id="4a75e-208">В противном случае уведомления об изменениях не будут возобновлены.</span><span class="sxs-lookup"><span data-stu-id="4a75e-208">Otherwise, change notifications remain paused.</span></span>

### <a name="reauthorizationrequired-notification-example"></a><span data-ttu-id="4a75e-209">Пример уведомления reauthorizationRequired</span><span class="sxs-lookup"><span data-stu-id="4a75e-209">reauthorizationRequired notification example</span></span>

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

<span data-ttu-id="4a75e-210">Обратите внимание на указанные ниже моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="4a75e-210">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="4a75e-211">Поле `"lifecycleEvent": "reauthorizationRequired"` назначает это уведомление запросом на авторизацию.</span><span class="sxs-lookup"><span data-stu-id="4a75e-211">The `"lifecycleEvent": "reauthorizationRequired"` field designates this notification as an authorization challenge.</span></span> <span data-ttu-id="4a75e-212">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="4a75e-212">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="4a75e-213">Это уведомление жизненного цикла не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-213">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="4a75e-214">Как и уведомления об изменениях, уведомления жизненного цикла можно объединять (в коллекции **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-214">Similar to change notifications, you can batch lifecycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="4a75e-215">Обрабатывайте каждое уведомление жизненного цикла в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="4a75e-215">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="4a75e-216">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="4a75e-216">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="4a75e-217">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="4a75e-217">Actions to take</span></span>

1. <span data-ttu-id="4a75e-218">[Подтвердите](webhooks.md#change-notifications) получение уведомления жизненного цикла, ответив на вызов POST с помощью `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="4a75e-218">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="4a75e-219">[Проверьте](webhooks.md#change-notifications) подлинность уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="4a75e-219">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="4a75e-220">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="4a75e-220">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="4a75e-221">**Примечание.** Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), они сделают это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, а также попросив пользователя войти еще раз (с помощью нового пароля).</span><span class="sxs-lookup"><span data-stu-id="4a75e-221">**Note:** If you're using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="4a75e-222">Обратите внимание, что получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и вызывающей стороне больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a75e-222">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="4a75e-223">Вызовите один из двух следующих API.</span><span class="sxs-lookup"><span data-stu-id="4a75e-223">Call either of the following two APIs.</span></span> <span data-ttu-id="4a75e-224">Если вызов API выполняется успешно, поток уведомлений об изменениях возобновляется.</span><span class="sxs-lookup"><span data-stu-id="4a75e-224">If the API call succeeds, the change notification flow resumes.</span></span>

    - <span data-ttu-id="4a75e-225">Чтобы повторно авторизовать подписку без продления ее срока, вызовите действие `/reauthorize`:</span><span class="sxs-lookup"><span data-stu-id="4a75e-225">Call the `/reauthorize` action to reauthorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="4a75e-226">Чтобы одновременно возобновить и повторно авторизовать подписку, выполните обычное действие возобновления:</span><span class="sxs-lookup"><span data-stu-id="4a75e-226">Perform a regular renew action to reauthorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="4a75e-227">Возобновление может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="4a75e-227">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="4a75e-228">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-228">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> 
      
      <span data-ttu-id="4a75e-229">Вы может повторить эти действия позднее в любое время и успешно выполнить их, если изменяются условия доступа.</span><span class="sxs-lookup"><span data-stu-id="4a75e-229">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="4a75e-230">Все уведомления об изменении ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="4a75e-230">Any notifications about resource changes that happen between the time the lifecycle notification was sent and the time when the app successfully creates the subscription again, would be lost.</span></span> <span data-ttu-id="4a75e-231">В таких случаях приложению нужно отдельно получить эти изменения.</span><span class="sxs-lookup"><span data-stu-id="4a75e-231">In such cases, the app should separately fetch those changes.</span></span>

### <a name="additional-information"></a><span data-ttu-id="4a75e-232">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="4a75e-232">Additional information</span></span>

<span data-ttu-id="4a75e-233">Ниже приведены сведения, которые помогут разобраться с проблемами авторизации.</span><span class="sxs-lookup"><span data-stu-id="4a75e-233">The following information can help you understand authorization challenges:</span></span>

- <span data-ttu-id="4a75e-234">Запросы авторизации не отменяют необходимость возобновления подписки на изменения ресурса до истечения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="4a75e-234">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="4a75e-235">Хотя вы можете возобновить подписку при получении запроса авторизации, Microsoft Graph может не выполнять запрос для всех ваших подписок.</span><span class="sxs-lookup"><span data-stu-id="4a75e-235">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="4a75e-236">Например, подписка без действий и уведомлений об изменениях, ожидающих доставки, может не создавать для приложения запросы на повторную авторизацию.</span><span class="sxs-lookup"><span data-stu-id="4a75e-236">For example, a subscription that does not have any activity and has no change notifications pending delivery may not signal any reauthorization challenges to your app.</span></span> <span data-ttu-id="4a75e-237">Обязательно [возобновите подписки](webhooks.md#renewing-a-subscription) до истечения их сроков действия.</span><span class="sxs-lookup"><span data-stu-id="4a75e-237">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

- <span data-ttu-id="4a75e-238">Частота запросов авторизации может изменяться.</span><span class="sxs-lookup"><span data-stu-id="4a75e-238">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="4a75e-239">Не делайте предположений о частоте запросов авторизации.</span><span class="sxs-lookup"><span data-stu-id="4a75e-239">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="4a75e-240">Эти уведомления жизненного цикла сообщают, когда нужно принимать действия, избавляя от отслеживания подписок, которым требуется повторная авторизация.</span><span class="sxs-lookup"><span data-stu-id="4a75e-240">These lifecycle notifications tell you when to take actions, saving you from having to track which subscriptions require reauthorization.</span></span> <span data-ttu-id="4a75e-241">Будьте готовы обрабатывать запросы авторизации каждые несколько минут для всех подписок или в редких случаях лишь для некоторых своих подписок.</span><span class="sxs-lookup"><span data-stu-id="4a75e-241">Be ready to handle authorization challenges from once every few minutes for every subscription to rarely for only some of your subscriptions.</span></span>

## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="4a75e-242">Готовый к изменениям код обработки уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="4a75e-242">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="4a75e-243">В будущем в Microsoft Graph будут добавлены другие типы уведомлений жизненного цикла подписки.</span><span class="sxs-lookup"><span data-stu-id="4a75e-243">In the future, Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="4a75e-244">Они будут публиковаться в той же конечной точке: **lifecycleNotificationUrl**, но у них будет другое значение для **lifecycleEvent**, и они могут содержать немного другую схему и свойства, относящиеся к сценарию, для которого они создаются.</span><span class="sxs-lookup"><span data-stu-id="4a75e-244">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="4a75e-245">Следует реализовать свой код с готовностью к будущим изменениям, чтобы он не прерывался, когда в Microsoft Graph вводятся новые типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="4a75e-245">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="4a75e-246">Мы рекомендуем следующий подход:</span><span class="sxs-lookup"><span data-stu-id="4a75e-246">We recommend the following approach:</span></span>

1. <span data-ttu-id="4a75e-247">Явным образом определите каждое уведомление жизненного цикла как поддерживаемое событие с помощью свойства **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="4a75e-247">Explicitly identify each lifecycle notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="4a75e-248">Например, найдите свойство `"lifecycleEvent": "subscriptionRemoved"` для определения конкретного события и обработайте его.</span><span class="sxs-lookup"><span data-stu-id="4a75e-248">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="4a75e-249">Обратите внимание на объявления уведомлений жизненного цикла о новых сценариях.</span><span class="sxs-lookup"><span data-stu-id="4a75e-249">Watch for announcements of lifecycle notifications for new scenarions.</span></span> <span data-ttu-id="4a75e-250">В будущем могут быть доступны и другие типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="4a75e-250">There might be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="4a75e-251">В своем приложении игнорируйте любые уведомления жизненного цикла, не распознаваемые приложением, и заносите их в журнал для ознакомления.</span><span class="sxs-lookup"><span data-stu-id="4a75e-251">In your app, ignore any lifecycle notification that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="4a75e-252">По своему усмотрению просматривайте соответствующую документацию о новых уведомлениях жизненного цикла и реализуйте для них нужную поддержку.</span><span class="sxs-lookup"><span data-stu-id="4a75e-252">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="4a75e-253">См. также</span><span class="sxs-lookup"><span data-stu-id="4a75e-253">See also</span></span>

- [<span data-ttu-id="4a75e-254">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="4a75e-254">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="4a75e-255">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="4a75e-255">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="4a75e-256">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="4a75e-256">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="4a75e-257">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="4a75e-257">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="4a75e-258">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="4a75e-258">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
