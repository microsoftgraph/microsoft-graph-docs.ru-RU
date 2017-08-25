# <a name="update-subscription"></a><span data-ttu-id="18893-101">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="18893-101">Update subscription</span></span>

<span data-ttu-id="18893-102">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="18893-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="18893-p101">Даты окончания срока действия для подписок на ресурсы задаются отдельными типами ресурсов.  Чтобы не пропускать уведомления, следует продлевать подписки задолго до конечной даты.  Отдельные даты окончания срока действия представлены в описании ресурса [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="18893-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="permissions"></a><span data-ttu-id="18893-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18893-106">Permissions</span></span>

<span data-ttu-id="18893-p102">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="18893-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="18893-109">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="18893-109">Resource type / Item</span></span>        | <span data-ttu-id="18893-110">Разрешение</span><span class="sxs-lookup"><span data-stu-id="18893-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="18893-111">Contacts</span><span class="sxs-lookup"><span data-stu-id="18893-111">Contacts</span></span>                    | <span data-ttu-id="18893-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="18893-112">Contacts.Read</span></span>       |
| <span data-ttu-id="18893-113">Беседы</span><span class="sxs-lookup"><span data-stu-id="18893-113">Conversations</span></span>               | <span data-ttu-id="18893-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="18893-114">Group.Read.All</span></span>      |
| <span data-ttu-id="18893-115">События</span><span class="sxs-lookup"><span data-stu-id="18893-115">Events</span></span>                      | <span data-ttu-id="18893-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="18893-116">Calendars.Read</span></span>      |
| <span data-ttu-id="18893-117">Сообщения</span><span class="sxs-lookup"><span data-stu-id="18893-117">Messages</span></span>                    | <span data-ttu-id="18893-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="18893-118">Mail.Read</span></span>           |
| <span data-ttu-id="18893-119">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="18893-119">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="18893-120">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="18893-120">Files.ReadWrite</span></span>     |
| <span data-ttu-id="18893-121">Диски (контент и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="18893-121">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="18893-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18893-122">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18893-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18893-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="18893-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18893-124">Request headers</span></span>
| <span data-ttu-id="18893-125">Имя</span><span class="sxs-lookup"><span data-stu-id="18893-125">Name</span></span>       | <span data-ttu-id="18893-126">Тип</span><span class="sxs-lookup"><span data-stu-id="18893-126">Type</span></span> | <span data-ttu-id="18893-127">Описание</span><span class="sxs-lookup"><span data-stu-id="18893-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18893-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="18893-128">Authorization</span></span>  | <span data-ttu-id="18893-129">string</span><span class="sxs-lookup"><span data-stu-id="18893-129">string</span></span>  | <span data-ttu-id="18893-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18893-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="18893-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="18893-132">Response</span></span>

<span data-ttu-id="18893-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18893-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18893-134">Пример</span><span class="sxs-lookup"><span data-stu-id="18893-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18893-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="18893-135">Request</span></span>
<span data-ttu-id="18893-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18893-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="18893-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="18893-137">Response</span></span>
<span data-ttu-id="18893-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18893-138">Here is an example of the response.</span></span>
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
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
