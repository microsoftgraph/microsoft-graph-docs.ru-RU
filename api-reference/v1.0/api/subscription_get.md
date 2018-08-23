# <a name="get-subscription"></a><span data-ttu-id="121f3-101">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="121f3-101">Get subscription</span></span>

<span data-ttu-id="121f3-102">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="121f3-102">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="121f3-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="121f3-103">Permissions</span></span>

<span data-ttu-id="121f3-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="121f3-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="121f3-106">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="121f3-106">Resource type / Item</span></span>        | <span data-ttu-id="121f3-107">Разрешение</span><span class="sxs-lookup"><span data-stu-id="121f3-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="121f3-108">Контакты</span><span class="sxs-lookup"><span data-stu-id="121f3-108">Contacts</span></span>                    | <span data-ttu-id="121f3-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="121f3-109">Contacts.Read</span></span>       |
| <span data-ttu-id="121f3-110">Разговоры</span><span class="sxs-lookup"><span data-stu-id="121f3-110">Conversations</span></span>               | <span data-ttu-id="121f3-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="121f3-111">Group.Read.All</span></span>      |
| <span data-ttu-id="121f3-112">События</span><span class="sxs-lookup"><span data-stu-id="121f3-112">Events</span></span>                      | <span data-ttu-id="121f3-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="121f3-113">Calendars.Read</span></span>      |
| <span data-ttu-id="121f3-114">Сообщения</span><span class="sxs-lookup"><span data-stu-id="121f3-114">Messages</span></span>                    | <span data-ttu-id="121f3-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="121f3-115">Mail.Read</span></span>           |
| <span data-ttu-id="121f3-116">Группы</span><span class="sxs-lookup"><span data-stu-id="121f3-116">Groups</span></span>                      | <span data-ttu-id="121f3-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="121f3-117">Group.Read.All</span></span>      |
| <span data-ttu-id="121f3-118">Пользователи</span><span class="sxs-lookup"><span data-stu-id="121f3-118">Users</span></span>                       | <span data-ttu-id="121f3-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="121f3-119">User.Read.All</span></span>       |
| <span data-ttu-id="121f3-120">Диск (пользователя OneDrive)</span><span class="sxs-lookup"><span data-stu-id="121f3-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="121f3-121">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="121f3-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="121f3-122">Диски (содержимое и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="121f3-122">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="121f3-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="121f3-123">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="121f3-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="121f3-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="121f3-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="121f3-125">Optional query parameters</span></span>

<span data-ttu-id="121f3-126">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="121f3-126">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="121f3-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="121f3-127">Request headers</span></span>

| <span data-ttu-id="121f3-128">Имя</span><span class="sxs-lookup"><span data-stu-id="121f3-128">Name</span></span>       | <span data-ttu-id="121f3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="121f3-129">Type</span></span> | <span data-ttu-id="121f3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="121f3-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="121f3-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="121f3-131">Authorization</span></span>  | <span data-ttu-id="121f3-132">строка</span><span class="sxs-lookup"><span data-stu-id="121f3-132">string</span></span>  | <span data-ttu-id="121f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="121f3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="121f3-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="121f3-135">Request body</span></span>

<span data-ttu-id="121f3-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="121f3-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="121f3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="121f3-137">Response</span></span>

<span data-ttu-id="121f3-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="121f3-138">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="121f3-139">Пример</span><span class="sxs-lookup"><span data-stu-id="121f3-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="121f3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="121f3-140">Request</span></span>

<span data-ttu-id="121f3-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="121f3-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="121f3-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="121f3-142">Response</span></span>

<span data-ttu-id="121f3-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="121f3-143">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
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
