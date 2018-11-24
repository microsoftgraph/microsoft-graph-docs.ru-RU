# <a name="update-subscription"></a><span data-ttu-id="64c5b-101">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="64c5b-101">Update subscription</span></span>

<span data-ttu-id="64c5b-102">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="64c5b-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="64c5b-103">Срок действия подписок после продолжительность времени, зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="64c5b-103">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="64c5b-104">Во избежание отсутствует уведомлений, приложение следует обновлять его подписки еще до которых истек срок действия.</span><span class="sxs-lookup"><span data-stu-id="64c5b-104">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="64c5b-105">В разделе [подписки](../resources/subscription.md) для Максимальная длина подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="64c5b-105">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="64c5b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64c5b-106">Permissions</span></span>

<span data-ttu-id="64c5b-p102">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64c5b-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="64c5b-109">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="64c5b-109">Resource type / Item</span></span>        | <span data-ttu-id="64c5b-110">Разрешение</span><span class="sxs-lookup"><span data-stu-id="64c5b-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="64c5b-111">Contacts</span><span class="sxs-lookup"><span data-stu-id="64c5b-111">Contacts</span></span>                    | <span data-ttu-id="64c5b-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="64c5b-112">Contacts.Read</span></span>       |
| <span data-ttu-id="64c5b-113">Беседы</span><span class="sxs-lookup"><span data-stu-id="64c5b-113">Conversations</span></span>               | <span data-ttu-id="64c5b-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="64c5b-114">Group.Read.All</span></span>      |
| <span data-ttu-id="64c5b-115">События</span><span class="sxs-lookup"><span data-stu-id="64c5b-115">Events</span></span>                      | <span data-ttu-id="64c5b-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="64c5b-116">Calendars.Read</span></span>      |
| <span data-ttu-id="64c5b-117">Сообщения</span><span class="sxs-lookup"><span data-stu-id="64c5b-117">Messages</span></span>                    | <span data-ttu-id="64c5b-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="64c5b-118">Mail.Read</span></span>           |
| <span data-ttu-id="64c5b-119">Groups</span><span class="sxs-lookup"><span data-stu-id="64c5b-119">Groups</span></span>                      | <span data-ttu-id="64c5b-120">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="64c5b-120">Group.Read.All</span></span>      |
| <span data-ttu-id="64c5b-121">Users</span><span class="sxs-lookup"><span data-stu-id="64c5b-121">Users</span></span>                       | <span data-ttu-id="64c5b-122">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="64c5b-122">User.Read.All</span></span>       |
| <span data-ttu-id="64c5b-123">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="64c5b-123">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="64c5b-124">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="64c5b-124">Files.ReadWrite</span></span>     |
| <span data-ttu-id="64c5b-125">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="64c5b-125">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="64c5b-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c5b-126">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="64c5b-127">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="64c5b-127">Security alert</span></span>| <span data-ttu-id="64c5b-128">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c5b-128">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64c5b-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64c5b-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="64c5b-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64c5b-130">Request headers</span></span>

| <span data-ttu-id="64c5b-131">Имя</span><span class="sxs-lookup"><span data-stu-id="64c5b-131">Name</span></span>       | <span data-ttu-id="64c5b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="64c5b-132">Type</span></span> | <span data-ttu-id="64c5b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="64c5b-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="64c5b-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="64c5b-134">Authorization</span></span>  | <span data-ttu-id="64c5b-135">string</span><span class="sxs-lookup"><span data-stu-id="64c5b-135">string</span></span>  | <span data-ttu-id="64c5b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64c5b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="64c5b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c5b-138">Response</span></span>

<span data-ttu-id="64c5b-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64c5b-139">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64c5b-140">Пример</span><span class="sxs-lookup"><span data-stu-id="64c5b-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64c5b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="64c5b-141">Request</span></span>

<span data-ttu-id="64c5b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64c5b-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="64c5b-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="64c5b-143">Response</span></span>

<span data-ttu-id="64c5b-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64c5b-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
