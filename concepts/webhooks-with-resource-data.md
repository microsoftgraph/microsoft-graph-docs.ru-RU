---
title: Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)
description: Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Уведомления могут включать свойства ресурсов.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: a0db70d65b919033f6c371b8bf704ed7e2c77b5b
ms.sourcegitcommit: 8a84ee922acd2946a3ffae9f8f7f7b485567bc05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2020
ms.locfileid: "42618653"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a><span data-ttu-id="7cb4f-104">Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7cb4f-104">Set up change notifications that include resource data (preview)</span></span>

<span data-ttu-id="7cb4f-105">Microsoft Graph позволяет приложениям подписываться на уведомления об изменениях ресурсов с использованием [веб-перехватчиков](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="7cb4f-106">Теперь можно настроить подписки таким образом, чтобы в уведомления включались данные измененных ресурсов (например, содержимое сообщения чата из Microsoft Teams).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-106">You can now set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message) in notifications.</span></span> <span data-ttu-id="7cb4f-107">Затем приложение сможет запустить свою бизнес-логику без отдельного вызова API для получения измененного ресурса.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="7cb4f-108">В результате приложение работает эффективнее, выполняя меньше вызовов API, что полезно в крупномасштабных сценариях.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="7cb4f-109">Добавление данных ресурса в уведомления требует реализации следующей дополнительной логики, чтобы выполнить требования по доступу к данным и их безопасности.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-109">Including resource data as part of notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="7cb4f-110">[Применяйте](#subscription-life-cycle-notifications) специальные уведомления _жизненного цикла_ подписки, чтобы обеспечить непрерывный поток данных.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-110">[Handle](#subscription-life-cycle-notifications) special subscription _life cycle_ notifications to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="7cb4f-111">Microsoft Graph периодически отправляет уведомления жизненного цикла, требуя от приложения повторной авторизации, чтобы обеспечить отсутствие неожиданных проблем с доступом при включении данных ресурсов в уведомления.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-111">Microsoft Graph sends life cycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in notifications.</span></span>
- <span data-ttu-id="7cb4f-112">[Проверяйте](#validating-the-authenticity-of-notifications) подлинность уведомлений, подтверждая что их источником является Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="7cb4f-113">[Предоставьте](#decrypting-resource-data-from-change-notifications) открытый ключ шифрования и используйте закрытый ключ для расшифровки данных ресурсов, полученных в уведомлениях.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="7cb4f-114">Сведения ресурсов в полезных данных уведомлений</span><span class="sxs-lookup"><span data-stu-id="7cb4f-114">Resource data in notification payload</span></span>

<span data-ttu-id="7cb4f-115">Обычно этот тип уведомлений об изменениях содержит следующие сведения ресурсов в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="7cb4f-116">Идентификатор и тип измененного экземпляра ресурса, возвращаемые в свойстве **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="7cb4f-117">Все значения свойств экземпляра ресурса, зашифрованные в соответствии с подпиской и возвращаемые в свойстве **encryptedContent**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="7cb4f-118">Или зависимые от ресурса определенные свойства, возвращаемые в свойстве **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="7cb4f-119">Чтобы получить только определенные свойства, их нужно указать в URL-адресе объекта **resource** в подписке, используя параметр `$select`.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="7cb4f-120">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="7cb4f-120">Supported resources</span></span>

<span data-ttu-id="7cb4f-121">В настоящее время ресурс [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (предварительная версия) в Microsoft Teams поддерживает уведомления об изменениях, включающие данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (preview) resource supports change notifications that include resource data.</span></span> <span data-ttu-id="7cb4f-122">В частности, вы можете настроить подписку, относящуюся к одному из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="7cb4f-123">Новые или измененные сообщения в определенном канале Teams: `/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="7cb4f-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="7cb4f-124">Новые или измененные сообщения в определенном чате Teams: `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="7cb4f-124">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>

<span data-ttu-id="7cb4f-125">Ресурс **chatMessage** поддерживает включение в уведомление всех свойств измененного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-125">The **chatMessage** resource supports including all the properties of a changed instance in a notification.</span></span> <span data-ttu-id="7cb4f-126">Он не поддерживает возвращение только выбранных свойств экземпляра.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-126">It does not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="7cb4f-127">В этой статье рассматривается пример подписки на уведомления об изменениях в канале Teams. При этом каждое уведомление содержит все данные ресурсов измененного экземпляра **chatMessage**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-127">This article walks through an example of subscribing to change notifications of messages in a Teams channel, with each notification including the full resource data of the changed **chatMessage** instance.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="7cb4f-128">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-128">Creating a subscription</span></span>

<span data-ttu-id="7cb4f-129">Чтобы включить данные ресурсов в уведомления об изменениях, **требуется** указать следующие свойства в дополнение к обычно указываемым при [создании подписки](webhooks.md#creating-a-subscription):</span><span class="sxs-lookup"><span data-stu-id="7cb4f-129">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="7cb4f-130">**includeResourceData**, которому следует присвоить значение `true`, чтобы явно запросить данные ресурса.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-130">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="7cb4f-131">**lifecycleNotificationUrl**, являющееся конечной точкой, в которую доставляются [уведомления жизненного цикла](#subscription-life-cycle-notifications).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-131">**lifecycleNotificationUrl** which is an endpoint where [life cycle notifications](#subscription-life-cycle-notifications) are delivered.</span></span> <span data-ttu-id="7cb4f-132">Оно может совпадать с **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-132">This can be the same or different as **notificationUrl**.</span></span>
- <span data-ttu-id="7cb4f-133">**encryptionCertificate**, содержащее только открытый ключ, используемый Microsoft Graph для шифрования данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-133">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="7cb4f-134">Сохраняйте соответствующий закрытый ключ для [расшифровки контента](#decrypting-resource-data-from-change-notifications).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-134">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="7cb4f-135">**encryptionCertificateId**, являющееся вашим собственным идентификатором для сертификата.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-135">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="7cb4f-136">Используйте этот идентификатор для определения в каждом уведомлении сертификата, используемого для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-136">Use this ID to match in each notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="7cb4f-137">Учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-137">Keep the following in mind:</span></span>

- <span data-ttu-id="7cb4f-138">Используйте одинаковое имя узла для обеих конечных точек уведомлений (**notificationUrl** и **lifecycleNotificationUrl**).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-138">Use the same host name for both notification endpoints (**notificationUrl** and **lifecycleNotificationUrl**).</span></span>
- <span data-ttu-id="7cb4f-139">Проверьте обе конечные точки уведомлений, как описано [здесь](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-139">Validate both notification endpoints as described [here](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="7cb4f-140">Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-140">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>
- <span data-ttu-id="7cb4f-141">Вы не сможете обновить (`PATCH`) существующую подписку, чтобы добавить свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-141">You cannot update (`PATCH`) an existing subscription to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="7cb4f-142">Следует удалить существующую подписку и создать новую, чтобы указать свойство **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-142">You should remove the existing subscription, and create a new subscription to include the **lifecycleNotificationUrl** property.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="7cb4f-143">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="7cb4f-143">Subscription request example</span></span>

<span data-ttu-id="7cb4f-144">В примере ниже выполняется подписка на два типа уведомлений:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-144">The following example subscribes to two types of notifications:</span></span> 

- <span data-ttu-id="7cb4f-145">Изменения ресурсов — создание или обновление сообщений каналов в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7cb4f-145">Resource changes - channel messages being created or updated in Microsoft Teams</span></span>
- <span data-ttu-id="7cb4f-146">События жизненного цикла подписки, которые могут влиять на поток уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-146">Subscription life cycle events which can affect the flow of change notifications.</span></span> <span data-ttu-id="7cb4f-147">Дополнительные сведения об уведомлениях жизненного цикла см. в [следующем разделе](#subscription-life-cycle-notifications).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-147">See more details about life cycle notifications in the [next section](#subscription-life-cycle-notifications).</span></span>

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

### <a name="subscription-response"></a><span data-ttu-id="7cb4f-148">Отклик подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-148">Subscription response</span></span>
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
  "encryptionCertificateThumbprint": "{thumbprint from the certificate}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-life-cycle-notifications"></a><span data-ttu-id="7cb4f-149">Уведомления жизненного цикла подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-149">Subscription life cycle notifications</span></span>

<span data-ttu-id="7cb4f-150">Некоторые события могут воздействовать на стандартный потоку уведомлений в существующей подписке.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-150">Certain events can interfere with normal notification flow in an existing subscription.</span></span> <span data-ttu-id="7cb4f-151">_Уведомления жизненного цикла_ подписки указывают необходимые действия для обеспечения непрерывного потока.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-151">Subscription _life cycle notifications_ inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="7cb4f-152">В отличие от уведомления об изменении ресурса, информирующем об изменении экземпляра ресурса, уведомление жизненного цикла относится к самой подписке и ее текущему состоянию в жизненном цикле.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-152">Unlike a resource change notification which informs a change to a resource instance, a life cycle notification is about the subscription itself, and its current state in the life cycle.</span></span> 

<span data-ttu-id="7cb4f-153">Уведомления жизненного цикла доставляются в объект **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-153">Life cycle notifications are delivered to the **lifecycleNotificationUrl**.</span></span> 

<span data-ttu-id="7cb4f-154">Содержание</span><span class="sxs-lookup"><span data-stu-id="7cb4f-154">In this section:</span></span>

- [<span data-ttu-id="7cb4f-155">Уведомление жизненного цикла, запрашивающее авторизацию подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-155">Life cycle notification that challenges subscription authorization</span></span>](#life-cycle-notification-that-challenges-subscription-authorization)
- [<span data-ttu-id="7cb4f-156">Поток запроса авторизации</span><span class="sxs-lookup"><span data-stu-id="7cb4f-156">Authorization challenge flow</span></span>](#authorization-challenge-flow)
- [<span data-ttu-id="7cb4f-157">Пример запроса авторизации</span><span class="sxs-lookup"><span data-stu-id="7cb4f-157">Example authorization challenge</span></span>](#example-authorization-challenge)
- [<span data-ttu-id="7cb4f-158">Ответ на запрос авторизации</span><span class="sxs-lookup"><span data-stu-id="7cb4f-158">Responding to an authorization challenge</span></span>](#responding-to-an-authorization-challenge)
- [<span data-ttu-id="7cb4f-159">Советы</span><span class="sxs-lookup"><span data-stu-id="7cb4f-159">Tips</span></span>](#tips)
- [<span data-ttu-id="7cb4f-160">Подготовка к изменениям кода для обработки других типов уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="7cb4f-160">Future-proof your code to handle other types of life cycle notifications</span></span>](#future-proof-your-code-to-handle-other-types-of-life-cycle-notifications)

### <a name="life-cycle-notification-that-challenges-subscription-authorization"></a><span data-ttu-id="7cb4f-161">Уведомление жизненного цикла, запрашивающее авторизацию подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-161">Life cycle notification that challenges subscription authorization</span></span>

<span data-ttu-id="7cb4f-162">Один из типов уведомлений жизненного цикла запрашивает авторизованное состояние активной подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-162">One type of life cycle notifications challenges the authorized state of an active subscription.</span></span> <span data-ttu-id="7cb4f-163">Если в свойстве **lifecycleEvent** уведомления указано значение `reauthorizationRequired`, требуется повторно авторизовать подписку, чтобы поток данных не прерывался.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-163">When the **lifecycleEvent** property in a notification indicates `reauthorizationRequired`, you must re-authorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="7cb4f-164">При создании долгосрочной подписки (например, длительностью 3 дня) уведомления о данных ресурсов направляются в расположение, указанное в свойстве **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-164">When you create a long-lived subscription (for example, one that lasts for 3 days), resource data notifications flows to the location indicated in **notificationUrl**.</span></span> <span data-ttu-id="7cb4f-165">Однако в любой момент Microsoft Graph может потребовать повторную авторизацию подписки, чтобы подтвердить наличие у вас доступа к данным ресурсов в случае изменения условий доступа с момента создания подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-165">However, at any point in time, Microsoft Graph may require that you re-authorize the subscription to prove that you still have access to resource data, in case the conditions of access have changed since the subscription was created.</span></span> <span data-ttu-id="7cb4f-166">Ниже приведены примеры изменений, влияющих на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-166">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="7cb4f-167">Администратор клиента может отозвать разрешения приложения на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-167">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="7cb4f-168">В интерактивном сценарии к пользователю, предоставляющему маркер проверки подлинности для вашего приложения, могут применяться динамические политики на основе различных факторов, например их расположения, состояния устройства или оценки риска.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-168">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="7cb4f-169">Например, если пользователь изменяет свое физическое расположение, ему может быть запрещен доступ к данным, и ваше приложение не сможет повторно авторизовать подписку.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-169">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to re-authorize the subscription.</span></span> <span data-ttu-id="7cb4f-170">Дополнительные сведения о динамических политиках, управляющих доступом, см. в статье [Политики условного доступа Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-170">For more information on dynamic policies that control access, see [Azure AD conditional access policies](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span></span> 

### <a name="authorization-challenge-flow"></a><span data-ttu-id="7cb4f-171">Поток запроса авторизации</span><span class="sxs-lookup"><span data-stu-id="7cb4f-171">Authorization challenge flow</span></span>

<span data-ttu-id="7cb4f-172">Поток запроса авторизации для активной подписки с неистекшим сроком действия выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-172">The flow of an authorization challenge for an active, non-expired subscription looks as follows:</span></span>

1. <span data-ttu-id="7cb4f-173">Microsoft Graph требует повторной авторизации подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-173">Microsoft Graph requires a subscription to be re-authorized</span></span>
    
    <span data-ttu-id="7cb4f-174">Причины этого могут отличаться для разных ресурсов и меняться со временем.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-174">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="7cb4f-175">Независимо от причины события повторной авторизации вам потребуется отреагировать на него.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-175">Regardless of the cause of the re-authorization event, you will need to respond to it.</span></span>

2. <span data-ttu-id="7cb4f-176">Microsoft Graph отправляет уведомление о запросе авторизации в **lifecycleNotificationUrl**</span><span class="sxs-lookup"><span data-stu-id="7cb4f-176">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**</span></span>

    <span data-ttu-id="7cb4f-177">Обратите внимание, что поток уведомлений о ресурсе может некоторое время продолжаться, предоставляя вам дополнительное время для ответа.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-177">Note that the flow of resource notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="7cb4f-178">Однако в конечном итоге доставка уведомлений о ресурсе будет приостановлена, пока вы не выполните требуемое действие.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-178">However, eventually resource notification delivery will pause, until you take the required action.</span></span>

3. <span data-ttu-id="7cb4f-179">Ответьте на это уведомление одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-179">Respond to this notification in one of two ways:</span></span>
    1. <span data-ttu-id="7cb4f-180">Повторная авторизация подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-180">Re-authorize the subscription.</span></span> <span data-ttu-id="7cb4f-181">Это не продлевает срок действия подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-181">This does not extend the expiry date of the subscription.</span></span>
    2. <span data-ttu-id="7cb4f-182">Возобновление подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-182">Renew the subscription.</span></span> <span data-ttu-id="7cb4f-183">Это повторно авторизует подписку и продлевает срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-183">This both re-authorizes and extends the expiry date.</span></span>

    <span data-ttu-id="7cb4f-184">Примечание. Оба действия требуют предоставление действительного маркера проверки подлинности по аналогии с [созданием новой подписки](webhooks.md#creating-a-subscription) или [продлением подписки до истечения срока ее действия](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-184">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="7cb4f-185">Если вы успешно выполнили повторную авторизацию или возобновление подписки, уведомления о ресурсах продолжать поступать.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-185">If you successfully re-authorize or renew the subscription, resource notifications continue.</span></span> <span data-ttu-id="7cb4f-186">В противном случае уведомления о ресурсах не будут возобновлены.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-186">Otherwise, resource notifications remain paused.</span></span>
    
### <a name="example-authorization-challenge"></a><span data-ttu-id="7cb4f-187">Пример запроса авторизации</span><span class="sxs-lookup"><span data-stu-id="7cb4f-187">Example authorization challenge</span></span>

<span data-ttu-id="7cb4f-188">Ниже представлен пример уведомления жизненного цикла, запрашивающего повторную авторизацию подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-188">Below is an example life cycle notification that requests re-authorizing a subscription.</span></span> 

<span data-ttu-id="7cb4f-189">Обратите внимание на следующее:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-189">Note the following:</span></span>

- <span data-ttu-id="7cb4f-190">Поле `"lifecycleEvent": "reauthorizationRequired"` определяет это уведомление как запрос авторизации.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-190">The `"lifecycleEvent": "reauthorizationRequired"` field identifies this notification as an authorization challenge.</span></span>
- <span data-ttu-id="7cb4f-191">Это уведомление не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-191">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="7cb4f-192">Как и уведомления о ресурсах, уведомления жизненного цикла можно объединять (в коллекции **value**), каждое с возможно разными значениями **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-192">Similar to resource notifications, you can batch life cycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="7cb4f-193">Обрабатывайте каждое уведомление в пакете соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-193">Process each notification in the batch accordingly.</span></span>

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

### <a name="responding-to-an-authorization-challenge"></a><span data-ttu-id="7cb4f-194">Ответ на запрос авторизации</span><span class="sxs-lookup"><span data-stu-id="7cb4f-194">Responding to an authorization challenge</span></span>

<span data-ttu-id="7cb4f-195">Чтобы обработать уведомление жизненного цикла с запросом авторизации, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-195">Take the following steps to process an authorization challenge life cycle notification.</span></span> <span data-ttu-id="7cb4f-196">Первые два действия по подтверждению и проверке уведомления жизненного цикла аналогичны [ответу на уведомление об изменении ресурса](webhooks.md#processing-the-notification).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-196">The first two steps of acknowledging and validating the life cycle notification is similar to [responding to a resource change notification](webhooks.md#processing-the-notification).</span></span>

1. <span data-ttu-id="7cb4f-197">Подтвердите получение уведомления, ответив на вызов POST с помощью `HTTP 202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-197">Acknowledge the receipt of the notification, by responding to the POST call with `HTTP 202 Accepted`.</span></span>
2. <span data-ttu-id="7cb4f-198">Проверьте подлинность уведомления.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-198">Validate the authenticity of the notification.</span></span> <span data-ttu-id="7cb4f-199">Дополнительные сведения см. [ниже](#validating-the-authenticity-of-notifications).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-199">Further details [below](#validating-the-authenticity-of-notifications).</span></span>
3. <span data-ttu-id="7cb4f-200">Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-200">Ensure the app has a valid access token to take the next step.</span></span> 

    <span data-ttu-id="7cb4f-201">Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), библиотека сделает это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, попросив пользователя повторно войти с помощью нового пароля.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-201">If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), the library handles this for you by either reusing a valid cached token, or obtaining a new token from prompting the user to log in again with a new password.</span></span> <span data-ttu-id="7cb4f-202">Однако получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и пользователю больше недоступны данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-202">However, obtaining a new token may fail, since the conditions of access may have changed, and the user may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="7cb4f-203">Вызовите один из двух следующих API.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-203">Call either of the following two APIs.</span></span> <span data-ttu-id="7cb4f-204">Если вызов API выполняется успешно, поток уведомлений о ресурсе возобновляется.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-204">If the API call succeeds, the resource notification flow resumes.</span></span>

    - <span data-ttu-id="7cb4f-205">Чтобы повторно авторизовать подписку без продления ее срока, вызовите действие `/reauthorize`:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-205">Call the `/reauthorize` action to re-authorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="7cb4f-206">Чтобы одновременно возобновить и повторно авторизовать подписку, выполните обычное действие возобновления:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-206">Perform a regular renew action to re-authorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="7cb4f-207">Возобновление может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-207">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="7cb4f-208">Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-208">It may be necessary for the app to obtain a new access token from the user to successfully re-authorize a subscription.</span></span> 
      
      <span data-ttu-id="7cb4f-209">Вы может повторить эти действия позднее в любое время и успешно выполнить их, если изменяются условия доступа.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-209">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="7cb4f-210">Все уведомления об изменении ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-210">Any notifications about resource changes that happen between the time the life cycle notification was sent, and the time when the app eventually re-creates the subscription successfully, would be lost.</span></span> <span data-ttu-id="7cb4f-211">В таких случаях приложению нужно отдельно получить эти изменения.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-211">In such cases, the app should separately fetch those changes.</span></span>

### <a name="tips"></a><span data-ttu-id="7cb4f-212">Советы </span><span class="sxs-lookup"><span data-stu-id="7cb4f-212">Tips</span></span>

<span data-ttu-id="7cb4f-213">Учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-213">Keep the following in mind:</span></span>

1. <span data-ttu-id="7cb4f-214">Запросы авторизации не отменяют необходимость возобновления подписки на изменения ресурса до истечения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-214">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="7cb4f-215">Хотя вы можете возобновить подписку при получении запроса авторизации, Microsoft Graph может не выполнять запрос для всех ваших подписок.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-215">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="7cb4f-216">Например, подписка без действий и уведомлений о ресурсах, ожидающих доставки, может не создавать для приложения запросы на повторную авторизацию.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-216">For example, a subscription that does not have any activity and has no resource notifications pending delivery may not signal any re-authorization challenges to your app.</span></span> <span data-ttu-id="7cb4f-217">Обязательно [возобновите подписки](webhooks.md#renewing-a-subscription) до истечения их сроков действия.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-217">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

2. <span data-ttu-id="7cb4f-218">Частота запросов авторизации может изменяться.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-218">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="7cb4f-219">Не делайте предположений о частоте запросов авторизации.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-219">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="7cb4f-220">Эти уведомления сообщают, когда нужно принимать действия, избавляя от отслеживания подписок, которым требуется повторная авторизация.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-220">These notifications tell you when to take actions, saving you from having to track which subscriptions require re-authorization.</span></span> <span data-ttu-id="7cb4f-221">Будьте готовы обрабатывать запросы авторизации каждые несколько минут для всех подписок или в редких случаях лишь для некоторых подписок.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-221">Be ready to handle authorization challenges anywhere from once a few minutes for every subscription, to rarely for only some of your subscriptions.</span></span>

### <a name="future-proof-your-code-to-handle-other-types-of-life-cycle-notifications"></a><span data-ttu-id="7cb4f-222">Подготовка к изменениям кода для обработки других типов уведомлений жизненного цикла</span><span class="sxs-lookup"><span data-stu-id="7cb4f-222">Future-proof your code to handle other types of life cycle notifications</span></span>

<span data-ttu-id="7cb4f-223">Ожидайте публикацию уведомлений жизненного цикла подписки в конечной точке, указанной в **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-223">Expect subscription life cycle notifications to be posted to the same endpoint specified by **lifecycleNotificationUrl**.</span></span> <span data-ttu-id="7cb4f-224">Они отличаются свойством **lifecycleEvent** и могут содержать немного другую схему и свойства для обслуживания своих сценариев.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-224">They differentiate by the **lifecycleEvent** property and may contain slightly different schema and properties to serve the scenarios they address.</span></span>

<span data-ttu-id="7cb4f-225">Применяйте свой код, предполагая новые типы уведомлений жизненного цикла:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-225">Implement your code in anticipation of new types of life cycle notifications:</span></span>

1. <span data-ttu-id="7cb4f-226">Используйте свойство **lifecycleEvent**, чтобы указать тип уведомления для определения соответствующего ответа.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-226">Use the **lifecycleEvent** property to identify the type of notification so to determine the appropriate response.</span></span> <span data-ttu-id="7cb4f-227">Например, найдите свойство `"lifecycleEvent": "reauthorizationRequired"` для определения конкретного события и обработайте его.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-227">For example, look for the `"lifecycleEvent": "reauthorizationRequired"` property to identify a specific event, and handle it.</span></span>

1. <span data-ttu-id="7cb4f-228">Регистрируйте все события жизненного цикла, не распознанные вашим приложением, чтобы получить сведения о них.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-228">Log any life cycle events that your app does not recognize to gain awareness.</span></span>

1. <span data-ttu-id="7cb4f-229">Подпишитесь на [блог разработчика Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы следить за объявлениями об уведомлениях жизненного цикла для новых сценариев.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-229">Subscribe to the [Microsoft Graph Developer Blog](https://developer.microsoft.com/graph/blogs/) to watch for announcements of life cycle notifications for new scenarios.</span></span>

1. <span data-ttu-id="7cb4f-230">Просматривайте соответствующую документацию о новых уведомлениях жизненного цикла и реализуйте для них нужную поддержку.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-230">Look up related documentation for new life cycle notifications and implement support for them as appropriate.</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="7cb4f-231">Проверка подлинности уведомлений</span><span class="sxs-lookup"><span data-stu-id="7cb4f-231">Validating the authenticity of notifications</span></span>

<span data-ttu-id="7cb4f-232">Приложения часто выполняют бизнес-логику на основе данных ресурсов, включенных в уведомления.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-232">Apps often execute business logic based on resource data included in notifications.</span></span> <span data-ttu-id="7cb4f-233">Важно сначала проверить подлинность каждого уведомления.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-233">Having first verified the authenticity of each notification is important.</span></span> <span data-ttu-id="7cb4f-234">В противном случае посторонние смогут обмануть ваше приложение с помощью ложных уведомлений, заставить его неправильно выполнять бизнес-логику и привести к нарушению безопасности.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-234">Otherwise, a third party could spoof your app with false notifications, make it execute its business logic incorrectly, and lead to a security incident.</span></span>

<span data-ttu-id="7cb4f-235">Для основных уведомлений, не содержащих данные ресурсов, просто проверьте их на основе значения **clientState**, как описано [здесь](webhooks.md#processing-the-notification).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-235">For basic notifications which do not contain resource data, simply validate them based on the **clientState** value as described [here](webhooks.md#processing-the-notification).</span></span> <span data-ttu-id="7cb4f-236">Это приемлемо, так как вы можете выполнять последующие надежные вызовы Microsoft Graph, чтобы получить доступ к данным ресурсов и, следовательно, влияние любых попыток подмены ограничено.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-236">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="7cb4f-237">Для уведомлений, доставляющих данные ресурсов, проведите более тщательную проверку перед обработкой данных.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-237">For notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="7cb4f-238">Содержание</span><span class="sxs-lookup"><span data-stu-id="7cb4f-238">In this section:</span></span>

- [<span data-ttu-id="7cb4f-239">Маркеры проверки в уведомлении</span><span class="sxs-lookup"><span data-stu-id="7cb4f-239">Validation tokens in the notification</span></span>](#validation-tokens-in-the-notification)
- [<span data-ttu-id="7cb4f-240">Способ проверки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-240">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="7cb4f-241">Пример маркера JWT</span><span class="sxs-lookup"><span data-stu-id="7cb4f-241">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-notification"></a><span data-ttu-id="7cb4f-242">Маркеры проверки в уведомлении</span><span class="sxs-lookup"><span data-stu-id="7cb4f-242">Validation tokens in the notification</span></span>

<span data-ttu-id="7cb4f-243">Уведомление с данными ресурсов содержит дополнительное свойство **validationTokens**, содержащее массив маркеров JWT, созданных Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-243">A notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="7cb4f-244">Microsoft Graph создает один маркер для каждой отдельной пары приложения и клиента, для которой существует элемент в массиве **value**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-244">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="7cb4f-245">Учитывайте, что уведомления могут содержать разные элементы для различных приложений и клиентов, подписанных с помощью одинакового значения **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-245">Keep in mind that notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="7cb4f-246">В следующем примере уведомление содержит два элемента для одного приложения и двух разных клиентов, поэтому массив **validationTokens** содержит два маркера, требующие проверки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-246">In the following example, the notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

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
### <a name="how-to-validate"></a><span data-ttu-id="7cb4f-247">Способ проверки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-247">How to validate</span></span>

<span data-ttu-id="7cb4f-248">Если вы незнакомы с проверкой маркеров, см. [статью в блоге](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) с полезным обзором.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-248">If you are new to token validation, refer to this [blog article](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for a useful overview.</span></span> <span data-ttu-id="7cb4f-249">Используйте пакет SDK, например библиотеку [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) Майкрософт для .NET или стороннюю библиотеку для другой платформы.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-249">Use an SDK, such as Microsoft's [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third party library for a different platform.</span></span>

<span data-ttu-id="7cb4f-250">Следует учитывать следующее:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-250">Be mindful of the following:</span></span> 

- <span data-ttu-id="7cb4f-251">Всегда отправляйте код состояния `HTTP 202 Accepted` в ответе на уведомление.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-251">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the notification.</span></span> 
- <span data-ttu-id="7cb4f-252">Делайте это перед проверкой уведомления (например, если вы храните уведомления в очередях для последующей обработки) или после нее (если они обрабатываются на ходу), даже если проверка завершилась сбоем.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-252">Do that before validating the notification (for example, if you store notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="7cb4f-253">Принятие уведомления позволяет избежать ненужных повторений доставки, а также мешает любым возможным злоумышленникам выяснить, прошли ли они проверку.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-253">Accepting a notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="7cb4f-254">Вы всегда можете игнорировать неверное уведомление после его принятия.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-254">You can always choose to ignore an invalid notification after you have accepted it.</span></span>

<span data-ttu-id="7cb4f-255">В частности, выполняйте проверку каждого маркера JWT в коллекции **validationTokens**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-255">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="7cb4f-256">Если любой из маркеров не прошел проверку, считайте уведомление подозрительным и выполните дальнейшее исследование.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-256">If any tokens fail, consider the notification suspicious and investigate further.</span></span> 

<span data-ttu-id="7cb4f-257">Для проверки маркеров и приложений, создающих маркеры, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-257">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="7cb4f-258">Убедитесь, что срок действия маркера не истек.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-258">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="7cb4f-259">Проверьте, что маркер не был подделан и был выдан ожидаемым центром авторизации (Microsoft Azure Active Directory):</span><span class="sxs-lookup"><span data-stu-id="7cb4f-259">Validate the token has not been tampered with and was issued by the expected authority, Microsoft Azure Active Directory:</span></span>

    - <span data-ttu-id="7cb4f-260">Получите ключи подписи от общей конечной точки конфигурации: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-260">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="7cb4f-261">Эта конфигурация кэшируется приложением на определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-261">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="7cb4f-262">Имейте в виду, что конфигурация часто обновляется, так как ключи входа ежедневно меняются.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-262">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="7cb4f-263">Проверьте подпись маркера JWT, использующего эти ключи.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-263">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="7cb4f-264">Не принимайте маркеры, выпущенные любыми другими центрами.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-264">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="7cb4f-265">Проверьте, что маркер выпущен для вашего приложения, подписавшегося на уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-265">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="7cb4f-266">Следующие действия являются частью стандартной логики проверки в библиотеках маркеров JWT, и обычно их можно выполнять в виде вызова одной функции.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-266">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="7cb4f-267">Убедитесь, что "аудитория" в маркере совпадает с идентификатором вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-267">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="7cb4f-268">Если уведомления получают несколько приложений, выполните проверку по нескольким идентификаторам.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-268">If you have more than one app receiving notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="7cb4f-269">**Важно**. Убедитесь, что приложение, создавшее маркер, представляет издателя уведомления об изменениях Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-269">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="7cb4f-270">Проверьте, что свойство **appid** в маркере соответствует ожидаемому значению `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-270">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="7cb4f-271">Это гарантирует, что уведомления не отправляются другим приложением, отличным от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-271">This ensures that notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="7cb4f-272">Пример маркера JWT</span><span class="sxs-lookup"><span data-stu-id="7cb4f-272">Example JWT token</span></span>

<span data-ttu-id="7cb4f-273">Ниже приведен пример свойств, входящих в маркер JWT, которые требуется проверить:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-273">Here is an example of the properties included in the JWT token that are needed for validation:</span></span>

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

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="7cb4f-274">Пример: подтверждение маркеров проверки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-274">Example: Verifying validation tokens</span></span>

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
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

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="7cb4f-275">Расшифровка данных ресурсов из уведомлений об изменениях</span><span class="sxs-lookup"><span data-stu-id="7cb4f-275">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="7cb4f-276">Свойство **resourceData** уведомления содержит только основной идентификатор и сведения о типе экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-276">The **resourceData** property of a notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="7cb4f-277">Свойство **encryptedData** содержит полные данные о ресурсе, зашифрованные Microsoft Graph с использованием открытого ключа, указанного в подписке.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-277">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="7cb4f-278">Это свойство также содержит значения, необходимые для проверки и расшифровки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-278">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="7cb4f-279">Это выполняется для повышения безопасности пользовательских данных, к которым получен доступ с помощью уведомлений.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-279">This is done to increase the security of customer data accessed via notifications.</span></span> <span data-ttu-id="7cb4f-280">Вы отвечаете за защиту закрытого ключа, чтобы гарантировать невозможность расшифровки пользовательских данных посторонними, даже если они смогли перехватить исходные уведомления.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-280">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original notifications.</span></span>

<span data-ttu-id="7cb4f-281">Содержание</span><span class="sxs-lookup"><span data-stu-id="7cb4f-281">In this section:</span></span>

- [<span data-ttu-id="7cb4f-282">Управление ключами шифрования</span><span class="sxs-lookup"><span data-stu-id="7cb4f-282">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="7cb4f-283">Расшифровка данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="7cb4f-283">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="7cb4f-284">Пример: расшифровка уведомления с зашифрованными данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="7cb4f-284">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="7cb4f-285">Управление ключами шифрования</span><span class="sxs-lookup"><span data-stu-id="7cb4f-285">Managing encryption keys</span></span>

1. <span data-ttu-id="7cb4f-286">Получите сертификат с парой асимметричных ключей.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-286">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="7cb4f-287">Вы можете самостоятельно подписать сертификат, так как Microsoft Graph не проверяет поставщика сертификата и использует открытый ключ только для шифрования.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-287">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="7cb4f-288">В качестве решения для создания и ротации сертификатов, а также безопасного управления ими используйте [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis).</span><span class="sxs-lookup"><span data-stu-id="7cb4f-288">Use [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="7cb4f-289">Убедитесь, что ключи удовлетворяют следующим условиям:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-289">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="7cb4f-290">Ключ должен быть типа `RSA`</span><span class="sxs-lookup"><span data-stu-id="7cb4f-290">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="7cb4f-291">Размер ключа должен находиться в диапазоне от 2048 до 4096 бит</span><span class="sxs-lookup"><span data-stu-id="7cb4f-291">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="7cb4f-292">Экспортируйте сертификат в формате X.509 с кодировкой base64 и **добавьте только открытый ключ**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-292">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="7cb4f-293">При создании подписки:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-293">When creating a subscription:</span></span>

    - <span data-ttu-id="7cb4f-294">Укажите сертификат в свойстве **encryptionCertificate**, используя контент в кодировке base64, в которой сертификат был экспортирован.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-294">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="7cb4f-295">Укажите ваш собственный идентификатор в свойстве **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-295">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="7cb4f-296">Этот идентификатор позволяет сопоставлять сертификаты с получаемыми уведомлениями, а также получать сертификаты из хранилища сертификатов.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-296">This identifier allows you to match your certificates to the notifications you receive, and to retrieve certificates from your certificate store.</span></span> <span data-ttu-id="7cb4f-297">Длина идентификатора не должна превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-297">The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="7cb4f-298">Обеспечьте защиту закрытого ключа, чтобы ваш код обработки уведомлений мог обращаться к закрытому ключу для расшифровки данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-298">Manage the private key securely, so that your notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="7cb4f-299">Ротация ключей</span><span class="sxs-lookup"><span data-stu-id="7cb4f-299">Rotating keys</span></span>

<span data-ttu-id="7cb4f-300">Чтобы уменьшить риск компрометации закрытого ключа, периодически изменяйте ассиметричные ключи.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-300">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="7cb4f-301">Чтобы добавить новую пару ключей, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-301">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="7cb4f-302">Получите новый сертификат с новой парой асимметричных ключей.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-302">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="7cb4f-303">Используйте его для всех создаваемых подписок.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-303">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="7cb4f-304">Обновите существующие подписки с использованием нового ключа сертификата.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-304">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="7cb4f-305">Выполняйте это в рамках регулярного возобновления подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-305">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="7cb4f-306">Или перечислите все подписки и укажите ключ.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-306">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="7cb4f-307">Используйте [операцию PATCH для подписки](/graph/api/subscription-update?view=graph-rest-1.0) и обновите свойства **encryptionCertificate** и **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-307">Use the [PATCH operation on the subscription](/graph/api/subscription-update?view=graph-rest-1.0) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="7cb4f-308">Учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-308">Keep in mind the following:</span></span>
    - <span data-ttu-id="7cb4f-309">В течение некоторого периода времени старый сертификат по-прежнему можно использовать для шифрования.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-309">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="7cb4f-310">Чтобы расшифровать контент, у вашего приложения должен быть доступ как к старым, так и к новым сертификатам.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-310">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="7cb4f-311">Используйте свойство **encryptionCertificateId** в каждом уведомлении, чтобы определить правильный ключ для использования.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-311">Use the **encryptionCertificateId** property in each notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="7cb4f-312">Удалите старый сертификат, только когда он перестает указываться в последних уведомлениях.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-312">Discard of the old certificate only when you have seen no recent notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="7cb4f-313">Расшифровка данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="7cb4f-313">Decrypting resource data</span></span>

<span data-ttu-id="7cb4f-314">Microsoft Graph использует двухэтапный процесс шифрования с целью оптимизации работы:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-314">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="7cb4f-315">Создается симметричный ключ однократного применения, который используется для шифрования данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-315">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="7cb4f-316">Используется открытый асимметричный ключ (указанный при подписке), чтобы зашифровать симметричный ключ и добавить его в каждое уведомление этой подписки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-316">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each notification of that subscription.</span></span>

<span data-ttu-id="7cb4f-317">Всегда предполагайте, что для каждого элемента в уведомлении используется разный симметричный ключ.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-317">Always assume that the symmetric key is different for each item in the notification.</span></span>

<span data-ttu-id="7cb4f-318">Чтобы расшифровать данные ресурсов, приложение должно выполнить обратные действия, используя свойства в разделе **encryptedContent** в каждом уведомлении:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-318">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each notification:</span></span>

1. <span data-ttu-id="7cb4f-319">Используйте свойство **encryptionCertificateId**, чтобы определить сертификат для использования.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-319">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="7cb4f-320">Инициализируйте криптографический компонент RSA (например, .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) с помощью закрытого ключа.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-320">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="7cb4f-321">Расшифруйте симметричный ключ, указанный в свойстве **dataKey** каждого элемента в уведомлении.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-321">Decrypt the symmetric key delivered in the **dataKey** property of each item in the notification.</span></span>

    <span data-ttu-id="7cb4f-322">Используйте оптимальное асимметричное шифрование с дополнением (OAEP) в качестве алгоритма расшифровки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-322">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="7cb4f-323">Используйте симметричный ключ, чтобы вычислить подпись HMAC-SHA256 значения в объекте **data**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-323">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="7cb4f-324">Сравните его со значением в объекте **dataSignature**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-324">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="7cb4f-325">Если они не совпадают, считайте, что полезные данные были подменены, и не расшифровывайте их.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-325">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="7cb4f-326">Используйте симметричный ключ с AES (например, .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) для расшифровки содержимого в объекте **data**.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-326">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="7cb4f-327">Используйте следующие параметры расшифровки для алгоритма AES:</span><span class="sxs-lookup"><span data-stu-id="7cb4f-327">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="7cb4f-328">Дополнение: PKCS7</span><span class="sxs-lookup"><span data-stu-id="7cb4f-328">Padding: PKCS7</span></span>
        - <span data-ttu-id="7cb4f-329">Режим шифрования: CBC</span><span class="sxs-lookup"><span data-stu-id="7cb4f-329">Cipher mode: CBC</span></span>
    - <span data-ttu-id="7cb4f-330">Настройте "вектор инициализации", скопировав первые 16 байт симметричного ключа, использованного для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-330">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="7cb4f-331">Расшифрованное значение — это строка JSON, представляющая экземпляр ресурса в уведомлении.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-331">The decrypted value is a JSON string that represents the resource instance in the notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="7cb4f-332">Пример: расшифровка уведомления с зашифрованными данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="7cb4f-332">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="7cb4f-333">Ниже приведен пример уведомления, включающего зашифрованные значения свойств экземпляра **chatMessage** в сообщении канала.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-333">The following is an example notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="7cb4f-334">Экземпляр задается значением `@odata.id`.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-334">The instance is specified by the `@odata.id` value.</span></span>

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

<span data-ttu-id="7cb4f-335">В этом разделе содержатся некоторые полезные фрагменты кода, использующие C# и .NET для каждого этапа расшифровки.</span><span class="sxs-lookup"><span data-stu-id="7cb4f-335">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="7cb4f-336">Расшифровка симметричного ключа</span><span class="sxs-lookup"><span data-stu-id="7cb4f-336">Decrypt the symmetric key</span></span>

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

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="7cb4f-337">Сравнение подписи данных с помощью HMAC-SHA256</span><span class="sxs-lookup"><span data-stu-id="7cb4f-337">Compare data signature using HMAC-SHA256</span></span>

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
if (comparisonSignature.equals(encodedHashedData);)
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="7cb4f-338">Расшифровка содержимого данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="7cb4f-338">Decrypt the resource data content</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7cb4f-339">См. также</span><span class="sxs-lookup"><span data-stu-id="7cb4f-339">See also</span></span>

- [<span data-ttu-id="7cb4f-340">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="7cb4f-340">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="7cb4f-341">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="7cb4f-341">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-beta)
- [<span data-ttu-id="7cb4f-342">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-342">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="7cb4f-343">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-343">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="7cb4f-344">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="7cb4f-344">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
