---
title: Настройка уведомлений об изменениях, включающих данные ресурсов
description: Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Уведомления об изменениях могут включать свойства ресурсов.
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 4da690a646c47ef857de860d36bde17a4ee26761
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547185"
---
# <a name="set-up-change-notifications-that-include-resource-data"></a><span data-ttu-id="2526d-104">Настройка уведомлений об изменениях, включающих данные ресурсов</span><span class="sxs-lookup"><span data-stu-id="2526d-104">Set up change notifications that include resource data</span></span>

<span data-ttu-id="2526d-105">Microsoft Graph позволяет приложениям подписываться на уведомления об изменениях ресурсов с использованием [веб-перехватчиков](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="2526d-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="2526d-106">Вы можете настроить подписки таким образом, чтобы в уведомления об изменениях включались данные измененных ресурсов (например, содержимое сообщения чата из Microsoft Teams или сведения о присутствии из Microsoft Teams).</span><span class="sxs-lookup"><span data-stu-id="2526d-106">You can set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message or Microsoft Teams presence information) in change notifications.</span></span> <span data-ttu-id="2526d-107">Затем приложение сможет запустить свою бизнес-логику без отдельного вызова API для получения измененного ресурса.</span><span class="sxs-lookup"><span data-stu-id="2526d-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="2526d-108">В результате приложение работает эффективнее, выполняя меньше вызовов API, что полезно в крупномасштабных сценариях.</span><span class="sxs-lookup"><span data-stu-id="2526d-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="2526d-109">Добавление данных ресурса в уведомления об изменениях требует реализации следующей дополнительной логики, чтобы выполнить требования по доступу к данным и их безопасности.</span><span class="sxs-lookup"><span data-stu-id="2526d-109">Including resource data as part of change notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="2526d-110">[Применяйте](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications)) специальные уведомления жизненного цикла подписки (предварительную версию), чтобы обеспечить непрерывный поток данных.</span><span class="sxs-lookup"><span data-stu-id="2526d-110">[Handle](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications)) special subscription lifecycle notifications (preview) to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="2526d-111">Microsoft Graph периодически отправляет уведомления жизненного цикла, требуя от приложения повторной авторизации, чтобы обеспечить отсутствие неожиданных проблем с доступом при включении данных ресурсов в уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2526d-111">Microsoft Graph sends lifecycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in change notifications.</span></span>
- <span data-ttu-id="2526d-112">[Проверяйте](#validating-the-authenticity-of-notifications) подлинность уведомлений об изменениях, подтверждая что их источником является Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2526d-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of change notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="2526d-113">[Предоставьте](#decrypting-resource-data-from-change-notifications) открытый ключ шифрования и используйте закрытый ключ для расшифровки данных ресурсов, полученных в уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2526d-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through change notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="2526d-114">Сведения ресурсов в полезных данных уведомлений</span><span class="sxs-lookup"><span data-stu-id="2526d-114">Resource data in notification payload</span></span>

<span data-ttu-id="2526d-115">Обычно этот тип уведомлений об изменениях содержит следующие сведения ресурсов в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="2526d-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="2526d-116">Идентификатор и тип измененного экземпляра ресурса, возвращаемые в свойстве **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="2526d-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="2526d-117">Все значения свойств экземпляра ресурса, зашифрованные в соответствии с подпиской и возвращаемые в свойстве **encryptedContent**.</span><span class="sxs-lookup"><span data-stu-id="2526d-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="2526d-118">Или зависимые от ресурса определенные свойства, возвращаемые в свойстве **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="2526d-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="2526d-119">Чтобы получить только определенные свойства, их нужно указать в URL-адресе объекта **resource** в подписке, используя параметр `$select`.</span><span class="sxs-lookup"><span data-stu-id="2526d-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="2526d-120">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="2526d-120">Supported resources</span></span>

<span data-ttu-id="2526d-121">В настоящее время ресурсы [chatMessage](/graph/api/resources/chatmessage) и [presence](/graph/api/resources/presence) (предварительная версия) в Microsoft Teams поддерживают уведомления об изменениях, включающие данные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2526d-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) as well as the Microsoft Teams [presence](/graph/api/resources/presence) (preview) resources supports change notifications that include resource data.</span></span> <span data-ttu-id="2526d-122">В частности, вы можете настроить подписку, относящуюся к одному из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="2526d-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="2526d-123">Новые или измененные сообщения в определенном канале Teams: `/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="2526d-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="2526d-124">Новые или измененные сообщения во всех каналах Teams всей организации (клиент): `/teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="2526d-124">New or changed messages in all Teams channels: `/teams/getAllMessages`</span></span>
- <span data-ttu-id="2526d-125">Новые или измененные сообщения в определенном чате Teams: `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="2526d-125">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>
- <span data-ttu-id="2526d-126">Новые или измененные сообщения во всех чатах всей организации (клиент): `/chats/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="2526d-126">New or changed messages in all Teams chats: `/chats/getAllMessages`</span></span>
- <span data-ttu-id="2526d-127">Обновление сведений о присутствии пользователя: `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="2526d-127">User's presence information update: `/communications/presences/{id}`</span></span>

<span data-ttu-id="2526d-128">Ресурсы **chatMessage** и **presence** (предварительная версия) поддерживают включение в уведомление об изменениях всех свойств измененного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="2526d-128">The **chatMessage** and the **presence** (preview) resources support including all the properties of a changed instance in a change notification.</span></span> <span data-ttu-id="2526d-129">Они не поддерживают возвращение только выбранных свойств экземпляра.</span><span class="sxs-lookup"><span data-stu-id="2526d-129">They do not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="2526d-130">В этой статье рассматривается пример подписки на уведомления об изменениях в канале Teams. При этом каждое уведомление об изменении содержит все данные ресурсов измененного экземпляра **chatMessage**.</span><span class="sxs-lookup"><span data-stu-id="2526d-130">This article walks through an example that shows you how to subscribe to change notifications for messages in a Teams channel, with each change notification including the full resource data of the changed **chatMessage** instance.</span></span> <span data-ttu-id="2526d-131">Дополнительные сведения о подписках на основе объекта **chatMessage** см. в статье [Получение уведомлений об изменениях для сообщений чатов и каналов](teams-changenotifications-chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="2526d-131">For more details about **chatMessage**-based subscriptions, see [Get change notifications for chat and channel messages](teams-changenotifications-chatmessage.md).</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="2526d-132">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="2526d-132">Creating a subscription</span></span>

<span data-ttu-id="2526d-133">Чтобы включить данные ресурсов в уведомления об изменениях, **требуется** указать следующие свойства в дополнение к обычно указываемым при [создании подписки](webhooks.md#creating-a-subscription):</span><span class="sxs-lookup"><span data-stu-id="2526d-133">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="2526d-134">**includeResourceData**, которому следует присвоить значение `true`, чтобы явно запросить данные ресурса.</span><span class="sxs-lookup"><span data-stu-id="2526d-134">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="2526d-135">**encryptionCertificate**, содержащее только открытый ключ, используемый Microsoft Graph для шифрования данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="2526d-135">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="2526d-136">Сохраняйте соответствующий закрытый ключ для [расшифровки контента](#decrypting-resource-data-from-change-notifications).</span><span class="sxs-lookup"><span data-stu-id="2526d-136">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="2526d-137">**encryptionCertificateId**, являющееся вашим собственным идентификатором для сертификата.</span><span class="sxs-lookup"><span data-stu-id="2526d-137">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="2526d-138">Используйте этот идентификатор для определения в каждом уведомлении об изменениях сертификата, используемого для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="2526d-138">Use this ID to match in each change notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="2526d-139">Учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="2526d-139">Keep the following in mind:</span></span>

- <span data-ttu-id="2526d-140">Проверьте обе конечные точки, как описано в ст. [Проверка конечной точки уведомлений](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="2526d-140">Validate both endpoints as described in [Notification endpoint validation](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="2526d-141">Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.</span><span class="sxs-lookup"><span data-stu-id="2526d-141">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="2526d-142">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="2526d-142">Subscription request example</span></span>

<span data-ttu-id="2526d-143">В приведенном ниже примере показано, как подписаться на сообщения канала, созданные или обновляемые в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2526d-143">The following example subscribes to channel messages being created or updated in Microsoft Teams.</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a><span data-ttu-id="2526d-144">Отклик подписки</span><span class="sxs-lookup"><span data-stu-id="2526d-144">Subscription response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications-preview"></a><span data-ttu-id="2526d-145">Уведомления жизненного цикла подписки (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2526d-145">Subscription lifecycle notifications (preview)</span></span>

<span data-ttu-id="2526d-146">Некоторые события могут воздействовать на поток уведомлений об изменениях в существующей подписке.</span><span class="sxs-lookup"><span data-stu-id="2526d-146">Certain events can interfere with change notification flow in an existing subscription.</span></span> <span data-ttu-id="2526d-147">Уведомления жизненного цикла подписки указывают необходимые действия для обеспечения непрерывного потока.</span><span class="sxs-lookup"><span data-stu-id="2526d-147">Subscription lifecycle notifications inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="2526d-148">В отличие от уведомления об изменении ресурса, информирующем об изменении экземпляра ресурса, уведомление жизненного цикла относится к самой подписке и ее текущему состоянию в жизненном цикле.</span><span class="sxs-lookup"><span data-stu-id="2526d-148">Unlike a resource change notification which informs a change to a resource instance, a lifecycle notification is about the subscription itself, and its current state in the lifecycle.</span></span> 

<span data-ttu-id="2526d-149">Дополнительные сведения о том, как получать уведомления в жизненном цикле (предварительная версия), а также отвечать на них, см. в статье [Уменьшение числа пропущенных подписок и уведомлений об изменениях (предварительная версия)](webhooks-lifecycle.md)</span><span class="sxs-lookup"><span data-stu-id="2526d-149">For more information about how to receive, and respond to, lifecycle notifications (preview), see [Reduce missing subscriptions and change notifications (preview)](webhooks-lifecycle.md)</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="2526d-150">Проверка подлинности уведомлений</span><span class="sxs-lookup"><span data-stu-id="2526d-150">Validating the authenticity of notifications</span></span>

<span data-ttu-id="2526d-151">Приложения часто запускают бизнес-логику на основе данных ресурсов, включенных в уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2526d-151">Apps often run business logic based on resource data included in change notifications.</span></span> <span data-ttu-id="2526d-152">Важно сначала проверить подлинность каждого уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2526d-152">Verifying the authenticity of each change notification first is important.</span></span> <span data-ttu-id="2526d-153">В противном случае посторонние смогут обмануть ваше приложение с помощью ложных уведомлений об изменениях, заставить его неправильно выполнять бизнес-логику, что приведет к нарушению безопасности.</span><span class="sxs-lookup"><span data-stu-id="2526d-153">Otherwise, a third party can spoof your app with false change notifications and make it run its business logic incorrectly, and this can lead to a security incident.</span></span>

<span data-ttu-id="2526d-154">Для основных уведомлений об изменениях, не содержащих данные ресурсов, просто проверьте их на основе значения **clientState**, как описано здесь [Обработка уведомлений об изменениях](webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="2526d-154">For basic change notifications that do not contain resource data, simply validate them based on the **clientState** value as described in [Processing the change notification](webhooks.md#processing-the-change-notification).</span></span> <span data-ttu-id="2526d-155">Это приемлемо, так как вы можете выполнять последующие надежные вызовы Microsoft Graph, чтобы получить доступ к данным ресурсов и, следовательно, влияние любых попыток подмены ограничено.</span><span class="sxs-lookup"><span data-stu-id="2526d-155">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="2526d-156">Для уведомлений об изменениях, доставляющих данные ресурсов, проведите более тщательную проверку перед обработкой данных.</span><span class="sxs-lookup"><span data-stu-id="2526d-156">For change notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="2526d-157">Содержание:</span><span class="sxs-lookup"><span data-stu-id="2526d-157">In this section:</span></span>

- [<span data-ttu-id="2526d-158">Маркеры проверки в уведомлении об изменениях</span><span class="sxs-lookup"><span data-stu-id="2526d-158">Validation tokens in the change notification</span></span>](#validation-tokens-in-the-change-notification)
- [<span data-ttu-id="2526d-159">Способ проверки</span><span class="sxs-lookup"><span data-stu-id="2526d-159">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="2526d-160">Пример маркера JWT</span><span class="sxs-lookup"><span data-stu-id="2526d-160">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a><span data-ttu-id="2526d-161">Маркеры проверки в уведомлении об изменениях</span><span class="sxs-lookup"><span data-stu-id="2526d-161">Validation tokens in the change notification</span></span>

<span data-ttu-id="2526d-162">Уведомление об изменениях с данными ресурсов содержит дополнительное свойство **validationTokens**, содержащее массив маркеров JWT, созданных Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2526d-162">A change notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="2526d-163">Microsoft Graph создает один маркер для каждой отдельной пары приложения и клиента, для которой существует элемент в массиве **value**.</span><span class="sxs-lookup"><span data-stu-id="2526d-163">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="2526d-164">Учитывайте, что уведомления об изменениях могут содержать разные элементы для различных приложений и клиентов, подписанных с помощью одинакового значения **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="2526d-164">Keep in mind that change notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="2526d-165">В следующем примере уведомление об изменении содержит два элемента для одного приложения и двух разных клиентов, поэтому массив **validationTokens** содержит два маркера, требующих проверки.</span><span class="sxs-lookup"><span data-stu-id="2526d-165">In the following example, the change notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

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

> <span data-ttu-id="2526d-166">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="2526d-166">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="how-to-validate"></a><span data-ttu-id="2526d-167">Способ проверки</span><span class="sxs-lookup"><span data-stu-id="2526d-167">How to validate</span></span>

<span data-ttu-id="2526d-168">Если вы незнакомы с проверкой маркеров, см. обзор в статье [Принципы проверки маркера](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/).</span><span class="sxs-lookup"><span data-stu-id="2526d-168">If you're new to token validation, see [Principles of Token Validation](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for an overview.</span></span> <span data-ttu-id="2526d-169">Используйте пакет SDK, например библиотеку [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) для .NET или стороннюю библиотеку для другой платформы.</span><span class="sxs-lookup"><span data-stu-id="2526d-169">Use an SDK, such as the [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third-party library for a different platform.</span></span>

<span data-ttu-id="2526d-170">Следует учитывать следующее:</span><span class="sxs-lookup"><span data-stu-id="2526d-170">Be mindful of the following:</span></span> 

- <span data-ttu-id="2526d-171">Всегда отправляйте код состояния `HTTP 202 Accepted` в ответе на уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="2526d-171">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the change notification.</span></span> 
- <span data-ttu-id="2526d-172">Дайте ответ перед проверкой уведомления об изменении (например, если вы храните уведомления об изменениях в очередях для последующей обработки) или после нее (если они обрабатываются на ходу), даже если проверка завершилась сбоем.</span><span class="sxs-lookup"><span data-stu-id="2526d-172">Respond before validating the change notification (for example, if you store change notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="2526d-173">Принятие уведомления об изменении позволяет избежать ненужных повторений доставки, а также мешает любым возможным злоумышленникам выяснить, прошли ли они проверку.</span><span class="sxs-lookup"><span data-stu-id="2526d-173">Accepting a change notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="2526d-174">Вы всегда можете игнорировать неверное уведомление об изменении после его принятия.</span><span class="sxs-lookup"><span data-stu-id="2526d-174">You can always choose to ignore an invalid change notification after you have accepted it.</span></span>

<span data-ttu-id="2526d-175">В частности, выполняйте проверку каждого маркера JWT в коллекции **validationTokens**.</span><span class="sxs-lookup"><span data-stu-id="2526d-175">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="2526d-176">Если любой из маркеров не прошел проверку, считайте уведомление об изменении подозрительным и выполните дальнейшее исследование.</span><span class="sxs-lookup"><span data-stu-id="2526d-176">If any tokens fail, consider the change notification suspicious and investigate further.</span></span> 

<span data-ttu-id="2526d-177">Для проверки маркеров и приложений, создающих маркеры, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="2526d-177">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="2526d-178">Убедитесь, что срок действия маркера не истек.</span><span class="sxs-lookup"><span data-stu-id="2526d-178">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="2526d-179">Проверьте, что маркер не был подделан и был выдан ожидаемым центром авторизации (платформой удостоверений Майкрософт для разработчиков):</span><span class="sxs-lookup"><span data-stu-id="2526d-179">Validate the token has not been tampered with and was issued by the expected authority, Microsoft identity platform:</span></span>

    - <span data-ttu-id="2526d-180">Получите ключи подписи от общей конечной точки конфигурации: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span><span class="sxs-lookup"><span data-stu-id="2526d-180">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="2526d-181">Эта конфигурация кэшируется приложением на определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="2526d-181">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="2526d-182">Имейте в виду, что конфигурация часто обновляется, так как ключи входа ежедневно меняются.</span><span class="sxs-lookup"><span data-stu-id="2526d-182">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="2526d-183">Проверьте подпись маркера JWT, использующего эти ключи.</span><span class="sxs-lookup"><span data-stu-id="2526d-183">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="2526d-184">Не принимайте маркеры, выпущенные любыми другими центрами.</span><span class="sxs-lookup"><span data-stu-id="2526d-184">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="2526d-185">Проверьте, что маркер выпущен для вашего приложения, подписавшегося на уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2526d-185">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="2526d-186">Следующие действия являются частью стандартной логики проверки в библиотеках маркеров JWT, и обычно их можно выполнять в виде вызова одной функции.</span><span class="sxs-lookup"><span data-stu-id="2526d-186">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="2526d-187">Убедитесь, что "аудитория" в маркере совпадает с идентификатором вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="2526d-187">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="2526d-188">Если уведомления об изменениях получают несколько приложений, выполните проверку по нескольким идентификаторам.</span><span class="sxs-lookup"><span data-stu-id="2526d-188">If you have more than one app receiving change notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="2526d-189">**Важно**. Убедитесь, что приложение, создавшее маркер, представляет издателя уведомления об изменениях Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2526d-189">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="2526d-190">Проверьте, что свойство **appid** в маркере соответствует ожидаемому значению `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span><span class="sxs-lookup"><span data-stu-id="2526d-190">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="2526d-191">Это гарантирует, что уведомления об изменениях не отправляются другим приложением, отличным от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2526d-191">This ensures that change notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="2526d-192">Пример маркера JWT</span><span class="sxs-lookup"><span data-stu-id="2526d-192">Example JWT token</span></span>

<span data-ttu-id="2526d-193">Ниже приведен пример свойств, входящих в маркер JWT, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="2526d-193">The following is an example of the properties included in the JWT token that are needed for validation.</span></span>

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

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="2526d-194">Пример: подтверждение маркеров проверки</span><span class="sxs-lookup"><span data-stu-id="2526d-194">Example: Verifying validation tokens</span></span>

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
<span data-ttu-id="2526d-195">Чтобы пример Java работал, вам также необходимо реализовать `JwkKeyResolver`.</span><span class="sxs-lookup"><span data-stu-id="2526d-195">For the Java sample to work, you will also need to implement the `JwkKeyResolver`.</span></span>  
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

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="2526d-196">Расшифровка данных ресурсов из уведомлений об изменениях</span><span class="sxs-lookup"><span data-stu-id="2526d-196">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="2526d-197">Свойство **resourceData** уведомления об изменении содержит только основной идентификатор и сведения о типе экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="2526d-197">The **resourceData** property of a change notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="2526d-198">Свойство **encryptedData** содержит полные данные о ресурсе, зашифрованные Microsoft Graph с использованием открытого ключа, указанного в подписке.</span><span class="sxs-lookup"><span data-stu-id="2526d-198">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="2526d-199">Это свойство также содержит значения, необходимые для проверки и расшифровки.</span><span class="sxs-lookup"><span data-stu-id="2526d-199">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="2526d-200">Это выполняется для повышения безопасности пользовательских данных, к которым получен доступ с помощью уведомлений об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2526d-200">This is done to increase the security of customer data accessed via change notifications.</span></span> <span data-ttu-id="2526d-201">Вы отвечаете за защиту закрытого ключа, чтобы гарантировать невозможность расшифровки пользовательских данных посторонними, даже если они смогли перехватить исходные уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2526d-201">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original change notifications.</span></span>

<span data-ttu-id="2526d-202">Содержание:</span><span class="sxs-lookup"><span data-stu-id="2526d-202">In this section:</span></span>

- [<span data-ttu-id="2526d-203">Управление ключами шифрования</span><span class="sxs-lookup"><span data-stu-id="2526d-203">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="2526d-204">Расшифровка данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="2526d-204">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="2526d-205">Пример: расшифровка уведомления с зашифрованными данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="2526d-205">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="2526d-206">Управление ключами шифрования</span><span class="sxs-lookup"><span data-stu-id="2526d-206">Managing encryption keys</span></span>

1. <span data-ttu-id="2526d-207">Получите сертификат с парой асимметричных ключей.</span><span class="sxs-lookup"><span data-stu-id="2526d-207">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="2526d-208">Вы можете самостоятельно подписать сертификат, так как Microsoft Graph не проверяет поставщика сертификата и использует открытый ключ только для шифрования.</span><span class="sxs-lookup"><span data-stu-id="2526d-208">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="2526d-209">В качестве решения для создания и ротации сертификатов, а также безопасного управления ими используйте [Azure Key Vault](/azure/key-vault/key-vault-whatis).</span><span class="sxs-lookup"><span data-stu-id="2526d-209">Use [Azure Key Vault](/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="2526d-210">Убедитесь, что ключи удовлетворяют следующим условиям:</span><span class="sxs-lookup"><span data-stu-id="2526d-210">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="2526d-211">Ключ должен быть типа `RSA`</span><span class="sxs-lookup"><span data-stu-id="2526d-211">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="2526d-212">Размер ключа должен находиться в диапазоне от 2048 до 4096 бит</span><span class="sxs-lookup"><span data-stu-id="2526d-212">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="2526d-213">Экспортируйте сертификат в формате X.509 с кодировкой base64 и **добавьте только открытый ключ**.</span><span class="sxs-lookup"><span data-stu-id="2526d-213">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="2526d-214">При создании подписки:</span><span class="sxs-lookup"><span data-stu-id="2526d-214">When creating a subscription:</span></span>

    - <span data-ttu-id="2526d-215">Укажите сертификат в свойстве **encryptionCertificate**, используя контент в кодировке base64, в которой сертификат был экспортирован.</span><span class="sxs-lookup"><span data-stu-id="2526d-215">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="2526d-216">Укажите ваш собственный идентификатор в свойстве **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="2526d-216">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="2526d-p121">Этот идентификатор позволяет сопоставлять сертификаты с получаемыми уведомлениями об изменениях, а также получать сертификаты из хранилища сертификатов. Длина идентификатора не должна превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="2526d-p121">This identifier allows you to match your certificates to the change notifications you receive, and to retrieve certificates from your certificate store. The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="2526d-219">Обеспечьте защиту закрытого ключа, чтобы ваш код обработки уведомлений об изменениях мог обращаться к закрытому ключу для расшифровки данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2526d-219">Manage the private key securely, so that your change notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="2526d-220">Ротация ключей</span><span class="sxs-lookup"><span data-stu-id="2526d-220">Rotating keys</span></span>

<span data-ttu-id="2526d-221">Чтобы уменьшить риск компрометации закрытого ключа, периодически изменяйте ассиметричные ключи.</span><span class="sxs-lookup"><span data-stu-id="2526d-221">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="2526d-222">Чтобы добавить новую пару ключей, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="2526d-222">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="2526d-223">Получите новый сертификат с новой парой асимметричных ключей.</span><span class="sxs-lookup"><span data-stu-id="2526d-223">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="2526d-224">Используйте его для всех создаваемых подписок.</span><span class="sxs-lookup"><span data-stu-id="2526d-224">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="2526d-225">Обновите существующие подписки с использованием нового ключа сертификата.</span><span class="sxs-lookup"><span data-stu-id="2526d-225">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="2526d-226">Выполняйте это в рамках регулярного возобновления подписки.</span><span class="sxs-lookup"><span data-stu-id="2526d-226">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="2526d-227">Или перечислите все подписки и укажите ключ.</span><span class="sxs-lookup"><span data-stu-id="2526d-227">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="2526d-228">Используйте [операцию PATCH для подписки](/graph/api/subscription-update) и обновите свойства **encryptionCertificate** и **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="2526d-228">Use the [PATCH operation on the subscription](/graph/api/subscription-update) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="2526d-229">Учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="2526d-229">Keep in mind the following:</span></span>
    - <span data-ttu-id="2526d-230">В течение некоторого периода времени старый сертификат по-прежнему можно использовать для шифрования.</span><span class="sxs-lookup"><span data-stu-id="2526d-230">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="2526d-231">Чтобы расшифровать контент, у вашего приложения должен быть доступ как к старым, так и к новым сертификатам.</span><span class="sxs-lookup"><span data-stu-id="2526d-231">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="2526d-232">Используйте свойство **encryptionCertificateId** в каждом уведомлении об изменении, чтобы определить правильный ключ для использования.</span><span class="sxs-lookup"><span data-stu-id="2526d-232">Use the **encryptionCertificateId** property in each change notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="2526d-233">Удалите старый сертификат, только когда он перестает указываться в последних уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2526d-233">Discard of the old certificate only when you have seen no recent change notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="2526d-234">Расшифровка данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="2526d-234">Decrypting resource data</span></span>

<span data-ttu-id="2526d-235">Microsoft Graph использует двухэтапный процесс шифрования с целью оптимизации работы:</span><span class="sxs-lookup"><span data-stu-id="2526d-235">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="2526d-236">Создается симметричный ключ однократного применения, который используется для шифрования данных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2526d-236">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="2526d-237">Используется открытый асимметричный ключ (указанный при подписке), чтобы зашифровать симметричный ключ и добавить его в каждое уведомление об изменении этой подписки.</span><span class="sxs-lookup"><span data-stu-id="2526d-237">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each change notification of that subscription.</span></span>

<span data-ttu-id="2526d-238">Всегда предполагайте, что для каждого элемента в уведомлении об изменении используется разный симметричный ключ.</span><span class="sxs-lookup"><span data-stu-id="2526d-238">Always assume that the symmetric key is different for each item in the change notification.</span></span>

<span data-ttu-id="2526d-239">Чтобы расшифровать данные ресурсов, приложение должно выполнить обратные действия, используя свойства в разделе **encryptedContent** в каждом уведомлении об изменении:</span><span class="sxs-lookup"><span data-stu-id="2526d-239">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each change notification:</span></span>

1. <span data-ttu-id="2526d-240">Используйте свойство **encryptionCertificateId**, чтобы определить сертификат для использования.</span><span class="sxs-lookup"><span data-stu-id="2526d-240">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="2526d-241">Инициализируйте криптографический компонент RSA (например, .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) с помощью закрытого ключа.</span><span class="sxs-lookup"><span data-stu-id="2526d-241">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="2526d-242">Расшифруйте симметричный ключ, указанный в свойстве **dataKey** каждого элемента в уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="2526d-242">Decrypt the symmetric key delivered in the **dataKey** property of each item in the change notification.</span></span>

    <span data-ttu-id="2526d-243">Используйте оптимальное асимметричное шифрование с дополнением (OAEP) в качестве алгоритма расшифровки.</span><span class="sxs-lookup"><span data-stu-id="2526d-243">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="2526d-244">Используйте симметричный ключ, чтобы вычислить подпись HMAC-SHA256 значения в объекте **data**.</span><span class="sxs-lookup"><span data-stu-id="2526d-244">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="2526d-245">Сравните его со значением в объекте **dataSignature**.</span><span class="sxs-lookup"><span data-stu-id="2526d-245">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="2526d-246">Если они не совпадают, считайте, что полезные данные были подменены, и не расшифровывайте их.</span><span class="sxs-lookup"><span data-stu-id="2526d-246">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="2526d-247">Используйте симметричный ключ с AES (например, .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) для расшифровки содержимого в объекте **data**.</span><span class="sxs-lookup"><span data-stu-id="2526d-247">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="2526d-248">Используйте следующие параметры расшифровки для алгоритма AES:</span><span class="sxs-lookup"><span data-stu-id="2526d-248">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="2526d-249">Дополнение: PKCS7</span><span class="sxs-lookup"><span data-stu-id="2526d-249">Padding: PKCS7</span></span>
        - <span data-ttu-id="2526d-250">Режим шифрования: CBC</span><span class="sxs-lookup"><span data-stu-id="2526d-250">Cipher mode: CBC</span></span>
    - <span data-ttu-id="2526d-251">Настройте "вектор инициализации", скопировав первые 16 байт симметричного ключа, использованного для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="2526d-251">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="2526d-252">Расшифрованное значение — это строка JSON, представляющая экземпляр ресурса в уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="2526d-252">The decrypted value is a JSON string that represents the resource instance in the change notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="2526d-253">Пример: расшифровка уведомления с зашифрованными данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="2526d-253">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="2526d-254">Ниже приведен пример уведомления об изменении, включающего зашифрованные значения свойств экземпляра **chatMessage** в сообщении канала.</span><span class="sxs-lookup"><span data-stu-id="2526d-254">The following is an example change notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="2526d-255">Экземпляр задается значением `@odata.id`.</span><span class="sxs-lookup"><span data-stu-id="2526d-255">The instance is specified by the `@odata.id` value.</span></span>

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

> <span data-ttu-id="2526d-256">**Примечание.** Полное описание данных, отправленных при доставке уведомлений об изменениях, см. в [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="2526d-256">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>


<span data-ttu-id="2526d-257">В этом разделе содержатся некоторые полезные фрагменты кода, использующие C# и .NET для каждого этапа расшифровки.</span><span class="sxs-lookup"><span data-stu-id="2526d-257">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="2526d-258">Расшифровка симметричного ключа</span><span class="sxs-lookup"><span data-stu-id="2526d-258">Decrypt the symmetric key</span></span>

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

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="2526d-259">Сравнение подписи данных с помощью HMAC-SHA256</span><span class="sxs-lookup"><span data-stu-id="2526d-259">Compare data signature using HMAC-SHA256</span></span>

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

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="2526d-260">Расшифровка содержимого данных ресурсов</span><span class="sxs-lookup"><span data-stu-id="2526d-260">Decrypt the resource data content</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2526d-261">См. также</span><span class="sxs-lookup"><span data-stu-id="2526d-261">See also</span></span>

- [<span data-ttu-id="2526d-262">Настройка уведомлений об изменениях в пользовательских данных</span><span class="sxs-lookup"><span data-stu-id="2526d-262">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="2526d-263">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="2526d-263">Subscription resource type</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="2526d-264">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="2526d-264">Get subscription</span></span>](/graph/api/subscription-get)
- [<span data-ttu-id="2526d-265">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="2526d-265">Create subscription</span></span>](/graph/api/subscription-post-subscriptions)
- [<span data-ttu-id="2526d-266">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="2526d-266">Update subscription</span></span>](/graph/api/subscription-update)
