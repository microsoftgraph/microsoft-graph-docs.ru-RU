---
title: Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)
description: Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Уведомления об изменениях могут включать свойства ресурсов.
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: eeff200c14b2da9039fecba39d7834c419e8caec
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598523"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a><span data-ttu-id="684cc-104">Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="684cc-104">Set up change notifications that include resource data (preview)</span></span>

<span data-ttu-id="684cc-105">Microsoft Graph позволяет приложениям подписываться на уведомления об изменениях ресурсов с использованием [веб-перехватчиков](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="684cc-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="684cc-106">Вы можете настроить подписки таким образом, чтобы в уведомления об изменениях включались данные измененных ресурсов (например, содержимое сообщения чата из Microsoft Teams или сведения о присутствии из Microsoft Teams).</span><span class="sxs-lookup"><span data-stu-id="684cc-106">You can set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message or Microsoft Teams presence information) in change notifications.</span></span> <span data-ttu-id="684cc-107">Затем приложение сможет запустить свою бизнес-логику без отдельного вызова API для получения измененного ресурса.</span><span class="sxs-lookup"><span data-stu-id="684cc-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="684cc-108">В результате приложение работает эффективнее, выполняя меньше вызовов API, что полезно в крупномасштабных сценариях.</span><span class="sxs-lookup"><span data-stu-id="684cc-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="684cc-109">Добавление данных ресурса в уведомления об изменениях требует реализации следующей дополнительной логики, чтобы выполнить требования по доступу к данным и их безопасности.</span><span class="sxs-lookup"><span data-stu-id="684cc-109">Including resource data as part of change notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="684cc-110">[Применяйте](#subscription-lifecycle-notifications) специальные уведомления жизненного цикла подписки, чтобы обеспечить непрерывный поток данных.</span><span class="sxs-lookup"><span data-stu-id="684cc-110">[Handle](#subscription-lifecycle-notifications) special subscription lifecycle notifications to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="684cc-111">Microsoft Graph периодически отправляет уведомления жизненного цикла, требуя от приложения повторной авторизации, чтобы обеспечить отсутствие неожиданных проблем с доступом при включении данных ресурсов в уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-111">Microsoft Graph sends lifecycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in change notifications.</span></span>
- <span data-ttu-id="684cc-112">[Проверяйте](#validating-the-authenticity-of-notifications) подлинность уведомлений об изменениях, подтверждая что их источником является Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="684cc-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of change notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="684cc-113">[Предоставьте](#decrypting-resource-data-from-change-notifications) открытый ключ шифрования и используйте закрытый ключ для расшифровки данных ресурсов, полученных в уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through change notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="684cc-114">Сведения ресурсов в полезных данных уведомлений</span><span class="sxs-lookup"><span data-stu-id="684cc-114">Resource data in notification payload</span></span>

<span data-ttu-id="684cc-115">Обычно этот тип уведомлений об изменениях содержит следующие сведения ресурсов в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="684cc-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="684cc-116">Идентификатор и тип измененного экземпляра ресурса, возвращаемые в свойстве **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="684cc-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="684cc-117">Все значения свойств экземпляра ресурса, зашифрованные в соответствии с подпиской и возвращаемые в свойстве **encryptedContent**.</span><span class="sxs-lookup"><span data-stu-id="684cc-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="684cc-118">Или зависимые от ресурса определенные свойства, возвращаемые в свойстве **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="684cc-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="684cc-119">Чтобы получить только определенные свойства, их нужно указать в URL-адресе объекта **resource** в подписке, используя параметр `$select`.</span><span class="sxs-lookup"><span data-stu-id="684cc-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="684cc-120">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="684cc-120">Supported resources</span></span>

<span data-ttu-id="684cc-121">В настоящее время ресурсы [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (предварительная версия) и [presence](/graph/api/resources/presence?view=graph-rest-beta) (предварительная версия) в Microsoft Teams поддерживают уведомления об изменениях, включающие данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="684cc-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (preview) as well as the Microsoft Teams [presence](/graph/api/resources/presence?view=graph-rest-beta) (preview) resources supports change notifications that include resource data.</span></span> <span data-ttu-id="684cc-122">В частности, вы можете настроить подписку, относящуюся к одному из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="684cc-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="684cc-123">Новые или измененные сообщения в определенном канале Teams: `/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="684cc-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="684cc-124">Новые или измененные сообщения в определенном чате Teams: `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="684cc-124">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>
- <span data-ttu-id="684cc-125">Обновление сведений о присутствии пользователя: `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="684cc-125">User's presence information update: `/communications/presences/{id}`</span></span>

<span data-ttu-id="684cc-126">Ресурсы **chatMessage** и **presence** поддерживают включение в уведомление об изменениях всех свойств измененного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="684cc-126">The **chatMessage** and the **presence** resources support including all the properties of a changed instance in a change notification.</span></span> <span data-ttu-id="684cc-127">Они не поддерживают возвращение только выбранных свойств экземпляра.</span><span class="sxs-lookup"><span data-stu-id="684cc-127">They do not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="684cc-128">В этой статье рассматривается пример подписки на уведомления об изменениях в канале Teams. При этом каждое уведомление об изменении содержит все данные ресурсов измененного экземпляра **chatMessage**.</span><span class="sxs-lookup"><span data-stu-id="684cc-128">This article walks through an example of subscribing to change notifications of messages in a Teams channel, with each change notification including the full resource data of the changed **chatMessage** instance.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="684cc-129">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-129">Creating a subscription</span></span>

<span data-ttu-id="684cc-130">Чтобы включить данные ресурсов в уведомления об изменениях, **требуется** указать следующие свойства в дополнение к обычно указываемым при [создании подписки](webhooks.md#creating-a-subscription):</span><span class="sxs-lookup"><span data-stu-id="684cc-130">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="684cc-131">**includeResourceData**, которому следует присвоить значение `true`, чтобы явно запросить данные ресурса.</span><span class="sxs-lookup"><span data-stu-id="684cc-131">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="684cc-132">**lifecycleNotificationUrl**, являющееся конечной точкой, в которую доставляются [уведомления жизненного цикла](#subscription-lifecycle-notifications).</span><span class="sxs-lookup"><span data-stu-id="684cc-132">**lifecycleNotificationUrl** which is an endpoint where [lifecycle notifications](#subscription-lifecycle-notifications) are delivered.</span></span> <span data-ttu-id="684cc-133">Оно может совпадать с **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="684cc-133">This can be the same or different as **notificationUrl**.</span></span>
- <span data-ttu-id="684cc-134">**encryptionCertificate**, содержащее только открытый ключ, используемый Microsoft Graph для шифрования данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="684cc-134">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="684cc-135">Сохраняйте соответствующий закрытый ключ для [расшифровки контента](#decrypting-resource-data-from-change-notifications).</span><span class="sxs-lookup"><span data-stu-id="684cc-135">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="684cc-136">**encryptionCertificateId**, являющееся вашим собственным идентификатором для сертификата.</span><span class="sxs-lookup"><span data-stu-id="684cc-136">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="684cc-137">Используйте этот идентификатор для определения в каждом уведомлении об изменениях сертификата, используемого для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="684cc-137">Use this ID to match in each change notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="684cc-138">Учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="684cc-138">Keep the following in mind:</span></span>

- <span data-ttu-id="684cc-139">Используйте одинаковое имя узла для обеих конечных точек уведомлений об изменениях (**notificationUrl** и **lifecycleNotificationUrl**).</span><span class="sxs-lookup"><span data-stu-id="684cc-139">Use the same host name for both change notification endpoints (**notificationUrl** and **lifecycleNotificationUrl**).</span></span>
- <span data-ttu-id="684cc-140">Проверьте обе конечные точки, как описано [здесь](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="684cc-140">Validate both endpoints as described [here](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="684cc-141">Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.</span><span class="sxs-lookup"><span data-stu-id="684cc-141">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>
- <span data-ttu-id="684cc-142">Вы не сможете обновить (`PATCH`) существующую подписку, чтобы добавить свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="684cc-142">You cannot update (`PATCH`) an existing subscription to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="684cc-143">Следует удалить существующую подписку и создать новую, чтобы указать свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="684cc-143">You should remove the existing subscription, and create a new subscription to include the **lifecycleNotificationUrl** property.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="684cc-144">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="684cc-144">Subscription request example</span></span>

<span data-ttu-id="684cc-145">В примере ниже выполняется подписка на два типа уведомлений:</span><span class="sxs-lookup"><span data-stu-id="684cc-145">The following example subscribes to two types of notifications:</span></span> 

- <span data-ttu-id="684cc-146">Изменения ресурсов — создание или обновление сообщений каналов в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="684cc-146">Resource changes - channel messages being created or updated in Microsoft Teams</span></span>
- <span data-ttu-id="684cc-147">События жизненного цикла подписки, которые могут влиять на поток уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-147">Subscription lifecycle events which can affect the flow of change notifications.</span></span> <span data-ttu-id="684cc-148">Дополнительные сведения об уведомлениях жизненного цикла см. в [следующем разделе](#subscription-lifecycle-notifications).</span><span class="sxs-lookup"><span data-stu-id="684cc-148">See more details about lifecycle notifications in the [next section](#subscription-lifecycle-notifications).</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a><span data-ttu-id="684cc-149">Отклик подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-149">Subscription response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications"></a><span data-ttu-id="684cc-150">Уведомления жизненного цикла подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-150">Subscription lifecycle notifications</span></span>

<span data-ttu-id="684cc-151">Некоторые события могут воздействовать на поток уведомлений об изменениях в существующей подписке.</span><span class="sxs-lookup"><span data-stu-id="684cc-151">Certain events can interfere with change notification flow in an existing subscription.</span></span> <span data-ttu-id="684cc-152">Уведомления жизненного цикла подписки указывают необходимые действия для обеспечения непрерывного потока.</span><span class="sxs-lookup"><span data-stu-id="684cc-152">Subscription lifecycle notifications inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="684cc-153">В отличие от уведомления об изменении ресурса, информирующем об изменении экземпляра ресурса, уведомление жизненного цикла относится к самой подписке и ее текущему состоянию в жизненном цикле.</span><span class="sxs-lookup"><span data-stu-id="684cc-153">Unlike a resource change notification which informs a change to a resource instance, a lifecycle notification is about the subscription itself, and its current state in the lifecycle.</span></span> 

<span data-ttu-id="684cc-154">Уведомления жизненного цикла доставляются в объект **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="684cc-154">Lifecycle notifications are delivered to the **lifecycleNotificationUrl**.</span></span> 

<span data-ttu-id="684cc-155">Содержание:</span><span class="sxs-lookup"><span data-stu-id="684cc-155">In this section:</span></span>

- [<span data-ttu-id="684cc-156">Уведомление жизненного цикла, запрашивающее авторизацию подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-156">Lifecycle notification that challenges subscription authorization</span></span>](#lifecycle-notification-that-challenges-subscription-authorization)
- [<span data-ttu-id="684cc-157">Поток запроса авторизации</span><span class="sxs-lookup"><span data-stu-id="684cc-157">Authorization challenge flow</span></span>](#authorization-challenge-flow)
- [<span data-ttu-id="684cc-158">Пример запроса авторизации</span><span class="sxs-lookup"><span data-stu-id="684cc-158">Example authorization challenge</span></span>](#example-authorization-challenge)
- [<span data-ttu-id="684cc-159">Ответ на запрос авторизации</span><span class="sxs-lookup"><span data-stu-id="684cc-159">Responding to an authorization challenge</span></span>](#responding-to-an-authorization-challenge)
- [<span data-ttu-id="684cc-160">Советы</span><span class="sxs-lookup"><span data-stu-id="684cc-160">Tips</span></span>](#tips)
- [<span data-ttu-id="684cc-161">Подготовка к изменениям кода для обработки других типов уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="684cc-161">Future-proof your code to handle other types of lifecycle notifications</span></span>](#future-proof-your-code-to-handle-other-types-of-lifecycle-notifications)

### <a name="lifecycle-notification-that-challenges-subscription-authorization"></a><span data-ttu-id="684cc-162">Уведомление жизненного цикла, запрашивающее авторизацию подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-162">Lifecycle notification that challenges subscription authorization</span></span>

<span data-ttu-id="684cc-163">Один из типов уведомлений жизненного цикла запрашивает авторизованное состояние активной подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-163">One type of lifecycle notifications challenges the authorized state of an active subscription.</span></span> <span data-ttu-id="684cc-164">Если в свойстве **lifecycleEvent** уведомления указано значение `reauthorizationRequired`, требуется повторно авторизовать подписку, чтобы поток данных не прерывался.</span><span class="sxs-lookup"><span data-stu-id="684cc-164">When the **lifecycleEvent** property in a notification indicates `reauthorizationRequired`, you must re-authorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="684cc-165">При создании долгосрочной подписки (например, длительностью 3 дня) уведомления об изменениях направляются в расположение, указанное в свойстве **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="684cc-165">When you create a long-lived subscription (for example, one that lasts for 3 days), change notifications flows to the location indicated in **notificationUrl**.</span></span> <span data-ttu-id="684cc-166">Однако в любой момент Microsoft Graph может потребовать повторную авторизацию подписки, чтобы подтвердить наличие у вас доступа к данным ресурсов в случае изменения условий доступа с момента создания подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-166">However, at any point in time, Microsoft Graph may require that you re-authorize the subscription to prove that you still have access to resource data, in case the conditions of access have changed since the subscription was created.</span></span> <span data-ttu-id="684cc-167">Ниже приведены примеры изменений, влияющих на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="684cc-167">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="684cc-168">Администратор клиента может отозвать разрешения приложения на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="684cc-168">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="684cc-169">В интерактивном сценарии к пользователю, предоставляющему маркер проверки подлинности для вашего приложения, могут применяться динамические политики на основе различных факторов, например их расположения, состояния устройства или оценки риска.</span><span class="sxs-lookup"><span data-stu-id="684cc-169">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="684cc-170">Например, если пользователь изменяет свое физическое расположение, ему может быть запрещен доступ к данным, и ваше приложение не сможет повторно авторизовать подписку.</span><span class="sxs-lookup"><span data-stu-id="684cc-170">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to re-authorize the subscription.</span></span> <span data-ttu-id="684cc-171">Дополнительные сведения о динамических политиках, управляющих доступом, см. в статье [Политики условного доступа Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="684cc-171">For more information on dynamic policies that control access, see [Azure AD conditional access policies](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span></span> 

### <a name="authorization-challenge-flow"></a><span data-ttu-id="684cc-172">Поток запроса авторизации</span><span class="sxs-lookup"><span data-stu-id="684cc-172">Authorization challenge flow</span></span>

<span data-ttu-id="684cc-173">Поток запроса авторизации для активной подписки с неистекшим сроком действия выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="684cc-173">The flow of an authorization challenge for an active, non-expired subscription looks as follows:</span></span>

1. <span data-ttu-id="684cc-174">Microsoft Graph требует повторной авторизации подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-174">Microsoft Graph requires a subscription to be re-authorized</span></span>
    
    <span data-ttu-id="684cc-175">Причины этого могут отличаться для разных ресурсов и меняться со временем.</span><span class="sxs-lookup"><span data-stu-id="684cc-175">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="684cc-176">Независимо от причины события повторной авторизации вам потребуется отреагировать на него.</span><span class="sxs-lookup"><span data-stu-id="684cc-176">Regardless of the cause of the re-authorization event, you will need to respond to it.</span></span>

2. <span data-ttu-id="684cc-177">Microsoft Graph отправляет уведомление о запросе авторизации в **lifecycleNotificationUrl**</span><span class="sxs-lookup"><span data-stu-id="684cc-177">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**</span></span>

    <span data-ttu-id="684cc-178">Обратите внимание, что поток уведомлений об изменениях может некоторое время продолжаться, предоставляя вам дополнительное время для ответа.</span><span class="sxs-lookup"><span data-stu-id="684cc-178">Note that the flow of change notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="684cc-179">Однако в конечном итоге доставка уведомлений об изменениях будет приостановлена, пока вы не выполните требуемое действие.</span><span class="sxs-lookup"><span data-stu-id="684cc-179">However, eventually change notification delivery will pause, until you take the required action.</span></span>

3. <span data-ttu-id="684cc-180">Ответьте на это уведомление жизненного цикла одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="684cc-180">Respond to this lifecycle notification in one of two ways:</span></span>
    1. <span data-ttu-id="684cc-181">Повторная авторизация подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-181">Re-authorize the subscription.</span></span> <span data-ttu-id="684cc-182">Это не продлевает срок действия подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-182">This does not extend the expiry date of the subscription.</span></span>
    2. <span data-ttu-id="684cc-183">Возобновление подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-183">Renew the subscription.</span></span> <span data-ttu-id="684cc-184">Это повторно авторизует подписку и продлевает срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="684cc-184">This both re-authorizes and extends the expiry date.</span></span>

    <span data-ttu-id="684cc-185">Примечание. Оба действия требуют предоставление действительного маркера проверки подлинности по аналогии с [созданием новой подписки](webhooks.md#creating-a-subscription) или [продлением подписки до истечения срока ее действия](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="684cc-185">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="684cc-186">Если вы успешно выполнили повторную авторизацию или возобновление подписки, уведомления об изменениях продолжать поступать.</span><span class="sxs-lookup"><span data-stu-id="684cc-186">If you successfully re-authorize or renew the subscription, change notifications continue.</span></span> <span data-ttu-id="684cc-187">В противном случае уведомления об изменениях не будут возобновлены.</span><span class="sxs-lookup"><span data-stu-id="684cc-187">Otherwise, change notifications remain paused.</span></span>
    
### <a name="example-authorization-challenge"></a><span data-ttu-id="684cc-188">Пример запроса авторизации</span><span class="sxs-lookup"><span data-stu-id="684cc-188">Example authorization challenge</span></span>

<span data-ttu-id="684cc-189">Ниже представлен пример уведомления жизненного цикла, запрашивающего повторную авторизацию подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-189">Below is an example lifecycle notification that requests re-authorizing a subscription.</span></span> 

<span data-ttu-id="684cc-190">Обратите внимание на следующее:</span><span class="sxs-lookup"><span data-stu-id="684cc-190">Note the following:</span></span>

- <span data-ttu-id="684cc-191">Поле `"lifecycleEvent": "reauthorizationRequired"` определяет это уведомление как запрос авторизации.</span><span class="sxs-lookup"><span data-stu-id="684cc-191">The `"lifecycleEvent": "reauthorizationRequired"` field identifies this notification as an authorization challenge.</span></span>
- <span data-ttu-id="684cc-192">Это уведомление жизненного цикла не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-192">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="684cc-193">Как и уведомления об изменениях, уведомления жизненного цикла можно объединять (в коллекции **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="684cc-193">Similar to change notifications, you can batch lifecycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="684cc-194">Обрабатывайте каждое уведомление жизненного цикла в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="684cc-194">Process each lifecycle notification in the batch accordingly.</span></span>

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

> <span data-ttu-id="684cc-195">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="684cc-195">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="responding-to-an-authorization-challenge"></a><span data-ttu-id="684cc-196">Ответ на запрос авторизации</span><span class="sxs-lookup"><span data-stu-id="684cc-196">Responding to an authorization challenge</span></span>

<span data-ttu-id="684cc-197">Чтобы обработать уведомление жизненного цикла с запросом авторизации, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="684cc-197">Take the following steps to process an authorization challenge lifecycle notification.</span></span> <span data-ttu-id="684cc-198">Первые два действия по подтверждению и проверке уведомления жизненного цикла аналогичны [ответу на уведомление об изменении ресурса](webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="684cc-198">The first two steps of acknowledging and validating the lifecycle notification is similar to [responding to a resource change notification](webhooks.md#processing-the-change-notification).</span></span>

1. <span data-ttu-id="684cc-199">Подтвердите получение уведомления жизненного цикла, ответив на вызов POST с помощью `HTTP 202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="684cc-199">Acknowledge the receipt of the lifecycle notification, by responding to the POST call with `HTTP 202 Accepted`.</span></span>
2. <span data-ttu-id="684cc-200">Проверьте подлинность уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="684cc-200">Validate the authenticity of the lifecycle notification.</span></span> <span data-ttu-id="684cc-201">Дополнительные сведения см. [ниже](#validating-the-authenticity-of-notifications).</span><span class="sxs-lookup"><span data-stu-id="684cc-201">Further details [below](#validating-the-authenticity-of-notifications).</span></span>
3. <span data-ttu-id="684cc-202">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="684cc-202">Ensure the app has a valid access token to take the next step.</span></span> 

    <span data-ttu-id="684cc-203">Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), библиотека сделает это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, попросив пользователя повторно войти с помощью нового пароля.</span><span class="sxs-lookup"><span data-stu-id="684cc-203">If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), the library handles this for you by either reusing a valid cached token, or obtaining a new token from prompting the user to log in again with a new password.</span></span> <span data-ttu-id="684cc-204">Однако получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и пользователю больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="684cc-204">However, obtaining a new token may fail, since the conditions of access may have changed, and the user may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="684cc-205">Вызовите один из двух следующих API.</span><span class="sxs-lookup"><span data-stu-id="684cc-205">Call either of the following two APIs.</span></span> <span data-ttu-id="684cc-206">Если вызов API выполняется успешно, поток уведомлений об изменениях возобновляется.</span><span class="sxs-lookup"><span data-stu-id="684cc-206">If the API call succeeds, the change notification flow resumes.</span></span>

    - <span data-ttu-id="684cc-207">Чтобы повторно авторизовать подписку без продления ее срока, вызовите действие `/reauthorize`:</span><span class="sxs-lookup"><span data-stu-id="684cc-207">Call the `/reauthorize` action to re-authorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="684cc-208">Чтобы одновременно возобновить и повторно авторизовать подписку, выполните обычное действие возобновления:</span><span class="sxs-lookup"><span data-stu-id="684cc-208">Perform a regular renew action to re-authorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="684cc-209">Возобновление может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="684cc-209">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="684cc-210">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-210">It may be necessary for the app to obtain a new access token from the user to successfully re-authorize a subscription.</span></span> 
      
      <span data-ttu-id="684cc-211">Вы может повторить эти действия позднее в любое время и успешно выполнить их, если изменяются условия доступа.</span><span class="sxs-lookup"><span data-stu-id="684cc-211">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="684cc-212">Все уведомления об изменении ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="684cc-212">Any notifications about resource changes that happen between the time the lifecycle notification was sent, and the time when the app eventually re-creates the subscription successfully, would be lost.</span></span> <span data-ttu-id="684cc-213">В таких случаях приложению нужно отдельно получить эти изменения.</span><span class="sxs-lookup"><span data-stu-id="684cc-213">In such cases, the app should separately fetch those changes.</span></span>

### <a name="tips"></a><span data-ttu-id="684cc-214">Советы </span><span class="sxs-lookup"><span data-stu-id="684cc-214">Tips</span></span>

<span data-ttu-id="684cc-215">Учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="684cc-215">Keep the following in mind:</span></span>

1. <span data-ttu-id="684cc-216">Запросы авторизации не отменяют необходимость возобновления подписки на изменения ресурса до истечения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="684cc-216">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="684cc-217">Хотя вы можете возобновить подписку при получении запроса авторизации, Microsoft Graph может не выполнять запрос для всех ваших подписок.</span><span class="sxs-lookup"><span data-stu-id="684cc-217">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="684cc-218">Например, подписка без действий и уведомлений об изменениях, ожидающих доставки, может не создавать для приложения запросы на повторную авторизацию.</span><span class="sxs-lookup"><span data-stu-id="684cc-218">For example, a subscription that does not have any activity and has no change notifications pending delivery may not signal any re-authorization challenges to your app.</span></span> <span data-ttu-id="684cc-219">Обязательно [возобновите подписки](webhooks.md#renewing-a-subscription) до истечения их сроков действия.</span><span class="sxs-lookup"><span data-stu-id="684cc-219">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

2. <span data-ttu-id="684cc-220">Частота запросов авторизации может изменяться.</span><span class="sxs-lookup"><span data-stu-id="684cc-220">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="684cc-221">Не делайте предположений о частоте запросов авторизации.</span><span class="sxs-lookup"><span data-stu-id="684cc-221">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="684cc-222">Эти уведомления жизненного цикла сообщают, когда нужно принимать действия, избавляя от отслеживания подписок, которым требуется повторная авторизация.</span><span class="sxs-lookup"><span data-stu-id="684cc-222">These lifecycle notifications tell you when to take actions, saving you from having to track which subscriptions require re-authorization.</span></span> <span data-ttu-id="684cc-223">Будьте готовы обрабатывать запросы авторизации каждые несколько минут для всех подписок или в редких случаях лишь для некоторых подписок.</span><span class="sxs-lookup"><span data-stu-id="684cc-223">Be ready to handle authorization challenges anywhere from once a few minutes for every subscription, to rarely for only some of your subscriptions.</span></span>

### <a name="future-proof-your-code-to-handle-other-types-of-lifecycle-notifications"></a><span data-ttu-id="684cc-224">Подготовка к изменениям кода для обработки других типов уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="684cc-224">Future-proof your code to handle other types of lifecycle notifications</span></span>

<span data-ttu-id="684cc-225">Ожидайте публикацию уведомлений жизненного цикла подписки в конечной точке, указанной в **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="684cc-225">Expect subscription lifecycle notifications to be posted to the same endpoint specified by **lifecycleNotificationUrl**.</span></span> <span data-ttu-id="684cc-226">Они отличаются свойством **lifecycleEvent** и могут содержать немного другую схему и свойства для обслуживания своих сценариев.</span><span class="sxs-lookup"><span data-stu-id="684cc-226">They differentiate by the **lifecycleEvent** property and may contain slightly different schema and properties to serve the scenarios they address.</span></span>

<span data-ttu-id="684cc-227">Применяйте свой код, предполагая новые типы уведомлений жизненного цикла:</span><span class="sxs-lookup"><span data-stu-id="684cc-227">Implement your code in anticipation of new types of lifecycle notifications:</span></span>

1. <span data-ttu-id="684cc-228">Используйте свойство **lifecycleEvent**, чтобы указать тип уведомления для определения соответствующего ответа.</span><span class="sxs-lookup"><span data-stu-id="684cc-228">Use the **lifecycleEvent** property to identify the type of notification so to determine the appropriate response.</span></span> <span data-ttu-id="684cc-229">Например, найдите свойство `"lifecycleEvent": "reauthorizationRequired"` для определения конкретного события и обработайте его.</span><span class="sxs-lookup"><span data-stu-id="684cc-229">For example, look for the `"lifecycleEvent": "reauthorizationRequired"` property to identify a specific event, and handle it.</span></span>

1. <span data-ttu-id="684cc-230">Регистрируйте все события жизненного цикла, не распознанные вашим приложением, чтобы получить сведения о них.</span><span class="sxs-lookup"><span data-stu-id="684cc-230">Log any lifecycle events that your app does not recognize to gain awareness.</span></span>

1. <span data-ttu-id="684cc-231">Подпишитесь на [блог разработчика Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы следить за объявлениями об уведомлениях жизненного цикла для новых сценариев.</span><span class="sxs-lookup"><span data-stu-id="684cc-231">Subscribe to the [Microsoft Graph Developer Blog](https://developer.microsoft.com/graph/blogs/) to watch for announcements of lifecycle notifications for new scenarios.</span></span>

1. <span data-ttu-id="684cc-232">Просматривайте соответствующую документацию о новых уведомлениях жизненного цикла и реализуйте для них нужную поддержку.</span><span class="sxs-lookup"><span data-stu-id="684cc-232">Look up related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="684cc-233">Проверка подлинности уведомлений</span><span class="sxs-lookup"><span data-stu-id="684cc-233">Validating the authenticity of notifications</span></span>

<span data-ttu-id="684cc-234">Приложения часто выполняют бизнес-логику на основе данных ресурсов, включенных в уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-234">Apps often execute business logic based on resource data included in change notifications.</span></span> <span data-ttu-id="684cc-235">Важно сначала проверить подлинность каждого уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-235">Having first verified the authenticity of each change notification is important.</span></span> <span data-ttu-id="684cc-236">В противном случае посторонние смогут обмануть ваше приложение с помощью ложных уведомлений об изменениях, заставить его неправильно выполнять бизнес-логику и привести к нарушению безопасности.</span><span class="sxs-lookup"><span data-stu-id="684cc-236">Otherwise, a third party could spoof your app with false change notifications, make it execute its business logic incorrectly, and lead to a security incident.</span></span>

<span data-ttu-id="684cc-237">Для основных уведомлений об изменениях, не содержащих данные ресурсов, просто проверьте их на основе значения **clientState**, как описано [здесь](webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="684cc-237">For basic change notifications which do not contain resource data, simply validate them based on the **clientState** value as described [here](webhooks.md#processing-the-change-notification).</span></span> <span data-ttu-id="684cc-238">Это приемлемо, так как вы можете выполнять последующие надежные вызовы Microsoft Graph, чтобы получить доступ к данным ресурсов и, следовательно, влияние любых попыток подмены ограничено.</span><span class="sxs-lookup"><span data-stu-id="684cc-238">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="684cc-239">Для уведомлений об изменениях, доставляющих данные ресурсов, проведите более тщательную проверку перед обработкой данных.</span><span class="sxs-lookup"><span data-stu-id="684cc-239">For change notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="684cc-240">Содержание:</span><span class="sxs-lookup"><span data-stu-id="684cc-240">In this section:</span></span>

- [<span data-ttu-id="684cc-241">Маркеры проверки в уведомлении об изменениях</span><span class="sxs-lookup"><span data-stu-id="684cc-241">Validation tokens in the change notification</span></span>](#validation-tokens-in-the-change-notification)
- [<span data-ttu-id="684cc-242">Способ проверки</span><span class="sxs-lookup"><span data-stu-id="684cc-242">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="684cc-243">Пример маркера JWT</span><span class="sxs-lookup"><span data-stu-id="684cc-243">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a><span data-ttu-id="684cc-244">Маркеры проверки в уведомлении об изменениях</span><span class="sxs-lookup"><span data-stu-id="684cc-244">Validation tokens in the change notification</span></span>

<span data-ttu-id="684cc-245">Уведомление об изменениях с данными ресурсов содержит дополнительное свойство **validationTokens**, содержащее массив маркеров JWT, созданных Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="684cc-245">A change notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="684cc-246">Microsoft Graph создает один маркер для каждой отдельной пары приложения и клиента, для которой существует элемент в массиве **value**.</span><span class="sxs-lookup"><span data-stu-id="684cc-246">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="684cc-247">Учитывайте, что уведомления об изменениях могут содержать разные элементы для различных приложений и клиентов, подписанных с помощью одинакового значения **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="684cc-247">Keep in mind that change notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="684cc-248">В следующем примере уведомление об изменении содержит два элемента для одного приложения и двух разных клиентов, поэтому массив **validationTokens** содержит два маркера, требующих проверки.</span><span class="sxs-lookup"><span data-stu-id="684cc-248">In the following example, the change notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

```json
{
    "value": [
          {
            "subscriptionId": "76619225-ff6b-4489-96ca-4ef547e78b22",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
            "changeType": "created",
            ...
          },
      {
            "subscriptionId": "e990d58f-fd93-40af-acf7-a7c907c5d8ea",
      "tenantId": "46d9e3bd-6309-4177-a016-b256a411e30f",
            "changeType": "created",
            ...
            }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhb...",
    "cGlkYWNyIjoiMiIsImlkc..."
    ]
}
```

> <span data-ttu-id="684cc-249">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="684cc-249">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="how-to-validate"></a><span data-ttu-id="684cc-250">Способ проверки</span><span class="sxs-lookup"><span data-stu-id="684cc-250">How to validate</span></span>

<span data-ttu-id="684cc-251">Если вы незнакомы с проверкой маркеров, см. обзор в статье [Принципы проверки маркера](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/).</span><span class="sxs-lookup"><span data-stu-id="684cc-251">If you're new to token validation, see [Principles of Token Validation](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for an overview.</span></span> <span data-ttu-id="684cc-252">Используйте пакет SDK, например библиотеку [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) для .NET или стороннюю библиотеку для другой платформы.</span><span class="sxs-lookup"><span data-stu-id="684cc-252">Use an SDK, such as the [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third-party library for a different platform.</span></span>

<span data-ttu-id="684cc-253">Следует учитывать следующее:</span><span class="sxs-lookup"><span data-stu-id="684cc-253">Be mindful of the following:</span></span> 

- <span data-ttu-id="684cc-254">Всегда отправляйте код состояния `HTTP 202 Accepted` в ответе на уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="684cc-254">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the change notification.</span></span> 
- <span data-ttu-id="684cc-255">Делайте это перед проверкой уведомления об изменении (например, если вы храните уведомления об изменениях в очередях для последующей обработки) или после нее (если они обрабатываются на ходу), даже если проверка завершилась сбоем.</span><span class="sxs-lookup"><span data-stu-id="684cc-255">Do that before validating the change notification (for example, if you store change notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="684cc-256">Принятие уведомления об изменении позволяет избежать ненужных повторений доставки, а также мешает любым возможным злоумышленникам выяснить, прошли ли они проверку.</span><span class="sxs-lookup"><span data-stu-id="684cc-256">Accepting a change notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="684cc-257">Вы всегда можете игнорировать неверное уведомление об изменении после его принятия.</span><span class="sxs-lookup"><span data-stu-id="684cc-257">You can always choose to ignore an invalid change notification after you have accepted it.</span></span>

<span data-ttu-id="684cc-258">В частности, выполняйте проверку каждого маркера JWT в коллекции **validationTokens**.</span><span class="sxs-lookup"><span data-stu-id="684cc-258">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="684cc-259">Если любой из маркеров не прошел проверку, считайте уведомление об изменении подозрительным и выполните дальнейшее исследование.</span><span class="sxs-lookup"><span data-stu-id="684cc-259">If any tokens fail, consider the change notification suspicious and investigate further.</span></span> 

<span data-ttu-id="684cc-260">Для проверки маркеров и приложений, создающих маркеры, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="684cc-260">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="684cc-261">Убедитесь, что срок действия маркера не истек.</span><span class="sxs-lookup"><span data-stu-id="684cc-261">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="684cc-262">Проверьте, что маркер не был подделан и был выдан ожидаемым центром авторизации (Microsoft Azure Active Directory):</span><span class="sxs-lookup"><span data-stu-id="684cc-262">Validate the token has not been tampered with and was issued by the expected authority, Microsoft Azure Active Directory:</span></span>

    - <span data-ttu-id="684cc-263">Получите ключи подписи от общей конечной точки конфигурации: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span><span class="sxs-lookup"><span data-stu-id="684cc-263">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="684cc-264">Эта конфигурация кэшируется приложением на определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="684cc-264">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="684cc-265">Имейте в виду, что конфигурация часто обновляется, так как ключи входа ежедневно меняются.</span><span class="sxs-lookup"><span data-stu-id="684cc-265">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="684cc-266">Проверьте подпись маркера JWT, использующего эти ключи.</span><span class="sxs-lookup"><span data-stu-id="684cc-266">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="684cc-267">Не принимайте маркеры, выпущенные любыми другими центрами.</span><span class="sxs-lookup"><span data-stu-id="684cc-267">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="684cc-268">Проверьте, что маркер выпущен для вашего приложения, подписавшегося на уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-268">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="684cc-269">Следующие действия являются частью стандартной логики проверки в библиотеках маркеров JWT, и обычно их можно выполнять в виде вызова одной функции.</span><span class="sxs-lookup"><span data-stu-id="684cc-269">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="684cc-270">Убедитесь, что "аудитория" в маркере совпадает с идентификатором вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="684cc-270">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="684cc-271">Если уведомления об изменениях получают несколько приложений, выполните проверку по нескольким идентификаторам.</span><span class="sxs-lookup"><span data-stu-id="684cc-271">If you have more than one app receiving change notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="684cc-272">**Важно**. Убедитесь, что приложение, создавшее маркер, представляет издателя уведомления об изменениях Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="684cc-272">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="684cc-273">Проверьте, что свойство **appid** в маркере соответствует ожидаемому значению `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span><span class="sxs-lookup"><span data-stu-id="684cc-273">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="684cc-274">Это гарантирует, что уведомления об изменениях не отправляются другим приложением, отличным от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="684cc-274">This ensures that change notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="684cc-275">Пример маркера JWT</span><span class="sxs-lookup"><span data-stu-id="684cc-275">Example JWT token</span></span>

<span data-ttu-id="684cc-276">Ниже приведен пример свойств, входящих в маркер JWT, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="684cc-276">The following is an example of the properties included in the JWT token that are needed for validation.</span></span>

```json
{
  // aud is your app's id 
  "aud": "8e460676-ae3f-4b1e-8790-ee0fb5d6148f",                           
  "iss": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "iat": 1565046813,
  "nbf": 1565046813,
  // Expiration date 
  "exp": 1565075913,                                                        
  "aio": "42FgYKhZ+uOZrHa7p+7tfruauq1HAA==",
  // appid represents the notification publisher and must always be the same value of 0bf30f3b-4a52-48df-9a82-234910c4a086 
  "appid": "0bf30f3b-4a52-48df-9a82-234910c4a086",                          
  "appidacr": "2",
  "idp": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "tid": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
  "uti": "-KoJHevhgEGnN4kwuixpAA",
  "ver": "1.0"
}
```

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="684cc-277">Пример: подтверждение маркеров проверки</span><span class="sxs-lookup"><span data-stu-id="684cc-277">Example: Verifying validation tokens</span></span>

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
    var openIdConfig = await configurationManager.GetConfigurationAsync();
    var handler = new JwtSecurityTokenHandler();
    try
    {
    handler.ValidateToken(token, new TokenValidationParameters
    {
        ValidateIssuer = true,
        ValidateAudience = true,
        ValidateIssuerSigningKey = true,
        ValidateLifetime = true,
        ValidIssuer = $"https://sts.windows.net/{tenantId}/",
        ValidAudiences = appIds,
        IssuerSigningKeys = openIdConfig.SigningKeys
    }, out _);
    return true;
    }
    catch (Exception ex)
    {
    Trace.TraceError($"{ex.Message}:{ex.StackTrace}");
    return false;
    }
}
```
```java
private boolean IsValidationTokenValid(String[] appIds, String tenantId, String serializedToken) {
    try {
        JwkKeyResolver jwksResolver = new JwkKeyResolver();
        Jws<Claims> token = Jwts.parserBuilder()
        .setSigningKeyResolver(jwksResolver)
        .build()
        .parseClaimsJws(serializedToken);
        Claims body = token.getBody();
        String audience = body.getAudience();
        boolean isAudienceValid = false;
        for(String appId : appIds) {
        isAudienceValid = isAudienceValid || appId.equals(audience);
        }
        boolean isTenantValid = body.getIssuer().endsWith(tenantId + "/");
        return isAudienceValid  && isTenantValid; //nbf,exp and signature are already validated by library
    } catch (Exception e) {
        LOGGER.error("could not validate token");
        LOGGER.error(e.getMessage());
        return false;
    }
}
```
```JavaScript
import jwt from 'jsonwebtoken';
import jkwsClient from 'jwks-rsa';

const client = jkwsClient({
  jwksUri: 'https://login.microsoftonline.com/common/discovery/v2.0/keys'
});

export function getKey(header, callback) {
  client.getSigningKey(header.kid, (err, key) => {
    var signingKey = key.publicKey || key.rsaPublicKey;
    callback(null, signingKey);
  });
}

export function isTokenValid(token, appId, tenantId) {
  return new Promise((resolve) => {
    const options = {
      audience: [appId],
      issuer: [`https://sts.windows.net/${tenantId}/`]
    };
    jwt.verify(token, getKey, options, (err) => {
      if (err) {
        // eslint-disable-next-line no-console
        console.error(err);
        resolve(false);
      } else {
        resolve(true);
      }
    });
  });
}
```
<span data-ttu-id="684cc-278">Чтобы пример Java работал, вам также необходимо реализовать `JwkKeyResolver`.</span><span class="sxs-lookup"><span data-stu-id="684cc-278">For the Java sample to work, you will also need to implement the `JwkKeyResolver`.</span></span>  
```java
package com.example.restservice;

import com.auth0.jwk.JwkProvider;
import com.auth0.jwk.UrlJwkProvider;
import com.auth0.jwk.Jwk;
import io.jsonwebtoken.Claims;
import io.jsonwebtoken.JwsHeader;
import io.jsonwebtoken.SigningKeyResolverAdapter;
import java.security.Key;
import java.net.URI;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class JwkKeyResolver extends SigningKeyResolverAdapter {
    private JwkProvider keyStore;
    private final Logger LOGGER = LoggerFactory.getLogger(this.getClass());
    public JwkKeyResolver() throws java.net.URISyntaxException, java.net.MalformedURLException {
        this.keyStore = new UrlJwkProvider((new URI("https://login.microsoftonline.com/common/discovery/keys").toURL()));
    }
    @Override
    public Key resolveSigningKey(JwsHeader jwsHeader, Claims claims) {
        try {
            String keyId = jwsHeader.getKeyId();
            Jwk pub = keyStore.get(keyId);
            return pub.getPublicKey();
        } catch (Exception e) {
            LOGGER.error(e.getMessage());
            return null;
        }
    }
}
```

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="684cc-279">Расшифровка данных ресурсов из уведомлений об изменениях</span><span class="sxs-lookup"><span data-stu-id="684cc-279">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="684cc-280">Свойство **resourceData** уведомления об изменении содержит только основной идентификатор и сведения о типе экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="684cc-280">The **resourceData** property of a change notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="684cc-281">Свойство **encryptedData** содержит полные данные о ресурсе, зашифрованные Microsoft Graph с использованием открытого ключа, указанного в подписке.</span><span class="sxs-lookup"><span data-stu-id="684cc-281">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="684cc-282">Это свойство также содержит значения, необходимые для проверки и расшифровки.</span><span class="sxs-lookup"><span data-stu-id="684cc-282">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="684cc-283">Это выполняется для повышения безопасности пользовательских данных, к которым получен доступ с помощью уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-283">This is done to increase the security of customer data accessed via change notifications.</span></span> <span data-ttu-id="684cc-284">Вы отвечаете за защиту закрытого ключа, чтобы гарантировать невозможность расшифровки пользовательских данных посторонними, даже если они смогли перехватить исходные уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-284">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original change notifications.</span></span>

<span data-ttu-id="684cc-285">Содержание:</span><span class="sxs-lookup"><span data-stu-id="684cc-285">In this section:</span></span>

- [<span data-ttu-id="684cc-286">Управление ключами шифрования</span><span class="sxs-lookup"><span data-stu-id="684cc-286">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="684cc-287">Расшифровка данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="684cc-287">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="684cc-288">Пример: расшифровка уведомления с зашифрованными данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="684cc-288">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="684cc-289">Управление ключами шифрования</span><span class="sxs-lookup"><span data-stu-id="684cc-289">Managing encryption keys</span></span>

1. <span data-ttu-id="684cc-290">Получите сертификат с парой асимметричных ключей.</span><span class="sxs-lookup"><span data-stu-id="684cc-290">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="684cc-291">Вы можете самостоятельно подписать сертификат, так как Microsoft Graph не проверяет поставщика сертификата и использует открытый ключ только для шифрования.</span><span class="sxs-lookup"><span data-stu-id="684cc-291">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="684cc-292">В качестве решения для создания и ротации сертификатов, а также безопасного управления ими используйте [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis).</span><span class="sxs-lookup"><span data-stu-id="684cc-292">Use [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="684cc-293">Убедитесь, что ключи удовлетворяют следующим условиям:</span><span class="sxs-lookup"><span data-stu-id="684cc-293">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="684cc-294">Ключ должен быть типа `RSA`</span><span class="sxs-lookup"><span data-stu-id="684cc-294">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="684cc-295">Размер ключа должен находиться в диапазоне от 2048 до 4096 бит</span><span class="sxs-lookup"><span data-stu-id="684cc-295">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="684cc-296">Экспортируйте сертификат в формате X.509 с кодировкой base64 и **добавьте только открытый ключ**.</span><span class="sxs-lookup"><span data-stu-id="684cc-296">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="684cc-297">При создании подписки:</span><span class="sxs-lookup"><span data-stu-id="684cc-297">When creating a subscription:</span></span>

    - <span data-ttu-id="684cc-298">Укажите сертификат в свойстве **encryptionCertificate**, используя контент в кодировке base64, в которой сертификат был экспортирован.</span><span class="sxs-lookup"><span data-stu-id="684cc-298">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="684cc-299">Укажите ваш собственный идентификатор в свойстве **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="684cc-299">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="684cc-300">Этот идентификатор позволяет сопоставлять сертификаты с получаемыми уведомлениями об изменениях, а также получать сертификаты из хранилища сертификатов.</span><span class="sxs-lookup"><span data-stu-id="684cc-300">This identifier allows you to match your certificates to the change notifications you receive, and to retrieve certificates from your certificate store.</span></span> <span data-ttu-id="684cc-301">Длина идентификатора не должна превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="684cc-301">The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="684cc-302">Обеспечьте защиту закрытого ключа, чтобы ваш код обработки уведомлений об изменениях мог обращаться к закрытому ключу для расшифровки данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="684cc-302">Manage the private key securely, so that your change notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="684cc-303">Ротация ключей</span><span class="sxs-lookup"><span data-stu-id="684cc-303">Rotating keys</span></span>

<span data-ttu-id="684cc-304">Чтобы уменьшить риск компрометации закрытого ключа, периодически изменяйте ассиметричные ключи.</span><span class="sxs-lookup"><span data-stu-id="684cc-304">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="684cc-305">Чтобы добавить новую пару ключей, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="684cc-305">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="684cc-306">Получите новый сертификат с новой парой асимметричных ключей.</span><span class="sxs-lookup"><span data-stu-id="684cc-306">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="684cc-307">Используйте его для всех создаваемых подписок.</span><span class="sxs-lookup"><span data-stu-id="684cc-307">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="684cc-308">Обновите существующие подписки с использованием нового ключа сертификата.</span><span class="sxs-lookup"><span data-stu-id="684cc-308">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="684cc-309">Выполняйте это в рамках регулярного возобновления подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-309">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="684cc-310">Или перечислите все подписки и укажите ключ.</span><span class="sxs-lookup"><span data-stu-id="684cc-310">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="684cc-311">Используйте [операцию PATCH для подписки](/graph/api/subscription-update?view=graph-rest-1.0) и обновите свойства **encryptionCertificate** и **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="684cc-311">Use the [PATCH operation on the subscription](/graph/api/subscription-update?view=graph-rest-1.0) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="684cc-312">Учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="684cc-312">Keep in mind the following:</span></span>
    - <span data-ttu-id="684cc-313">В течение некоторого периода времени старый сертификат по-прежнему можно использовать для шифрования.</span><span class="sxs-lookup"><span data-stu-id="684cc-313">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="684cc-314">Чтобы расшифровать контент, у вашего приложения должен быть доступ как к старым, так и к новым сертификатам.</span><span class="sxs-lookup"><span data-stu-id="684cc-314">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="684cc-315">Используйте свойство **encryptionCertificateId** в каждом уведомлении об изменении, чтобы определить правильный ключ для использования.</span><span class="sxs-lookup"><span data-stu-id="684cc-315">Use the **encryptionCertificateId** property in each change notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="684cc-316">Удалите старый сертификат, только когда он перестает указываться в последних уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="684cc-316">Discard of the old certificate only when you have seen no recent change notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="684cc-317">Расшифровка данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="684cc-317">Decrypting resource data</span></span>

<span data-ttu-id="684cc-318">Microsoft Graph использует двухэтапный процесс шифрования с целью оптимизации работы:</span><span class="sxs-lookup"><span data-stu-id="684cc-318">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="684cc-319">Создается симметричный ключ однократного применения, который используется для шифрования данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="684cc-319">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="684cc-320">Используется открытый асимметричный ключ (указанный при подписке), чтобы зашифровать симметричный ключ и добавить его в каждое уведомление об изменении этой подписки.</span><span class="sxs-lookup"><span data-stu-id="684cc-320">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each change notification of that subscription.</span></span>

<span data-ttu-id="684cc-321">Всегда предполагайте, что для каждого элемента в уведомлении об изменении используется разный симметричный ключ.</span><span class="sxs-lookup"><span data-stu-id="684cc-321">Always assume that the symmetric key is different for each item in the change notification.</span></span>

<span data-ttu-id="684cc-322">Чтобы расшифровать данные ресурсов, приложение должно выполнить обратные действия, используя свойства в разделе **encryptedContent** в каждом уведомлении об изменении:</span><span class="sxs-lookup"><span data-stu-id="684cc-322">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each change notification:</span></span>

1. <span data-ttu-id="684cc-323">Используйте свойство **encryptionCertificateId**, чтобы определить сертификат для использования.</span><span class="sxs-lookup"><span data-stu-id="684cc-323">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="684cc-324">Инициализируйте криптографический компонент RSA (например, .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) с помощью закрытого ключа.</span><span class="sxs-lookup"><span data-stu-id="684cc-324">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="684cc-325">Расшифруйте симметричный ключ, указанный в свойстве **dataKey** каждого элемента в уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="684cc-325">Decrypt the symmetric key delivered in the **dataKey** property of each item in the change notification.</span></span>

    <span data-ttu-id="684cc-326">Используйте оптимальное асимметричное шифрование с дополнением (OAEP) в качестве алгоритма расшифровки.</span><span class="sxs-lookup"><span data-stu-id="684cc-326">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="684cc-327">Используйте симметричный ключ, чтобы вычислить подпись HMAC-SHA256 значения в объекте **data**.</span><span class="sxs-lookup"><span data-stu-id="684cc-327">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="684cc-328">Сравните его со значением в объекте **dataSignature**.</span><span class="sxs-lookup"><span data-stu-id="684cc-328">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="684cc-329">Если они не совпадают, считайте, что полезные данные были подменены, и не расшифровывайте их.</span><span class="sxs-lookup"><span data-stu-id="684cc-329">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="684cc-330">Используйте симметричный ключ с AES (например, .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) для расшифровки содержимого в объекте **data**.</span><span class="sxs-lookup"><span data-stu-id="684cc-330">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="684cc-331">Используйте следующие параметры расшифровки для алгоритма AES:</span><span class="sxs-lookup"><span data-stu-id="684cc-331">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="684cc-332">Дополнение: PKCS7</span><span class="sxs-lookup"><span data-stu-id="684cc-332">Padding: PKCS7</span></span>
        - <span data-ttu-id="684cc-333">Режим шифрования: CBC</span><span class="sxs-lookup"><span data-stu-id="684cc-333">Cipher mode: CBC</span></span>
    - <span data-ttu-id="684cc-334">Настройте "вектор инициализации", скопировав первые 16 байт симметричного ключа, использованного для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="684cc-334">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="684cc-335">Расшифрованное значение — это строка JSON, представляющая экземпляр ресурса в уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="684cc-335">The decrypted value is a JSON string that represents the resource instance in the change notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="684cc-336">Пример: расшифровка уведомления с зашифрованными данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="684cc-336">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="684cc-337">Ниже приведен пример уведомления об изменении, включающего зашифрованные значения свойств экземпляра **chatMessage** в сообщении канала.</span><span class="sxs-lookup"><span data-stu-id="684cc-337">The following is an example change notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="684cc-338">Экземпляр задается значением `@odata.id`.</span><span class="sxs-lookup"><span data-stu-id="684cc-338">The instance is specified by the `@odata.id` value.</span></span>

```json
{
    "value": [
        {
            "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
            "changeType": "created",
            // Other properties typical in a resource change notification
            "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
            "resourceData": {
                "id": "1565293727947",
                "@odata.type": "#Microsoft.Graph.ChatMessage",
                "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
            },
            "encryptedContent": {
                "data": "{encrypted data that produces a full resource}",
        "dataSignature": "<HMAC-SHA256 hash>",
                "dataKey": "{encrypted symmetric key from Microsoft Graph}",
                "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
                "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
            }
        }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
    ]
}
```

> <span data-ttu-id="684cc-339">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="684cc-339">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>


<span data-ttu-id="684cc-340">В этом разделе содержатся некоторые полезные фрагменты кода, использующие C# и .NET для каждого этапа расшифровки.</span><span class="sxs-lookup"><span data-stu-id="684cc-340">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="684cc-341">Расшифровка симметричного ключа</span><span class="sxs-lookup"><span data-stu-id="684cc-341">Decrypt the symmetric key</span></span>

```csharp
// Initialize with the private key that matches the encryptionCertificateId.
RSACryptoServiceProvider rsaProvider = ...;        
byte[] encryptedSymmetricKey = Convert.FromBase64String(<value from dataKey property>);

// Decrypt using OAEP padding.
byte[] decryptedSymmetricKey = rsaProvider.Decrypt(encryptedSymmetricKey, fOAEP: true);

// Can now use decryptedSymmetricKey with the AES algorithm.
```
```Java
String storename = ""; //name/path of the jks store
String storepass = ""; //password used to open the jks store
String alias = ""; //alias of the certificate when store in the jks store, should be passed as encryptionCertificateId when subscribing and retrieved from the notification
KeyStore ks = KeyStore.getInstance("JKS");
ks.load(new FileInputStream(storename), storepass.toCharArray());
Key asymmetricKey = ks.getKey(alias, storepass.toCharArray());
byte[] encryptedSymetricKey = Base64.decodeBase64("<value from dataKey property>");
Cipher cipher = Cipher.getInstance("RSA/ECB/OAEPWithSHA1AndMGF1Padding");
cipher.init(Cipher.DECRYPT_MODE, asymmetricKey);
byte[] decryptedSymmetricKey = cipher.doFinal(encryptedSymetricKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```
```JavaScript
const base64encodedKey = 'base 64 encoded dataKey value';
const asymetricPrivateKey = 'pem encoded private key';
const decodedKey = Buffer.from(base64encodedKey, 'base64');
const decryptedSymetricKey = crypto.privateDecrypt(asymetricPrivateKey, decodedKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="684cc-342">Сравнение подписи данных с помощью HMAC-SHA256</span><span class="sxs-lookup"><span data-stu-id="684cc-342">Compare data signature using HMAC-SHA256</span></span>

```csharp
byte[] decryptedSymmetricKey = <the aes key decrypted in the previous step>;
byte[] encryptedPayload = <the value from the data property, still encrypted>;
byte[] expectedSignature = <the value from the dataSignature property>;
byte[] actualSignature;

using (HMACSHA256 hmac = new HMACSHA256(decryptedSymmetricKey))
{
    actualSignature = hmac.ComputeHash(encryptedPayload);
}
if (actualSignature.SequenceEqual(expectedSignature))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```Java
byte[] decryptedSymmetricKey = "<the aes key decrypted in the previous step>";
byte[] decodedEncryptedData = Base64.decodeBase64("data property from encryptedContent object");
Mac mac = Mac.getInstance("HMACSHA256");
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "HMACSHA256");
mac.init(skey);
byte[] hashedData = mac.doFinal(decodedEncryptedData);
String encodedHashedData = new String(Base64.encodeBase64(hashedData));
if (comparisonSignature.equals(encodedHashedData))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```JavaScript
const decryptedSymetricKey = []; //Buffer provided by previous step
const base64encodedSignature = 'base64 encodded value from the dataSignature property';
const hmac = crypto.createHmac('sha256', decryptedSymetricKey);
hmac.write(base64encodedPayload, 'base64');
if(base64encodedSignature === hmac.digest('base64'))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="684cc-343">Расшифровка содержимого данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="684cc-343">Decrypt the resource data content</span></span>

```csharp
AesCryptoServiceProvider aesProvider = new AesCryptoServiceProvider();
aesProvider.Key = decryptedSymmetricKey;
aesProvider.Padding = PaddingMode.PKCS7;
aesProvider.Mode = CipherMode.CBC;

// Obtain the intialization vector from the symmetric key itself.
int vectorSize = 16;
byte[] iv = new byte[vectorSize];
Array.Copy(decryptedSymmetricKey, iv, vectorSize);
aesProvider.IV = iv;

byte[] encryptedPayload = Convert.FromBase64String(<value from dataKey property>);

string decryptedResourceData;
// Decrypt the resource data content.
using (var decryptor = aesProvider.CreateDecryptor())
{
  using (MemoryStream msDecrypt = new MemoryStream(encryptedPayload))
  {
      using (CryptoStream csDecrypt = new CryptoStream(msDecrypt, decryptor, CryptoStreamMode.Read))
      {
          using (StreamReader srDecrypt = new StreamReader(csDecrypt))
          {
              decryptedResourceData = srDecrypt.ReadToEnd();
          }
      }
  }
}

// decryptedResourceData now contains a JSON string that represents the resource.
```
```Java
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "AES");
IvParameterSpec ivspec = new IvParameterSpec(Arrays.copyOf(decryptedSymmetricKey, 16));
Cipher cipher = Cipher.getInstance("AES/CBC/PKCS5PADDING");
cipher.init(Cipher.DECRYPT_MODE, skey, ivspec);
String decryptedResourceData = new String(cipher.doFinal(Base64.decodeBase64(encryptedData)));
```
```JavaScript
const base64encodedPayload = 'base64 encoded value from data property';
const decryptedSymetricKey = []; //Buffer provided by previous step
const iv = Buffer.alloc(16, 0);
decryptedSymetricKey.copy(iv, 0, 0, 16);
const decipher = crypto.createDecipheriv('aes-256-cbc', decryptedSymetricKey, iv);
let decryptedPayload = decipher.update(base64encodedPayload, 'base64', 'utf8');
decryptedPayload += decipher.final('utf8');
```

## <a name="see-also"></a><span data-ttu-id="684cc-344">См. также</span><span class="sxs-lookup"><span data-stu-id="684cc-344">See also</span></span>

- [<span data-ttu-id="684cc-345">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="684cc-345">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="684cc-346">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="684cc-346">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-beta)
- [<span data-ttu-id="684cc-347">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-347">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="684cc-348">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-348">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="684cc-349">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="684cc-349">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
