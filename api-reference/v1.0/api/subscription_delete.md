# <a name="delete-subscription"></a><span data-ttu-id="8efcd-101">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="8efcd-101">Delete subscription</span></span>

<span data-ttu-id="8efcd-102">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="8efcd-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8efcd-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8efcd-103">Permissions</span></span>

<span data-ttu-id="8efcd-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8efcd-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="8efcd-106">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="8efcd-106">Resource type / Item</span></span>        | <span data-ttu-id="8efcd-107">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8efcd-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8efcd-108">Контакты</span><span class="sxs-lookup"><span data-stu-id="8efcd-108">Contacts</span></span>                    | <span data-ttu-id="8efcd-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8efcd-109">Contacts.Read</span></span>       |
| <span data-ttu-id="8efcd-110">Разговоры</span><span class="sxs-lookup"><span data-stu-id="8efcd-110">Conversations</span></span>               | <span data-ttu-id="8efcd-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8efcd-111">Group.Read.All</span></span>      |
| <span data-ttu-id="8efcd-112">События</span><span class="sxs-lookup"><span data-stu-id="8efcd-112">Events</span></span>                      | <span data-ttu-id="8efcd-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8efcd-113">Calendars.Read</span></span>      |
| <span data-ttu-id="8efcd-114">Сообщения</span><span class="sxs-lookup"><span data-stu-id="8efcd-114">Messages</span></span>                    | <span data-ttu-id="8efcd-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8efcd-115">Mail.Read</span></span>           |
| <span data-ttu-id="8efcd-116">Группы</span><span class="sxs-lookup"><span data-stu-id="8efcd-116">Groups</span></span>                      | <span data-ttu-id="8efcd-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8efcd-117">Group.Read.All</span></span>      |
| <span data-ttu-id="8efcd-118">Пользователи</span><span class="sxs-lookup"><span data-stu-id="8efcd-118">Users</span></span>                       | <span data-ttu-id="8efcd-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8efcd-119">User.Read.All</span></span>       |
| <span data-ttu-id="8efcd-120">Диск (пользователя OneDrive)</span><span class="sxs-lookup"><span data-stu-id="8efcd-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8efcd-121">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="8efcd-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8efcd-122">Диски (содержимое и диски в SharePoint, к которым предоставлен общий доступ)</span><span class="sxs-lookup"><span data-stu-id="8efcd-122">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="8efcd-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8efcd-123">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8efcd-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8efcd-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8efcd-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8efcd-125">Request headers</span></span>

| <span data-ttu-id="8efcd-126">Имя</span><span class="sxs-lookup"><span data-stu-id="8efcd-126">Name</span></span>       | <span data-ttu-id="8efcd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8efcd-127">Type</span></span> | <span data-ttu-id="8efcd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8efcd-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8efcd-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8efcd-129">Authorization</span></span>  | <span data-ttu-id="8efcd-130">строка</span><span class="sxs-lookup"><span data-stu-id="8efcd-130">string</span></span>  | <span data-ttu-id="8efcd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8efcd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8efcd-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8efcd-133">Request body</span></span>

<span data-ttu-id="8efcd-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8efcd-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8efcd-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8efcd-135">Response</span></span>

<span data-ttu-id="8efcd-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8efcd-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8efcd-137">Пример</span><span class="sxs-lookup"><span data-stu-id="8efcd-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8efcd-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8efcd-138">Request</span></span>

<span data-ttu-id="8efcd-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8efcd-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8efcd-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="8efcd-140">Response</span></span>

<span data-ttu-id="8efcd-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8efcd-141">Here is an example of the response.</span></span>
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
