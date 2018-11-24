# <a name="create-subscription"></a><span data-ttu-id="c4694-101">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="c4694-101">Create subscription</span></span>

<span data-ttu-id="c4694-102">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c4694-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4694-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4694-103">Permissions</span></span>

<span data-ttu-id="c4694-p101">Создание подписки требует наличия области чтения для ресурса. Например, чтобы получать сообщения уведомлений, приложению необходимо разрешение `Mail.Read`. В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4694-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c4694-108">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="c4694-108">Resource type / Item</span></span>        | <span data-ttu-id="c4694-109">Разрешение</span><span class="sxs-lookup"><span data-stu-id="c4694-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="c4694-110">Contacts</span><span class="sxs-lookup"><span data-stu-id="c4694-110">Contacts</span></span>                    | <span data-ttu-id="c4694-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c4694-111">Contacts.Read</span></span>       |
| <span data-ttu-id="c4694-112">Беседы</span><span class="sxs-lookup"><span data-stu-id="c4694-112">Conversations</span></span>               | <span data-ttu-id="c4694-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4694-113">Group.Read.All</span></span>      |
| <span data-ttu-id="c4694-114">События</span><span class="sxs-lookup"><span data-stu-id="c4694-114">Events</span></span>                      | <span data-ttu-id="c4694-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c4694-115">Calendars.Read</span></span>      |
| <span data-ttu-id="c4694-116">Сообщения</span><span class="sxs-lookup"><span data-stu-id="c4694-116">Messages</span></span>                    | <span data-ttu-id="c4694-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c4694-117">Mail.Read</span></span>           |
| <span data-ttu-id="c4694-118">Groups</span><span class="sxs-lookup"><span data-stu-id="c4694-118">Groups</span></span>                      | <span data-ttu-id="c4694-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4694-119">Group.Read.All</span></span>      |
| <span data-ttu-id="c4694-120">Users</span><span class="sxs-lookup"><span data-stu-id="c4694-120">Users</span></span>                       | <span data-ttu-id="c4694-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4694-121">User.Read.All</span></span>       |
| <span data-ttu-id="c4694-122">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="c4694-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="c4694-123">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="c4694-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="c4694-124">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="c4694-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="c4694-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4694-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="c4694-126">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="c4694-126">Security alert</span></span>| <span data-ttu-id="c4694-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4694-127">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="c4694-128">**Примечание:** Конечная точка /v1.0 позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c4694-128">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="c4694-129">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c4694-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="c4694-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4694-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="c4694-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4694-131">Request headers</span></span>

| <span data-ttu-id="c4694-132">Имя</span><span class="sxs-lookup"><span data-stu-id="c4694-132">Name</span></span>       | <span data-ttu-id="c4694-133">Тип</span><span class="sxs-lookup"><span data-stu-id="c4694-133">Type</span></span> | <span data-ttu-id="c4694-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c4694-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c4694-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4694-135">Authorization</span></span>  | <span data-ttu-id="c4694-136">string</span><span class="sxs-lookup"><span data-stu-id="c4694-136">string</span></span>  | <span data-ttu-id="c4694-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4694-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c4694-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4694-139">Response</span></span>

<span data-ttu-id="c4694-140">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c4694-140">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4694-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c4694-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c4694-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4694-142">Request</span></span>

<span data-ttu-id="c4694-143">Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="c4694-143">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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

<span data-ttu-id="c4694-144">В тексте запроса укажите представление объекта [подписки](../resources/subscription.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="c4694-144">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="c4694-145">`clientState` Поле является необязательным.</span><span class="sxs-lookup"><span data-stu-id="c4694-145">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="c4694-146">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="c4694-146">Resources examples</span></span>

<span data-ttu-id="c4694-147">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="c4694-147">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="c4694-148">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="c4694-148">Resource type</span></span> | <span data-ttu-id="c4694-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4694-149">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="c4694-150">Почта</span><span class="sxs-lookup"><span data-stu-id="c4694-150">Mail</span></span>|<span data-ttu-id="c4694-151">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="c4694-151">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="c4694-152">me/messages</span><span class="sxs-lookup"><span data-stu-id="c4694-152">me/messages</span></span>|
|<span data-ttu-id="c4694-153">Контакты</span><span class="sxs-lookup"><span data-stu-id="c4694-153">Contacts</span></span>|<span data-ttu-id="c4694-154">me/contacts</span><span class="sxs-lookup"><span data-stu-id="c4694-154">me/contacts</span></span>|
|<span data-ttu-id="c4694-155">Календари</span><span class="sxs-lookup"><span data-stu-id="c4694-155">Calendars</span></span>|<span data-ttu-id="c4694-156">me/events</span><span class="sxs-lookup"><span data-stu-id="c4694-156">me/events</span></span>|
|<span data-ttu-id="c4694-157">Users</span><span class="sxs-lookup"><span data-stu-id="c4694-157">Users</span></span>|<span data-ttu-id="c4694-158">users</span><span class="sxs-lookup"><span data-stu-id="c4694-158">users</span></span>|
|<span data-ttu-id="c4694-159">Groups</span><span class="sxs-lookup"><span data-stu-id="c4694-159">Groups</span></span>|<span data-ttu-id="c4694-160">группы</span><span class="sxs-lookup"><span data-stu-id="c4694-160">groups</span></span>|
|<span data-ttu-id="c4694-161">Conversations</span><span class="sxs-lookup"><span data-stu-id="c4694-161">Conversations</span></span>|<span data-ttu-id="c4694-162">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="c4694-162">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="c4694-163">Drives</span><span class="sxs-lookup"><span data-stu-id="c4694-163">Drives</span></span>|<span data-ttu-id="c4694-164">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="c4694-164">me/drive/root</span></span>|
|<span data-ttu-id="c4694-165">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="c4694-165">Security alert</span></span>|<span data-ttu-id="c4694-166">Оповещение системы безопасности /? $filter = состояние eq «Создать»</span><span class="sxs-lookup"><span data-stu-id="c4694-166">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="c4694-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4694-167">Response</span></span>

<span data-ttu-id="c4694-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c4694-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="c4694-171">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="c4694-171">Notification endpoint validation</span></span>

<span data-ttu-id="c4694-172">Конечная точка уведомления подписки (указанного в `notificationUrl` свойство) должен быть способен отвечать на запрос проверки, как описано в [Настройка уведомлений для изменения в данные пользователя](../../../concepts/webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="c4694-172">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](../../../concepts/webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="c4694-173">Если не удается выполнить проверку, запрос на создание подписки возвращает ошибку 400 Ошибочный запрос.</span><span class="sxs-lookup"><span data-stu-id="c4694-173">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
