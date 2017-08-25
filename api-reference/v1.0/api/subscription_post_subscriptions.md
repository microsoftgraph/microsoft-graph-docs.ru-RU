# <a name="create-subscription"></a><span data-ttu-id="59571-101">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="59571-101">Create subscription</span></span>

<span data-ttu-id="59571-102">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="59571-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>
## <a name="permissions"></a><span data-ttu-id="59571-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59571-103">Permissions</span></span>
<span data-ttu-id="59571-p101">Создание подписки требует наличия области чтения для ресурса. Например, чтобы получать сообщения уведомлений, приложению необходимо разрешение `Mail.Read`. В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="59571-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="59571-108">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="59571-108">Resource type / Item</span></span>        | <span data-ttu-id="59571-109">Разрешение</span><span class="sxs-lookup"><span data-stu-id="59571-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="59571-110">Contacts</span><span class="sxs-lookup"><span data-stu-id="59571-110">Contacts</span></span>                    | <span data-ttu-id="59571-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="59571-111">Contacts.Read</span></span>       |
| <span data-ttu-id="59571-112">Беседы</span><span class="sxs-lookup"><span data-stu-id="59571-112">Conversations</span></span>               | <span data-ttu-id="59571-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="59571-113">Group.Read.All</span></span>      |
| <span data-ttu-id="59571-114">События</span><span class="sxs-lookup"><span data-stu-id="59571-114">Events</span></span>                      | <span data-ttu-id="59571-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="59571-115">Calendars.Read</span></span>      |
| <span data-ttu-id="59571-116">Сообщения</span><span class="sxs-lookup"><span data-stu-id="59571-116">Messages</span></span>                    | <span data-ttu-id="59571-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="59571-117">Mail.Read</span></span>           |
| <span data-ttu-id="59571-118">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="59571-118">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="59571-119">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="59571-119">Files.ReadWrite</span></span>     |
| <span data-ttu-id="59571-120">Диски (контент и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="59571-120">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="59571-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59571-121">Files.ReadWrite.All</span></span> |

 <span data-ttu-id="59571-p102">***Примечание.*** Конечная точка /v1.0 позволяет использовать разрешения для приложений в случае большинства ресурсов. Тип ресурсов Conversations в корневых элементах диска Group и OneDrive не поддерживает разрешения для приложений.</span><span class="sxs-lookup"><span data-stu-id="59571-p102">***Note:*** The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="59571-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59571-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a><span data-ttu-id="59571-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59571-125">Request headers</span></span>
| <span data-ttu-id="59571-126">Имя</span><span class="sxs-lookup"><span data-stu-id="59571-126">Name</span></span>       | <span data-ttu-id="59571-127">Тип</span><span class="sxs-lookup"><span data-stu-id="59571-127">Type</span></span> | <span data-ttu-id="59571-128">Описание</span><span class="sxs-lookup"><span data-stu-id="59571-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59571-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="59571-129">Authorization</span></span>  | <span data-ttu-id="59571-130">string</span><span class="sxs-lookup"><span data-stu-id="59571-130">string</span></span>  | <span data-ttu-id="59571-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59571-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="59571-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="59571-133">Response</span></span>

<span data-ttu-id="59571-134">В случае успеха этот метод возвращает код отклика `201, Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="59571-134">If successful, this method returns `201, Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59571-135">Пример</span><span class="sxs-lookup"><span data-stu-id="59571-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59571-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="59571-136">Request</span></span>
<span data-ttu-id="59571-137">Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="59571-137">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->
```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "subscription-identifier"
}
```
<span data-ttu-id="59571-p104">Предоставьте в теле запроса описание объекта [subscription](../resources/subscription.md) в формате JSON. Поле *clientState* не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="59571-p104">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object. The *clientState* field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="59571-140">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="59571-140">Resources examples</span></span>
<span data-ttu-id="59571-141">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="59571-141">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="59571-142">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="59571-142">Resource type</span></span> | <span data-ttu-id="59571-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="59571-143">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="59571-144">Mail</span><span class="sxs-lookup"><span data-stu-id="59571-144">Mail</span></span>|<span data-ttu-id="59571-145">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="59571-145">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="59571-146">me/messages</span><span class="sxs-lookup"><span data-stu-id="59571-146">me/messages</span></span>|
|<span data-ttu-id="59571-147">Contacts</span><span class="sxs-lookup"><span data-stu-id="59571-147">Contacts</span></span>|<span data-ttu-id="59571-148">me/contacts</span><span class="sxs-lookup"><span data-stu-id="59571-148">me/contacts</span></span>|
|<span data-ttu-id="59571-149">Calendars</span><span class="sxs-lookup"><span data-stu-id="59571-149">Calendars</span></span>|<span data-ttu-id="59571-150">me/events</span><span class="sxs-lookup"><span data-stu-id="59571-150">me/events</span></span>|
|<span data-ttu-id="59571-151">Conversations</span><span class="sxs-lookup"><span data-stu-id="59571-151">Conversations</span></span>|<span data-ttu-id="59571-152">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="59571-152">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="59571-153">Drives</span><span class="sxs-lookup"><span data-stu-id="59571-153">Drives</span></span>|<span data-ttu-id="59571-154">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="59571-154">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="59571-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="59571-155">Response</span></span>
<span data-ttu-id="59571-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59571-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 201 Created

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/mailFolders('Inbox')/messages",
  "changeType":"created, updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```
## <a name="subscription-validation"></a><span data-ttu-id="59571-159">Проверка подписки</span><span class="sxs-lookup"><span data-stu-id="59571-159">Subscription validation</span></span>
<span data-ttu-id="59571-p106">Чтобы подписки по ошибке не отправляли уведомления на произвольные URL-адреса, у конечной точки уведомлений подписки должна быть возможность ответить на запрос проверки. Во время обработки запроса `POST` к конечной точке `/subscriptions` Microsoft Graph отправляет запрос `POST` обратно на адрес `notificationUrl` в следующей форме:</span><span class="sxs-lookup"><span data-stu-id="59571-p106">In order to to avoid mistaken subscriptions directing notifications to arbitrary URLs, the subscription notification endpoint must be capable of responding to a validation request. During processing of the `POST` to the `/subscriptions` endpoint, the Microsoft Graph will send a `POST` request back to your `notificationUrl` in the following form:</span></span> 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
<span data-ttu-id="59571-162">В течение 10 секунд конечная точка уведомления должна отправить код отклика 200 со значением `<token>` в теле отклика и типом контента `text/plain`, как показано ниже. В противном случае запрос на создание будет отменен.</span><span class="sxs-lookup"><span data-stu-id="59571-162">The notification endpoint must send a 200 response with the value of `<token>` as its body and a content type of `text/plain`, as shown below, within 10 seconds otherwise the creation request will be discarded.</span></span>
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
## <a name="notification-payload"></a><span data-ttu-id="59571-163">Полезные данные уведомлений</span><span class="sxs-lookup"><span data-stu-id="59571-163">Notification payload</span></span>
<span data-ttu-id="59571-p107">При изменении подписанного ресурса веб-перехватчик отправляет уведомление на URL-адрес уведомлений с приведенными ниже полезными данными.  В течение 30 секунд конечная точка уведомлений должна отправить код отклика 200 или 204 без тела отклика. В противном случае будут выполняться повторные попытки отправки уведомления с экспоненциально растущими интервалами.  Службы, у которых обработка запросов постоянно занимает не менее 30 секунд, можно отрегулировать, чтобы сократить отправляемый им набор уведомлений.</span><span class="sxs-lookup"><span data-stu-id="59571-p107">When the subscribed resource changes, the webhooks facility sends a notification to your notification URL with the following payload.  The notification endpoint must send a response of 200 or 204 with no response body within 30 seconds otherwise the notification attempt will be retried at exponentially increasing intervals.  Services that consistently take 30 seconds or more may be throttled and receive a sparser notification set.</span></span>

<span data-ttu-id="59571-167">В ответ на уведомления службы также могут возвращать код отклика 422. В этом случае подписка автоматически удаляется, в поток уведомлений останавливается.</span><span class="sxs-lookup"><span data-stu-id="59571-167">Services may also return a 422 response from a notification, in which case the subscription will be automatically deleted and the stream of notifications will come to a halt.</span></span>

<span data-ttu-id="59571-168">В зависимости от подписанного ресурса, в дополнительном поле resourceData могут быть представлены различные сведения.</span><span class="sxs-lookup"><span data-stu-id="59571-168">Depending on the subscribed resource, an additional resourceData field may provide additional information.</span></span>

```http
{
   "value":[
      {
         "subscriptionId":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
         "subscriptionExpirationDateTime":"2015-11-20T18:23:45.9356913Z",
         "clientState":"subscription-identifier",
         "changeType":"Created",
         "resource":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
         "resourceData":{
            "@odata.type":"#Microsoft.Graph.Message",
            "@odata.id":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
            "@odata.etag":"W/\"CQAAABYAAACoeN6SYXGLRrvRm+CYrrfQAACvvGdb\"",
            "Id":"AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA="
         }
      }
   ]
}
```
<span data-ttu-id="59571-p108">При получении уведомлений от подписок на диски поле resourceData содержит значение null, а для определения внесенных изменений необходимо вызвать API [delta](item_delta.md). Ниже представлен пример уведомления о диске.</span><span class="sxs-lookup"><span data-stu-id="59571-p108">When receiving notifications from Drive subscriptions the resourceData will be null and the [delta](item_delta.md) API should be called to determine the changes that have occured. Here is an example of a Drive notification:</span></span>
```http
{
  "subscriptionId": "aa269f87-2a92-4cff-a43e-2771878c3727",
  "clientState": "My client state",
  "changeType": "updated",
  "resource": "me/drive/root",
  "subscriptionExpirationDateTime": "2016-08-26T23:08:37.00+00:00",
  "resourceData": null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
