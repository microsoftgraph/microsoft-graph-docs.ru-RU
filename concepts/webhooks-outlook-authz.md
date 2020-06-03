---
title: Сокращение количества отсутствующих подписок и уведомлений об изменениях для ресурсов Outlook (Предварительная версия)
description: Outlook может приостановить доставку уведомлений об изменениях из-за событий безопасности, например сброса пароля пользователя. Особые события жизненного цикла, которые необходимо `subscriptionRemoved` `missed` обработать для обеспечения непрерывной доставки уведомлений об изменениях.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 8b2174ea14dd7e3d6af7f0b4a447c4e5afa6fce1
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429630"
---
# <a name="reduce-missing-subscriptions-and-change-notifications-for-outlook-resources-preview"></a><span data-ttu-id="99127-104">Сокращение количества отсутствующих подписок и уведомлений об изменениях для ресурсов Outlook (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="99127-104">Reduce missing subscriptions and change notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="99127-105">Подписки на приложения на уведомления об изменениях для ресурсов Outlook могут стать удаленными и пропускать некоторые уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="99127-105">Apps subscribing to change notifications for Outlook resources might get their subscriptions removed and miss some change notifications.</span></span> <span data-ttu-id="99127-106">Приложения должны реализовать логику для обнаружения и восстановления после потери и возобновление непрерывного процесса уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="99127-106">Apps should implement logic to detect and recover from the loss, and resume a continuous change notification flow.</span></span>

<span data-ttu-id="99127-107">Некоторые события в Outlook могут приводить к удалению подписки.</span><span class="sxs-lookup"><span data-stu-id="99127-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="99127-108">К таким событиям относятся:</span><span class="sxs-lookup"><span data-stu-id="99127-108">These events include:</span></span>

- <span data-ttu-id="99127-109">сброс пароля пользователя;</span><span class="sxs-lookup"><span data-stu-id="99127-109">User's password has been reset</span></span>
- <span data-ttu-id="99127-110">устройство пользователя не соответствует требованиям;</span><span class="sxs-lookup"><span data-stu-id="99127-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="99127-111">учетная запись пользователя отозвана.</span><span class="sxs-lookup"><span data-stu-id="99127-111">User's account has been revoked</span></span>

<span data-ttu-id="99127-112">В случае такого события Outlook отправляет специальное уведомление жизненного цикла `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="99127-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="99127-113">Outlook также отправляет еще одно уведомление о жизненном цикле, `missed` Если уведомление об изменении не может быть доставлено приложению.</span><span class="sxs-lookup"><span data-stu-id="99127-113">Outlook also sends another lifecycle notification, `missed`, if a change notification cannot be delivered to an app.</span></span>

<span data-ttu-id="99127-114">Приложение, которое поддается подписке на уведомления об изменениях для ресурсов Outlook, таких как **сообщение** и **событие**, должно прослушивать `subscriptionRemoved` `missed` сигналы и выполнять следующие действия:</span><span class="sxs-lookup"><span data-stu-id="99127-114">An app subscribing to change notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="99127-115">После получения `subscriptionRemoved` уведомления жизненного цикла приложение должно повторно создать подписку, чтобы обеспечить непрерывный процесс.</span><span class="sxs-lookup"><span data-stu-id="99127-115">Upon receiving a `subscriptionRemoved` lifecycle notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="99127-116">При получении `missed` уведомления о жизненном цикле приложение должно повторно синхронизировать данные ресурса с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="99127-116">On receiving a `missed` lifecycle notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="99127-117">Чтобы получать уведомления о жизненном цикле, вы можете использовать существующую конечную точку **notificationUrl** , которая уже получает уведомления об изменениях, или зарегистрировать отдельные **лифецикленотификатионурл** для получения `subscriptionRemoved` уведомлений и их `missed` жизненного цикла в отдельной конечной точке.</span><span class="sxs-lookup"><span data-stu-id="99127-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives change notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` lifecycle notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="99127-118">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="99127-118">Creating a subscription</span></span>

<span data-ttu-id="99127-119">При создании подписки можно указать отдельную конечную точку с помощью свойства **лифецикленотификатионурл** .</span><span class="sxs-lookup"><span data-stu-id="99127-119">When creating a subscription, you can specify a separate endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="99127-120">Если указана конечная точка, все текущие и будущие типы уведомлений жизненного цикла будут доставляться в нее.</span><span class="sxs-lookup"><span data-stu-id="99127-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="99127-121">В противном случае, `subscriptionRemoved` и `missed` уведомления о жизненных циклах будут доставляться в существующие **notificationUrl** для всех существующих подписок.</span><span class="sxs-lookup"><span data-stu-id="99127-121">Otherwise, `subscriptionRemoved` and `missed` lifecycle notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="99127-122">**Примечание.** Свойство **lifecycleNotificationUrl** можно настроить или считать только с помощью интерфейсов API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="99127-122">**Note:** The **lifecycleNotificationUrl** property can only be set or read using Microsoft Graph beta APIs.</span></span> <span data-ttu-id="99127-123">Однако подписки, созданные с помощью бета-версий API, хранятся в той же рабочей среде, что и подписки, созданные с помощью версии 1.0, поэтому можно реализовать новый поток Outlook в дополнение к вашим подпискам, создаваемым с помощью версии API 1.0.</span><span class="sxs-lookup"><span data-stu-id="99127-123">However, subscriptions created using beta APIs are stored in the same production environment as those created using v1.0, so you can implement the new Outlook flow in addition to your subscriptions creating using v1.0 APIs.</span></span>

> <span data-ttu-id="99127-124">Подписки, созданные с помощью версии API 1.0, будут получать уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="99127-124">Subscriptions created via the v1.0 APIs will receive lifecycle notifications.</span></span> 

### <a name="subscription-request-example"></a><span data-ttu-id="99127-125">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="99127-125">Subscription request example</span></span>

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
 
> <span data-ttu-id="99127-126">**Важно!** Используйте одинаковое имя узла для обоих URL-адресов уведомлений.</span><span class="sxs-lookup"><span data-stu-id="99127-126">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="99127-127">**Примечание:** Необходимо проверить обе конечные точки, как описано в статье [Управление подписками](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="99127-127">**Note:** You need to validate both endpoints as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="99127-128">Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.</span><span class="sxs-lookup"><span data-stu-id="99127-128">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="99127-129">**Примечание.** Вы не сможете обновить (`PATCH`) существующие подписки, чтобы добавить свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="99127-129">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="99127-130">Следует удалить такие существующие подписки, создать новые подписки и указать свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="99127-130">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="99127-131">Существующие подписки без свойства **лифецикленотификатионурл** будут получать `subscriptionRemoved` `missed` уведомления о жизненном цикле через **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="99127-131">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` lifecycle notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="99127-132">Ответ на уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="99127-132">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="99127-133">`subscriptionRemoved`Уведомление о жизненном цикле уведомляет о том, что подписка удалена и должна быть повторно создана, если вы хотите продолжить получать уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="99127-133">The `subscriptionRemoved` lifecycle notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving change notifications.</span></span> 

<span data-ttu-id="99127-134">Вы можете создать подписку с длинным сроком действия (3 дня), а уведомления об изменениях начнут переступать в **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="99127-134">You can create a long-lived subscription (3 days), and change notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="99127-135">Однако условия доступа к данным ресурса могут со временем измениться.</span><span class="sxs-lookup"><span data-stu-id="99127-135">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="99127-136">Например, в службе Outlook может произойти событие, требующее от приложения повторной проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="99127-136">For example, an event in the Outlook service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="99127-137">В таком случае поток выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="99127-137">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="99127-138">Outlook определяет, что подписка должна быть удалена из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="99127-138">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="99127-139">Для этих событий отсутствует заданная периодичность.</span><span class="sxs-lookup"><span data-stu-id="99127-139">There is no set cadence for these events.</span></span> <span data-ttu-id="99127-140">Для одних ресурсов они могут происходить часто, а для других — практически никогда.</span><span class="sxs-lookup"><span data-stu-id="99127-140">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="99127-141">Microsoft Graph отправляет `subscriptionRemoved` уведомление о жизненном цикле в **лифецикленотификатионурл** (если оно указано) или **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="99127-141">Microsoft Graph sends a `subscriptionRemoved` lifecycle notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="99127-142">Вы можете ответить на это уведомление о жизненном цикле, создав новую подписку для того же ресурса.</span><span class="sxs-lookup"><span data-stu-id="99127-142">You can respond to this lifecycle notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="99127-143">Для этого нужно представить допустимый маркер доступа; в некоторых случаях это означает, что приложению необходимо выполнить повторную проверку подлинности пользователя, чтобы получить новый допустимый маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="99127-143">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="99127-144">Если вы успешно создали новую подписку, уведомления об изменениях начнут переступать повторно.</span><span class="sxs-lookup"><span data-stu-id="99127-144">If you successfully create a new subscription, change notifications will start flowing again.</span></span> <span data-ttu-id="99127-145">Однако в случае ошибки (например, приложению не удается получить действительный маркер доступа) уведомления об изменениях не будут отправлены.</span><span class="sxs-lookup"><span data-stu-id="99127-145">However, if you fail (for example, the app can't obtain a valid access token), change notifications will not be sent.</span></span>

5. <span data-ttu-id="99127-146">Создав новую подписку, вы можете синхронизировать данные ресурсов, чтобы выявить все отсутствующие изменения.</span><span class="sxs-lookup"><span data-stu-id="99127-146">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="99127-147">Пример уведомления subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="99127-147">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="99127-148">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="99127-148">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="99127-149">Поле `"lifecycleEvent": "subscriptionRemoved"` определяет это уведомление, как связанное с удалением подписки.</span><span class="sxs-lookup"><span data-stu-id="99127-149">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="99127-150">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="99127-150">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="99127-151">В уведомлении о жизненном цикле не содержатся сведения об определенном ресурсе, так как он не связан с изменением ресурса, но с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="99127-151">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="99127-152">Аналогично уведомлениям об изменении, уведомления о жизненном цикле могут составляться пакетно (в массиве **значений** ), с которым, возможно, различное значение **лифецикливент** .</span><span class="sxs-lookup"><span data-stu-id="99127-152">Similar to change notifications, lifecycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="99127-153">Соответствующим образом обработайте каждое уведомление о жизненном цикле в пакете.</span><span class="sxs-lookup"><span data-stu-id="99127-153">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="99127-154">**Примечание:** полное описание данных, отправленных при доставке уведомлений об изменении, приведено в разделе [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="99127-154">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="99127-155">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="99127-155">Actions to take</span></span>

1. <span data-ttu-id="99127-156">[Подтвердите](webhooks.md#change-notifications) получение уведомления о жизненном цикле, выполнив ответ на вызов Post `202 - Accepted` .</span><span class="sxs-lookup"><span data-stu-id="99127-156">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="99127-157">[Проверка](webhooks.md#change-notifications) подлинности уведомления о жизненном цикле.</span><span class="sxs-lookup"><span data-stu-id="99127-157">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="99127-158">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="99127-158">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="99127-159">**Примечание.** Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), они сделают это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, а также попросив пользователя войти еще раз (с помощью нового пароля).</span><span class="sxs-lookup"><span data-stu-id="99127-159">**Note:** If you're using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="99127-160">Обратите внимание, что получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и вызывающей стороне больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99127-160">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="99127-161">Создайте новую подписку с помощью стандартного процесса, описанного [здесь](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="99127-161">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="99127-162">**Примечание.** Это действие может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="99127-162">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="99127-163">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="99127-163">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="99127-164">Вы можете повторить эти действия позднее в любое время, например, когда изменятся условия доступа.</span><span class="sxs-lookup"><span data-stu-id="99127-164">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="99127-165">Любые изменения ресурсов за период времени с момента отправки уведомления о жизненном цикле, чтобы приложение успешно повторно создало подписку, будет потеряно.</span><span class="sxs-lookup"><span data-stu-id="99127-165">Any resource changes in the time period from when the lifecycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="99127-166">Приложению потребуется получить эти изменения самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="99127-166">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="99127-167">После создания новой подписки синхронизируйте все недостающие данные ресурсов из последнего известного времени, когда вы получили уведомление об изменении этого ресурса; Например:`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="99127-167">After creating the new subscription, sync any missing resource data from the last known time you received a change notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="99127-168">Реагирование на пропущенные уведомления</span><span class="sxs-lookup"><span data-stu-id="99127-168">Responding to missed notifications</span></span>

<span data-ttu-id="99127-169">Эти сигналы сообщают о том, что некоторые уведомления об изменениях могут быть не доставлены.</span><span class="sxs-lookup"><span data-stu-id="99127-169">These signals inform you that some change notifications might not have been delivered.</span></span> <span data-ttu-id="99127-170">Вам следует решить, пропустить или обработать эти сигналы.</span><span class="sxs-lookup"><span data-stu-id="99127-170">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="99127-171">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="99127-171">Notification example</span></span>

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

<span data-ttu-id="99127-172">Обратите внимание на следующие моменты для этого типа уведомления.</span><span class="sxs-lookup"><span data-stu-id="99127-172">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="99127-173">`"lifecycleEvent": "missed"`Это поле указывает на сигнал о пропущенных уведомлениях об изменении.</span><span class="sxs-lookup"><span data-stu-id="99127-173">The `"lifecycleEvent": "missed"` field designates this as a signal about missed change notifications.</span></span> <span data-ttu-id="99127-174">Также возможны другие типы уведомлений жизненного цикла. В будущем будут добавлены новые типы.</span><span class="sxs-lookup"><span data-stu-id="99127-174">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="99127-175">В уведомлении о жизненном цикле не содержатся сведения об определенном ресурсе, так как он не связан с изменением ресурса, но с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="99127-175">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="99127-176">Как и в случае с уведомлениями об изменении, уведомления жизненного цикла могут объединяться в пакет (в массиве **значений** ) с разными значениями **лифецикливент** .</span><span class="sxs-lookup"><span data-stu-id="99127-176">Similar to change notifications, lifecycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="99127-177">Соответствующим образом обработайте каждое уведомление о жизненном цикле в пакете.</span><span class="sxs-lookup"><span data-stu-id="99127-177">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="99127-178">**Примечание:** полное описание данных, отправленных при доставке уведомлений об изменении, приведено в разделе [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="99127-178">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="99127-179">Выполняемые действия</span><span class="sxs-lookup"><span data-stu-id="99127-179">Actions to take</span></span>

1. <span data-ttu-id="99127-180">[Подтвердите](webhooks.md#change-notifications) получение уведомления о жизненном цикле, выполнив ответ на вызов Post `202 - Accepted` .</span><span class="sxs-lookup"><span data-stu-id="99127-180">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="99127-181">Если вы игнорируете эти сигналы, не выполняйте других действий.</span><span class="sxs-lookup"><span data-stu-id="99127-181">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="99127-182">В противном случае:</span><span class="sxs-lookup"><span data-stu-id="99127-182">Otherwise:</span></span>
2. <span data-ttu-id="99127-183">[Проверка](webhooks.md#change-notifications) подлинности уведомления о жизненном цикле.</span><span class="sxs-lookup"><span data-stu-id="99127-183">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="99127-184">Выполните полную повторную синхронизацию данных ресурса для выявления изменений, не доставленных в качестве уведомлений.</span><span class="sxs-lookup"><span data-stu-id="99127-184">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="99127-185">Готовый к изменениям код обработки уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="99127-185">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="99127-186">В будущем Microsoft Graph добавит дополнительные типы уведомлений о жизненном цикле подписки.</span><span class="sxs-lookup"><span data-stu-id="99127-186">In the future, Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="99127-187">Они будут публиковаться в той же конечной точке: **lifecycleNotificationUrl**, но у них будет другое значение для **lifecycleEvent**, и они могут содержать немного другую схему и свойства, относящиеся к сценарию, для которого они создаются.</span><span class="sxs-lookup"><span data-stu-id="99127-187">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="99127-188">Следует реализовать свой код с готовностью к будущим изменениям, чтобы он не прерывался, когда в Microsoft Graph вводятся новые типы уведомлений жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="99127-188">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="99127-189">Мы рекомендуем следующий подход:</span><span class="sxs-lookup"><span data-stu-id="99127-189">We recommend the following approach:</span></span>

1. <span data-ttu-id="99127-190">Явно определите каждое уведомление о жизненном цикле в качестве события, которое поддерживается, с помощью свойства **лифецикливент** .</span><span class="sxs-lookup"><span data-stu-id="99127-190">Explicitly identify each lifecycle notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="99127-191">Например, найдите свойство `"lifecycleEvent": "subscriptionRemoved"` для определения конкретного события и обработайте его.</span><span class="sxs-lookup"><span data-stu-id="99127-191">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="99127-192">Просмотрите объявления уведомлений о жизненном цикле для новых сценарионс.</span><span class="sxs-lookup"><span data-stu-id="99127-192">Watch for announcements of lifecycle notifications for new scenarions.</span></span> <span data-ttu-id="99127-193">В будущем может быть несколько типов уведомлений о жизненном цикле.</span><span class="sxs-lookup"><span data-stu-id="99127-193">There might be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="99127-194">В приложении игнорируйте все уведомления о жизненном цикле, которые приложение не распознает, и заносить их в журнал для получения сведений о состоянии.</span><span class="sxs-lookup"><span data-stu-id="99127-194">In your app, ignore any lifecycle notification that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="99127-195">По своему усмотрению просматривайте соответствующую документацию о новых уведомлениях жизненного цикла и реализуйте для них нужную поддержку.</span><span class="sxs-lookup"><span data-stu-id="99127-195">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="99127-196">См. также</span><span class="sxs-lookup"><span data-stu-id="99127-196">See also</span></span>

- [<span data-ttu-id="99127-197">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="99127-197">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="99127-198">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="99127-198">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="99127-199">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="99127-199">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="99127-200">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="99127-200">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="99127-201">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="99127-201">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
