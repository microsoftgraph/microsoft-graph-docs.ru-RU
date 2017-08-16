# <a name="delete-subscription"></a><span data-ttu-id="13384-101">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="13384-101">Delete subscription</span></span>

<span data-ttu-id="13384-102">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="13384-102">Delete a subscription.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13384-103">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="13384-103">Prerequisites</span></span>

<span data-ttu-id="13384-104">В таблице ниже перечислены рекомендуемые разрешения, которые требуются для каждого ресурса.</span><span class="sxs-lookup"><span data-stu-id="13384-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="13384-105">Тип ресурса / Элемент</span><span class="sxs-lookup"><span data-stu-id="13384-105">Resource type / Item</span></span>        | <span data-ttu-id="13384-106">Область</span><span class="sxs-lookup"><span data-stu-id="13384-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="13384-107">Контакты</span><span class="sxs-lookup"><span data-stu-id="13384-107">Contacts</span></span>                    | <span data-ttu-id="13384-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="13384-108">Contacts.Read</span></span>       |
| <span data-ttu-id="13384-109">Беседы</span><span class="sxs-lookup"><span data-stu-id="13384-109">Conversations</span></span>               | <span data-ttu-id="13384-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="13384-110">Group.Read.All</span></span>      |
| <span data-ttu-id="13384-111">События</span><span class="sxs-lookup"><span data-stu-id="13384-111">Events</span></span>                      | <span data-ttu-id="13384-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="13384-112">Calendars.Read</span></span>      |
| <span data-ttu-id="13384-113">Сообщения</span><span class="sxs-lookup"><span data-stu-id="13384-113">Messages</span></span>                    | <span data-ttu-id="13384-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13384-114">Mail.Read</span></span>           |
| <span data-ttu-id="13384-115">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="13384-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="13384-116">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="13384-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="13384-117">Диски (контент и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="13384-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="13384-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13384-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13384-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13384-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="13384-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13384-120">Request headers</span></span>
| <span data-ttu-id="13384-121">Имя</span><span class="sxs-lookup"><span data-stu-id="13384-121">Name</span></span>       | <span data-ttu-id="13384-122">Тип</span><span class="sxs-lookup"><span data-stu-id="13384-122">Type</span></span> | <span data-ttu-id="13384-123">Описание</span><span class="sxs-lookup"><span data-stu-id="13384-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="13384-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="13384-124">Authorization</span></span>  | <span data-ttu-id="13384-125">string</span><span class="sxs-lookup"><span data-stu-id="13384-125">string</span></span>  | <span data-ttu-id="13384-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13384-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13384-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13384-128">Request body</span></span>
<span data-ttu-id="13384-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13384-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13384-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="13384-130">Response</span></span>

<span data-ttu-id="13384-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13384-131">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="13384-132">Пример</span><span class="sxs-lookup"><span data-stu-id="13384-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13384-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="13384-133">Request</span></span>
<span data-ttu-id="13384-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13384-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="13384-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="13384-135">Response</span></span>
<span data-ttu-id="13384-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="13384-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
