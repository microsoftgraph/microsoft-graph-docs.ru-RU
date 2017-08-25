# <a name="get-subscription"></a><span data-ttu-id="bfbad-101">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="bfbad-101">Get subscription</span></span>

<span data-ttu-id="bfbad-102">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="bfbad-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfbad-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfbad-103">Permissions</span></span>

<span data-ttu-id="bfbad-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bfbad-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="bfbad-106">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="bfbad-106">Resource type / Item</span></span>        | <span data-ttu-id="bfbad-107">Разрешение</span><span class="sxs-lookup"><span data-stu-id="bfbad-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="bfbad-108">Contacts</span><span class="sxs-lookup"><span data-stu-id="bfbad-108">Contacts</span></span>                    | <span data-ttu-id="bfbad-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bfbad-109">Contacts.Read</span></span>       |
| <span data-ttu-id="bfbad-110">Беседы</span><span class="sxs-lookup"><span data-stu-id="bfbad-110">Conversations</span></span>               | <span data-ttu-id="bfbad-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfbad-111">Group.Read.All</span></span>      |
| <span data-ttu-id="bfbad-112">События</span><span class="sxs-lookup"><span data-stu-id="bfbad-112">Events</span></span>                      | <span data-ttu-id="bfbad-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bfbad-113">Calendars.Read</span></span>      |
| <span data-ttu-id="bfbad-114">Сообщения</span><span class="sxs-lookup"><span data-stu-id="bfbad-114">Messages</span></span>                    | <span data-ttu-id="bfbad-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bfbad-115">Mail.Read</span></span>           |
| <span data-ttu-id="bfbad-116">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="bfbad-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="bfbad-117">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="bfbad-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="bfbad-118">Диски (контент и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="bfbad-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="bfbad-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfbad-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfbad-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfbad-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfbad-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bfbad-121">Optional query parameters</span></span>
<span data-ttu-id="bfbad-122">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bfbad-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfbad-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfbad-123">Request headers</span></span>
| <span data-ttu-id="bfbad-124">Имя</span><span class="sxs-lookup"><span data-stu-id="bfbad-124">Name</span></span>       | <span data-ttu-id="bfbad-125">Тип</span><span class="sxs-lookup"><span data-stu-id="bfbad-125">Type</span></span> | <span data-ttu-id="bfbad-126">Описание</span><span class="sxs-lookup"><span data-stu-id="bfbad-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bfbad-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfbad-127">Authorization</span></span>  | <span data-ttu-id="bfbad-128">string</span><span class="sxs-lookup"><span data-stu-id="bfbad-128">string</span></span>  | <span data-ttu-id="bfbad-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfbad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfbad-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfbad-131">Request body</span></span>
<span data-ttu-id="bfbad-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfbad-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfbad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfbad-133">Response</span></span>

<span data-ttu-id="bfbad-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfbad-134">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfbad-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bfbad-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfbad-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfbad-136">Request</span></span>
<span data-ttu-id="bfbad-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfbad-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="bfbad-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfbad-138">Response</span></span>
<span data-ttu-id="bfbad-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bfbad-139">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
