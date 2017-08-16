# <a name="get-subscription"></a><span data-ttu-id="e0dbf-101">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="e0dbf-101">Get subscription</span></span>

<span data-ttu-id="e0dbf-102">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0dbf-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="e0dbf-103">Prerequisites</span></span>

<span data-ttu-id="e0dbf-104">В таблице ниже перечислены рекомендуемые разрешения, которые требуются для каждого ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="e0dbf-105">Тип ресурса / Элемент</span><span class="sxs-lookup"><span data-stu-id="e0dbf-105">Resource type / Item</span></span>        | <span data-ttu-id="e0dbf-106">Область</span><span class="sxs-lookup"><span data-stu-id="e0dbf-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="e0dbf-107">Контакты</span><span class="sxs-lookup"><span data-stu-id="e0dbf-107">Contacts</span></span>                    | <span data-ttu-id="e0dbf-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e0dbf-108">Contacts.Read</span></span>       |
| <span data-ttu-id="e0dbf-109">Беседы</span><span class="sxs-lookup"><span data-stu-id="e0dbf-109">Conversations</span></span>               | <span data-ttu-id="e0dbf-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0dbf-110">Group.Read.All</span></span>      |
| <span data-ttu-id="e0dbf-111">События</span><span class="sxs-lookup"><span data-stu-id="e0dbf-111">Events</span></span>                      | <span data-ttu-id="e0dbf-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e0dbf-112">Calendars.Read</span></span>      |
| <span data-ttu-id="e0dbf-113">Сообщения</span><span class="sxs-lookup"><span data-stu-id="e0dbf-113">Messages</span></span>                    | <span data-ttu-id="e0dbf-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e0dbf-114">Mail.Read</span></span>           |
| <span data-ttu-id="e0dbf-115">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="e0dbf-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="e0dbf-116">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="e0dbf-117">Диски (контент и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="e0dbf-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="e0dbf-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0dbf-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0dbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0dbf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0dbf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e0dbf-120">Optional query parameters</span></span>
<span data-ttu-id="e0dbf-121">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0dbf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0dbf-122">Request headers</span></span>
| <span data-ttu-id="e0dbf-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e0dbf-123">Name</span></span>       | <span data-ttu-id="e0dbf-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e0dbf-124">Type</span></span> | <span data-ttu-id="e0dbf-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e0dbf-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0dbf-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0dbf-126">Authorization</span></span>  | <span data-ttu-id="e0dbf-127">string</span><span class="sxs-lookup"><span data-stu-id="e0dbf-127">string</span></span>  | <span data-ttu-id="e0dbf-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0dbf-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0dbf-130">Request body</span></span>
<span data-ttu-id="e0dbf-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0dbf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0dbf-132">Response</span></span>

<span data-ttu-id="e0dbf-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0dbf-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e0dbf-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0dbf-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0dbf-135">Request</span></span>
<span data-ttu-id="e0dbf-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="e0dbf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0dbf-137">Response</span></span>
<span data-ttu-id="e0dbf-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e0dbf-138">Here is an example of the response.</span></span>
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
