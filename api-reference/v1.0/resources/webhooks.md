# <a name="working-with-webhooks-in-microsoft-graph"></a><span data-ttu-id="06c0f-101">Работа с веб-перехватчиками в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="06c0f-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="06c0f-p101">REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="06c0f-105">С помощью REST API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="06c0f-105">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

* <span data-ttu-id="06c0f-106">Сообщения</span><span class="sxs-lookup"><span data-stu-id="06c0f-106">Messages</span></span>
* <span data-ttu-id="06c0f-107">События</span><span class="sxs-lookup"><span data-stu-id="06c0f-107">Events</span></span>
* <span data-ttu-id="06c0f-108">Контакты</span><span class="sxs-lookup"><span data-stu-id="06c0f-108">Contacts</span></span>
* <span data-ttu-id="06c0f-109">Групповые чаты</span><span class="sxs-lookup"><span data-stu-id="06c0f-109">Group conversations</span></span>
* <span data-ttu-id="06c0f-110">Контент с общим доступом в OneDrive, включая диски, сопоставленные с сайтами SharePoint</span><span class="sxs-lookup"><span data-stu-id="06c0f-110">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
* <span data-ttu-id="06c0f-111">Личные папки пользователя в OneDrive</span><span class="sxs-lookup"><span data-stu-id="06c0f-111">User's personal OneDrive folders</span></span>

<span data-ttu-id="06c0f-112">Например, вы можете создать подписку на определенную папку: `me/mailfolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="06c0f-112">You can create a subscription to a specific folder: `me/mailfolders('inbox')/messages`</span></span>

<span data-ttu-id="06c0f-113">Либо на ресурс верхнего уровня: `me/messages`, `me/contacts`, `me/events`</span><span class="sxs-lookup"><span data-stu-id="06c0f-113">Or to a top-level resource: `me/messages`</span></span>

<span data-ttu-id="06c0f-114">В Sharepoint либо на диске в OneDrive для бизнеса: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="06c0f-114">Or on a Sharepoint / OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="06c0f-115">Либо в личном OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="06c0f-115">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="06c0f-p102">Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке. Затем приложение действует в соответствии с бизнес-логикой. Например, оно получает дополнительные данные, обновляет кэш и представления и т. д.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p102">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span>

<span data-ttu-id="06c0f-p103">Приложения должны обновлять свои подписки до истечения срока действия подписок. На данный момент самый длинный срок действия подписки — три дня минус 90 минут со времени создания подписки. Приложениям необходимо обновлять свои подписки до истечения срока их действия. В противном случае им потребуется создавать новые подписки.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p103">Subscriptions expire. The current longest expiration time is three days minus 90 minutes (4230 in total) from the time of creation. Apps need to renew their subscriptions before the expiration time. Otherwise they'll need to create a new subscription.</span></span>

<span data-ttu-id="06c0f-123">Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="06c0f-123">Apps should renew their subscriptions before they expire. They can also unsubscribe at any time to stop getting notifications.</span></span>

<span data-ttu-id="06c0f-p104">В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api/subscription_post_subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span> 

| <span data-ttu-id="06c0f-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06c0f-128">Permission type</span></span> | <span data-ttu-id="06c0f-129">Типы ресурсов, поддерживаемые в версии 1.0</span><span class="sxs-lookup"><span data-stu-id="06c0f-129">Supported resource types in v1.0</span></span> |
|:----------------|:---------------------------------|
| <span data-ttu-id="06c0f-130">Delegated — рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="06c0f-130">Delegated - work or school account</span></span> | [<span data-ttu-id="06c0f-131">contact](contact.md), [conversation](conversation.md), [drive](drive.md), [event](event.md), [message</span><span class="sxs-lookup"><span data-stu-id="06c0f-131">contact](contact.md), [conversation](conversation.md), [drive](drive.md), [event](event.md), [message</span></span>](message.md) |
| <span data-ttu-id="06c0f-132">Delegated — личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="06c0f-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="06c0f-133">Нет</span><span class="sxs-lookup"><span data-stu-id="06c0f-133">None</span></span> |
| <span data-ttu-id="06c0f-134">Application</span><span class="sxs-lookup"><span data-stu-id="06c0f-134">Application</span></span> | [<span data-ttu-id="06c0f-135">contact](contact.md), [conversation](conversation.md), [event](event.md), [message</span><span class="sxs-lookup"><span data-stu-id="06c0f-135">contact](contact.md), [conversation](conversation.md), [event](event.md), [message</span></span>](message.md) |

## <a name="code-samples"></a><span data-ttu-id="06c0f-136">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="06c0f-136">Code samples</span></span>

<span data-ttu-id="06c0f-137">Указанные ниже примеры кода доступны на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="06c0f-137">The following samples are available on GitHub in the OneDrive organization.</span></span>

* [<span data-ttu-id="06c0f-138">Пример веб-перехватчиков Microsoft Graph для Node.js</span><span class="sxs-lookup"><span data-stu-id="06c0f-138">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="06c0f-139">Пример веб-перехватчиков Microsoft Graph для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="06c0f-139">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

# <a name="creating-a-subscription"></a><span data-ttu-id="06c0f-140">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="06c0f-140">Creating a subscription</span></span>

<span data-ttu-id="06c0f-p105">Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="06c0f-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="06c0f-143">Клиент отправляет запрос (POST) на подписку для определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="06c0f-143">The client sends a subscription (POST) request for a specific resource.</span></span>
2. <span data-ttu-id="06c0f-144">Microsoft Graph проверяет запрос.</span><span class="sxs-lookup"><span data-stu-id="06c0f-144">Microsoft Graph verifies the request.</span></span>
  * <span data-ttu-id="06c0f-145">Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="06c0f-145">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
  * <span data-ttu-id="06c0f-146">В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.</span><span class="sxs-lookup"><span data-stu-id="06c0f-146">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>
3. <span data-ttu-id="06c0f-147">Клиент отправляет маркер проверки обратно в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="06c0f-147">The client sends the validation token back to Microsoft Graph.</span></span>

<span data-ttu-id="06c0f-148">Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления с соответствующими подписками.</span><span class="sxs-lookup"><span data-stu-id="06c0f-148">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

## <a name="notification-url-validation"></a><span data-ttu-id="06c0f-149">Проверка URL-адреса уведомления</span><span class="sxs-lookup"><span data-stu-id="06c0f-149">Notification URL validation</span></span>

<span data-ttu-id="06c0f-p106">Прежде чем создавать подписку, Microsoft Graph проверяет URL-адрес уведомлений в запросе на подписку. Проверка происходит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="06c0f-p106">Microsoft Graph validates the notification URL in a subscription request before creating the subscription. The validation process occurs as follows:</span></span>

1. <span data-ttu-id="06c0f-152">Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:</span><span class="sxs-lookup"><span data-stu-id="06c0f-152">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. <span data-ttu-id="06c0f-153">В течение 10 секунд клиент должен предоставить отклик с указанными ниже характеристиками.</span><span class="sxs-lookup"><span data-stu-id="06c0f-153">The client must provide a response with the following characteristics within 10 seconds:</span></span>

  * <span data-ttu-id="06c0f-154">Код состояния 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="06c0f-154">An 200 (OK) status code.</span></span>
  * <span data-ttu-id="06c0f-155">Необходимый тип контента — текст (в том числе обычный).</span><span class="sxs-lookup"><span data-stu-id="06c0f-155">The content type must be text/plain.</span></span> 
  * <span data-ttu-id="06c0f-156">Текст должен включать маркер проверки, который предоставил Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="06c0f-156">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="06c0f-157">Клиент должен удалить маркер проверки после того, как предоставит его в отклике.</span><span class="sxs-lookup"><span data-stu-id="06c0f-157">The client should discard the validation token after providing it in the response.</span></span>

## <a name="subscription-request-example"></a><span data-ttu-id="06c0f-158">Пример запроса на подписку</span><span class="sxs-lookup"><span data-stu-id="06c0f-158">Subscription request example</span></span>

```
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

<span data-ttu-id="06c0f-p107">Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`. Определения и значения свойств представлены в [описании типа ресурса subscription](subscription.md). Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p107">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required. See [subscription resource type](subscription.md) for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span>

<span data-ttu-id="06c0f-162">В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [subscription](subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="06c0f-162">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](subscription.md) object in the body.</span></span>

# <a name="renewing-a-subscription"></a><span data-ttu-id="06c0f-163">Возобновление подписки</span><span class="sxs-lookup"><span data-stu-id="06c0f-163">Renewing a subscription</span></span>

<span data-ttu-id="06c0f-p108">Клиент может возобновить подписку, указав срок действия до трех дней с момента отправки запроса. Свойство expirationDateTime является обязательным.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p108">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span>

## <a name="subscription-renewal-example"></a><span data-ttu-id="06c0f-166">Пример продления подписки</span><span class="sxs-lookup"><span data-stu-id="06c0f-166">Subscription renewal example</span></span>

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="06c0f-p109">В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [subscription](subscription.md) в тексте отклика. Объект подписки включает новое значение expirationDateTime.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p109">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](subscription.md) object in the body. The subscription object includes the new expirationDateTime value.</span></span> 

# <a name="deleting-a-subscription"></a><span data-ttu-id="06c0f-169">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="06c0f-169">Deleting a subscription</span></span>

<span data-ttu-id="06c0f-170">Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.</span><span class="sxs-lookup"><span data-stu-id="06c0f-170">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="06c0f-171">В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="06c0f-171">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

# <a name="notifications"></a><span data-ttu-id="06c0f-172">Уведомления</span><span class="sxs-lookup"><span data-stu-id="06c0f-172">Notifications</span></span>

<span data-ttu-id="06c0f-p110">После создания подписки клиент начнет получать уведомления. При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений. Клиент получает уведомления только об изменениях определенных типов, например *created*.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p110">The client starts receiving notifications after creating the subscription. Microsoft Graph sends a POST request to the notification URL when changes happen to the resource. The client only gets notifications according to the specified change type, such as *created*.</span></span>

## <a name="notification-properties"></a><span data-ttu-id="06c0f-176">Свойства уведомлений</span><span class="sxs-lookup"><span data-stu-id="06c0f-176">Notification properties</span></span>

<span data-ttu-id="06c0f-177">Объект уведомления содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="06c0f-177">The notification object has the following properties:</span></span>

* <span data-ttu-id="06c0f-178">subscriptionId — идентификатор подписки, к которой относится уведомление.</span><span class="sxs-lookup"><span data-stu-id="06c0f-178">subscriptionId - The ID for the subscription to which this notification belongs.</span></span>
* <span data-ttu-id="06c0f-179">subscriptionExpirationDateTime — время окончания срока действия для подписки.</span><span class="sxs-lookup"><span data-stu-id="06c0f-179">subscriptionExpirationDateTime - The expiration time for the subscription.</span></span>
* <span data-ttu-id="06c0f-180">clientState — свойство clientState, указанное в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="06c0f-180">clientState - The clientState property specified in the subscription request.</span></span>
* <span data-ttu-id="06c0f-p111">changeType — тип события, вызвавшего уведомление. Примеры: *created* при получении сообщения или *updated*, когда сообщение помечается как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p111">changeType - The event type that caused the notification. For example, *created* on mail receive, or *updated* on marking a message read.</span></span>
* <span data-ttu-id="06c0f-183">resource — URI ресурса относительно `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="06c0f-183">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> 
* <span data-ttu-id="06c0f-p112">resourceData — объект, зависящий от ресурса, подписка на который создается.  Например, для ресурсов Outlook:</span><span class="sxs-lookup"><span data-stu-id="06c0f-p112">resourceData - The object dependent on the resource being subscribed to.  For example, for Outlook resources:</span></span>
  * <span data-ttu-id="06c0f-186">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="06c0f-186">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span>
  * <span data-ttu-id="06c0f-187">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="06c0f-187">@odata.id - The OData identifier of the object.</span></span>
  * <span data-ttu-id="06c0f-188">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="06c0f-188">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span>
  * <span data-ttu-id="06c0f-189">id — идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="06c0f-189">id - The identifier of the object.</span></span>


> <span data-ttu-id="06c0f-p113">Примечание. Значение Id, указанное в resourceData, действительно в момент добавления уведомления в очередь. Некоторые действия, например перемещение сообщения в другую папку, могут привести к изменению идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p113">Note: The Id value provided in resourceData is valid at the time the notification was queued. Some actions, such as moving a message to another folder, may result in a resource's Id being changed.</span></span> 

## <a name="notification-example"></a><span data-ttu-id="06c0f-192">Пример уведомления</span><span class="sxs-lookup"><span data-stu-id="06c0f-192">Notification example</span></span>

<span data-ttu-id="06c0f-193">Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления, аналогичные указанному ниже.</span><span class="sxs-lookup"><span data-stu-id="06c0f-193">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
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

<span data-ttu-id="06c0f-p114">Обратите внимание, что объект value содержит список. Если в очереди много уведомлений, Microsoft Graph отправляет их в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p114">Note that the value object contains a list. If there are many queued notifications, Microsoft Graph sends them in a single request.</span></span>

## <a name="processing-the-notification"></a><span data-ttu-id="06c0f-196">Обработка уведомления</span><span class="sxs-lookup"><span data-stu-id="06c0f-196">Processing the notification</span></span>

<span data-ttu-id="06c0f-p115">Когда приложение начинает получать уведомления, оно должно обрабатывать их. Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p115">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="06c0f-p116">Проверьте свойство `clientState`. Свойство clientState в уведомлении должно совпадать со свойством, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p116">Validate the `clientState` property. The clientState property in the notification must match the one submitted with the subscription request.</span></span>
  > <span data-ttu-id="06c0f-p117">Примечание. Если это не так, уведомление не следует рассматривать как действительное. Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p117">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

2. <span data-ttu-id="06c0f-203">Обновляйте приложение в соответствии с бизнес-логикой.</span><span class="sxs-lookup"><span data-stu-id="06c0f-203">Update your application based on your business logic.</span></span>
3. <span data-ttu-id="06c0f-p118">Отправляйте код состояния `202 - Accepted` в ответе, отправляемом в Microsoft Graph. Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="06c0f-p118">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
  > <span data-ttu-id="06c0f-206">Код состояния `202 - Accepted` следует отправлять, даже если свойство clientState не совпадает со значением, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="06c0f-206">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="06c0f-207">Повторяйте эти действия для других уведомлений в запросе.</span><span class="sxs-lookup"><span data-stu-id="06c0f-207">Repeat for other notifications in the request.</span></span>

# <a name="additional-resources"></a><span data-ttu-id="06c0f-208">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="06c0f-208">Additional resources</span></span>

* [<span data-ttu-id="06c0f-209">Тип ресурса Subscription</span><span class="sxs-lookup"><span data-stu-id="06c0f-209">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="06c0f-210">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="06c0f-210">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="06c0f-211">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="06c0f-211">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* [<span data-ttu-id="06c0f-212">Пример Microsoft Graph Webhooks для Node.js</span><span class="sxs-lookup"><span data-stu-id="06c0f-212">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="06c0f-213">Пример Microsoft Graph Webhooks для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="06c0f-213">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
