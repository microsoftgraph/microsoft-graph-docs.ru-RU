# <a name="delete-subscription"></a><span data-ttu-id="ec088-101">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="ec088-101">Delete subscription</span></span>

<span data-ttu-id="ec088-102">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="ec088-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec088-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec088-103">Permissions</span></span>

<span data-ttu-id="ec088-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec088-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ec088-106">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="ec088-106">Resource type / Item</span></span>        | <span data-ttu-id="ec088-107">Разрешение</span><span class="sxs-lookup"><span data-stu-id="ec088-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="ec088-108">Contacts</span><span class="sxs-lookup"><span data-stu-id="ec088-108">Contacts</span></span>                    | <span data-ttu-id="ec088-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ec088-109">Contacts.Read</span></span>       |
| <span data-ttu-id="ec088-110">Conversations</span><span class="sxs-lookup"><span data-stu-id="ec088-110">Conversations</span></span>               | <span data-ttu-id="ec088-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec088-111">Group.Read.All</span></span>      |
| <span data-ttu-id="ec088-112">Events</span><span class="sxs-lookup"><span data-stu-id="ec088-112">Events</span></span>                      | <span data-ttu-id="ec088-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ec088-113">Calendars.Read</span></span>      |
| <span data-ttu-id="ec088-114">Messages</span><span class="sxs-lookup"><span data-stu-id="ec088-114">Messages</span></span>                    | <span data-ttu-id="ec088-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ec088-115">Mail.Read</span></span>           |
| <span data-ttu-id="ec088-116">Drive (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="ec088-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="ec088-117">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="ec088-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="ec088-118">Drives (контент и библиотеки документов в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="ec088-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="ec088-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec088-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec088-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec088-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="ec088-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec088-121">Request headers</span></span>
| <span data-ttu-id="ec088-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ec088-122">Name</span></span>       | <span data-ttu-id="ec088-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ec088-123">Type</span></span> | <span data-ttu-id="ec088-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ec088-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ec088-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec088-125">Authorization</span></span>  | <span data-ttu-id="ec088-126">string</span><span class="sxs-lookup"><span data-stu-id="ec088-126">string</span></span>  | <span data-ttu-id="ec088-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec088-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec088-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec088-129">Request body</span></span>
<span data-ttu-id="ec088-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec088-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec088-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec088-131">Response</span></span>

<span data-ttu-id="ec088-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ec088-132">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="ec088-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ec088-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec088-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec088-134">Request</span></span>
<span data-ttu-id="ec088-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec088-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="ec088-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec088-136">Response</span></span>
<span data-ttu-id="ec088-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ec088-137">Here is an example of the response.</span></span>
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
