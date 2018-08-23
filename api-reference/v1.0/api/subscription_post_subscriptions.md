# <a name="create-subscription"></a><span data-ttu-id="be32e-101">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="be32e-101">Create subscription</span></span>

<span data-ttu-id="be32e-102">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="be32e-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="be32e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be32e-103">Permissions</span></span>

<span data-ttu-id="be32e-p101">Создание подписки требует наличия области чтения для ресурса. Например, чтобы получать сообщения уведомлений, приложению необходимо разрешение `Mail.Read`. В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="be32e-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="be32e-108">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="be32e-108">Resource type / Item</span></span>        | <span data-ttu-id="be32e-109">Разрешение</span><span class="sxs-lookup"><span data-stu-id="be32e-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="be32e-110">Контакты</span><span class="sxs-lookup"><span data-stu-id="be32e-110">Contacts</span></span>                    | <span data-ttu-id="be32e-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="be32e-111">Contacts.Read</span></span>       |
| <span data-ttu-id="be32e-112">Разговоры</span><span class="sxs-lookup"><span data-stu-id="be32e-112">Conversations</span></span>               | <span data-ttu-id="be32e-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="be32e-113">Group.Read.All</span></span>      |
| <span data-ttu-id="be32e-114">События</span><span class="sxs-lookup"><span data-stu-id="be32e-114">Events</span></span>                      | <span data-ttu-id="be32e-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="be32e-115">Calendars.Read</span></span>      |
| <span data-ttu-id="be32e-116">Сообщения</span><span class="sxs-lookup"><span data-stu-id="be32e-116">Messages</span></span>                    | <span data-ttu-id="be32e-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="be32e-117">Mail.Read</span></span>           |
| <span data-ttu-id="be32e-118">Группы</span><span class="sxs-lookup"><span data-stu-id="be32e-118">Groups</span></span>                      | <span data-ttu-id="be32e-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="be32e-119">Group.Read.All</span></span>      |
| <span data-ttu-id="be32e-120">Пользователи</span><span class="sxs-lookup"><span data-stu-id="be32e-120">Users</span></span>                       | <span data-ttu-id="be32e-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="be32e-121">User.Read.All</span></span>       |
| <span data-ttu-id="be32e-122">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="be32e-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="be32e-123">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="be32e-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="be32e-124">Диски (содержимое и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="be32e-124">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="be32e-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be32e-125">Files.ReadWrite.All</span></span> |

 > <span data-ttu-id="be32e-126">**Примечание:** Конечная точка /v1.0 позволяет использовать разрешения для приложений для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="be32e-126">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="be32e-127">Разговоры в группе и в корневом диске OneDrive не поддерживаются разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="be32e-127">Note: The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="be32e-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be32e-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="be32e-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be32e-129">Request headers</span></span>

| <span data-ttu-id="be32e-130">Имя</span><span class="sxs-lookup"><span data-stu-id="be32e-130">Name</span></span>       | <span data-ttu-id="be32e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="be32e-131">Type</span></span> | <span data-ttu-id="be32e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="be32e-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be32e-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be32e-133">Authorization</span></span>  | <span data-ttu-id="be32e-134">строка</span><span class="sxs-lookup"><span data-stu-id="be32e-134">string</span></span>  | <span data-ttu-id="be32e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be32e-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="be32e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="be32e-137">Response</span></span>

<span data-ttu-id="be32e-138">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be32e-138">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be32e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="be32e-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="be32e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="be32e-140">Request</span></span>

<span data-ttu-id="be32e-141">Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="be32e-141">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="be32e-142">В теле запроса укажите JSON-представление объекта [подписки](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="be32e-142">In the request body, supply a JSON representation of the [Contact](../resources/subscription.md) object.</span></span>
<span data-ttu-id="be32e-143">Поле `clientState` является необязательным.</span><span class="sxs-lookup"><span data-stu-id="be32e-143">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="be32e-144">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="be32e-144">Resources examples</span></span>

<span data-ttu-id="be32e-145">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="be32e-145">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="be32e-146">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="be32e-146">Resource type</span></span> | <span data-ttu-id="be32e-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="be32e-147">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="be32e-148">Почта</span><span class="sxs-lookup"><span data-stu-id="be32e-148">Mail</span></span>|<span data-ttu-id="be32e-149">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="be32e-149">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="be32e-150">me/messages</span><span class="sxs-lookup"><span data-stu-id="be32e-150">me/messages</span></span>|
|<span data-ttu-id="be32e-151">Контакты</span><span class="sxs-lookup"><span data-stu-id="be32e-151">Contacts</span></span>|<span data-ttu-id="be32e-152">me/contacts</span><span class="sxs-lookup"><span data-stu-id="be32e-152">me/contacts</span></span>|
|<span data-ttu-id="be32e-153">Календари</span><span class="sxs-lookup"><span data-stu-id="be32e-153">Calendars</span></span>|<span data-ttu-id="be32e-154">me/events</span><span class="sxs-lookup"><span data-stu-id="be32e-154">me/events</span></span>|
|<span data-ttu-id="be32e-155">Пользователи</span><span class="sxs-lookup"><span data-stu-id="be32e-155">Users</span></span>|<span data-ttu-id="be32e-156">users</span><span class="sxs-lookup"><span data-stu-id="be32e-156">users</span></span>|
|<span data-ttu-id="be32e-157">Группы</span><span class="sxs-lookup"><span data-stu-id="be32e-157">Groups</span></span>|<span data-ttu-id="be32e-158">groups</span><span class="sxs-lookup"><span data-stu-id="be32e-158">groups</span></span>|
|<span data-ttu-id="be32e-159">Разговоры</span><span class="sxs-lookup"><span data-stu-id="be32e-159">Conversations</span></span>|<span data-ttu-id="be32e-160">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="be32e-160">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="be32e-161">Диски</span><span class="sxs-lookup"><span data-stu-id="be32e-161">Drives</span></span>|<span data-ttu-id="be32e-162">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="be32e-162">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="be32e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="be32e-163">Response</span></span>

<span data-ttu-id="be32e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="be32e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="be32e-167">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="be32e-167">Notification endpoint validation</span></span>

<span data-ttu-id="be32e-168">Конечная точка уведомления подписки (указанного в свойстве`notificationUrl`) должна быть способна отвечать на запрос проверки, как описано в [Настройка уведомлений для изменения данных пользователя](../../../concepts/webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="be32e-168">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](../../../concepts/webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="be32e-169">Если не удается выполнить проверку, запрос на создание подписки возвращает ошибку "400— Ошибочный запрос".</span><span class="sxs-lookup"><span data-stu-id="be32e-169">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
