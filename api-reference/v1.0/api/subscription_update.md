# <a name="update-subscription"></a><span data-ttu-id="04a7c-101">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="04a7c-101">Update subscription</span></span>

<span data-ttu-id="04a7c-102">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="04a7c-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="04a7c-103">Срок действия подписок истекает по прошествии времени, которое зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="04a7c-103">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="04a7c-104">Чтобы не пропустить уведомления, приложение должно возобновить подписку заранее, до наступления даты истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="04a7c-104">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="04a7c-105">В разделе [подписка](../resources/subscription.md) можно ознакомиться с максимальным сроком действия подписки для каждого типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="04a7c-105">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="04a7c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04a7c-106">Permissions</span></span>

<span data-ttu-id="04a7c-p102">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04a7c-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="04a7c-109">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="04a7c-109">Resource type / Item</span></span>        | <span data-ttu-id="04a7c-110">Разрешение</span><span class="sxs-lookup"><span data-stu-id="04a7c-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="04a7c-111">Контакты</span><span class="sxs-lookup"><span data-stu-id="04a7c-111">Contacts</span></span>                    | <span data-ttu-id="04a7c-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="04a7c-112">Contacts.Read</span></span>       |
| <span data-ttu-id="04a7c-113">Беседы</span><span class="sxs-lookup"><span data-stu-id="04a7c-113">Conversations</span></span>               | <span data-ttu-id="04a7c-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04a7c-114">Group.Read.All</span></span>      |
| <span data-ttu-id="04a7c-115">События</span><span class="sxs-lookup"><span data-stu-id="04a7c-115">Events</span></span>                      | <span data-ttu-id="04a7c-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="04a7c-116">Calendars.Read</span></span>      |
| <span data-ttu-id="04a7c-117">Сообщения</span><span class="sxs-lookup"><span data-stu-id="04a7c-117">Messages</span></span>                    | <span data-ttu-id="04a7c-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="04a7c-118">Mail.Read</span></span>           |
| <span data-ttu-id="04a7c-119">Группы</span><span class="sxs-lookup"><span data-stu-id="04a7c-119">Groups</span></span>                      | <span data-ttu-id="04a7c-120">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04a7c-120">Group.Read.All</span></span>      |
| <span data-ttu-id="04a7c-121">Пользователи</span><span class="sxs-lookup"><span data-stu-id="04a7c-121">Users</span></span>                       | <span data-ttu-id="04a7c-122">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="04a7c-122">User.Read.All</span></span>       |
| <span data-ttu-id="04a7c-123">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="04a7c-123">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="04a7c-124">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="04a7c-124">Files.ReadWrite</span></span>     |
| <span data-ttu-id="04a7c-125">Диски (содержимое и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="04a7c-125">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="04a7c-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04a7c-126">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04a7c-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04a7c-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="04a7c-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04a7c-128">Request headers</span></span>

| <span data-ttu-id="04a7c-129">Имя</span><span class="sxs-lookup"><span data-stu-id="04a7c-129">Name</span></span>       | <span data-ttu-id="04a7c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="04a7c-130">Type</span></span> | <span data-ttu-id="04a7c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="04a7c-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04a7c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="04a7c-132">Authorization</span></span>  | <span data-ttu-id="04a7c-133">string (строка)</span><span class="sxs-lookup"><span data-stu-id="04a7c-133">string</span></span>  | <span data-ttu-id="04a7c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04a7c-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="04a7c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="04a7c-136">Response</span></span>

<span data-ttu-id="04a7c-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04a7c-137">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04a7c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="04a7c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="04a7c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="04a7c-139">Request</span></span>

<span data-ttu-id="04a7c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04a7c-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="04a7c-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="04a7c-141">Response</span></span>

<span data-ttu-id="04a7c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04a7c-142">Here is an example of the response.</span></span>
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
