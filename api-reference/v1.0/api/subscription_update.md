# <a name="update-subscription"></a><span data-ttu-id="c5203-101">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="c5203-101">Update subscription</span></span>

<span data-ttu-id="c5203-102">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="c5203-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="c5203-p101">Даты окончания срока действия для подписок на ресурсы задаются отдельными типами ресурсов.  Чтобы не пропускать уведомления, следует продлевать подписки задолго до конечной даты.  Отдельные даты окончания срока действия представлены в описании ресурса [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="c5203-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5203-106">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="c5203-106">Prerequisites</span></span>

<span data-ttu-id="c5203-107">В таблице ниже перечислены рекомендуемые разрешения, которые требуются для каждого ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5203-107">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="c5203-108">Тип ресурса / Элемент</span><span class="sxs-lookup"><span data-stu-id="c5203-108">Resource type / Item</span></span>        | <span data-ttu-id="c5203-109">Область</span><span class="sxs-lookup"><span data-stu-id="c5203-109">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="c5203-110">Контакты</span><span class="sxs-lookup"><span data-stu-id="c5203-110">Contacts</span></span>                    | <span data-ttu-id="c5203-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c5203-111">Contacts.Read</span></span>       |
| <span data-ttu-id="c5203-112">Беседы</span><span class="sxs-lookup"><span data-stu-id="c5203-112">Conversations</span></span>               | <span data-ttu-id="c5203-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5203-113">Group.Read.All</span></span>      |
| <span data-ttu-id="c5203-114">События</span><span class="sxs-lookup"><span data-stu-id="c5203-114">Events</span></span>                      | <span data-ttu-id="c5203-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c5203-115">Calendars.Read</span></span>      |
| <span data-ttu-id="c5203-116">Сообщения</span><span class="sxs-lookup"><span data-stu-id="c5203-116">Messages</span></span>                    | <span data-ttu-id="c5203-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c5203-117">Mail.Read</span></span>           |
| <span data-ttu-id="c5203-118">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="c5203-118">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="c5203-119">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="c5203-119">Files.ReadWrite</span></span>     |
| <span data-ttu-id="c5203-120">Диски (контент и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="c5203-120">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="c5203-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5203-121">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5203-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5203-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="c5203-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5203-123">Request headers</span></span>
| <span data-ttu-id="c5203-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c5203-124">Name</span></span>       | <span data-ttu-id="c5203-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c5203-125">Type</span></span> | <span data-ttu-id="c5203-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c5203-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5203-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5203-127">Authorization</span></span>  | <span data-ttu-id="c5203-128">string</span><span class="sxs-lookup"><span data-stu-id="c5203-128">string</span></span>  | <span data-ttu-id="c5203-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5203-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c5203-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5203-131">Response</span></span>

<span data-ttu-id="c5203-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5203-132">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5203-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c5203-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5203-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5203-134">Request</span></span>
<span data-ttu-id="c5203-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5203-135">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c5203-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5203-136">Response</span></span>
<span data-ttu-id="c5203-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c5203-137">Here is an example of the response.</span></span>
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
