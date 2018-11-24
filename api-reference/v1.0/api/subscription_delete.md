# <a name="delete-subscription"></a><span data-ttu-id="1877c-101">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="1877c-101">Delete subscription</span></span>

<span data-ttu-id="1877c-102">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="1877c-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="1877c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1877c-103">Permissions</span></span>

<span data-ttu-id="1877c-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1877c-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="1877c-106">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="1877c-106">Resource type / Item</span></span>        | <span data-ttu-id="1877c-107">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1877c-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="1877c-108">Contacts</span><span class="sxs-lookup"><span data-stu-id="1877c-108">Contacts</span></span>                    | <span data-ttu-id="1877c-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1877c-109">Contacts.Read</span></span>       |
| <span data-ttu-id="1877c-110">Беседы</span><span class="sxs-lookup"><span data-stu-id="1877c-110">Conversations</span></span>               | <span data-ttu-id="1877c-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1877c-111">Group.Read.All</span></span>      |
| <span data-ttu-id="1877c-112">События</span><span class="sxs-lookup"><span data-stu-id="1877c-112">Events</span></span>                      | <span data-ttu-id="1877c-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1877c-113">Calendars.Read</span></span>      |
| <span data-ttu-id="1877c-114">Сообщения</span><span class="sxs-lookup"><span data-stu-id="1877c-114">Messages</span></span>                    | <span data-ttu-id="1877c-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1877c-115">Mail.Read</span></span>           |
| <span data-ttu-id="1877c-116">Groups</span><span class="sxs-lookup"><span data-stu-id="1877c-116">Groups</span></span>                      | <span data-ttu-id="1877c-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1877c-117">Group.Read.All</span></span>      |
| <span data-ttu-id="1877c-118">Users</span><span class="sxs-lookup"><span data-stu-id="1877c-118">Users</span></span>                       | <span data-ttu-id="1877c-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1877c-119">User.Read.All</span></span>       |
| <span data-ttu-id="1877c-120">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="1877c-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="1877c-121">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="1877c-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="1877c-122">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="1877c-122">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="1877c-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1877c-123">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="1877c-124">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="1877c-124">Security alert</span></span>| <span data-ttu-id="1877c-125">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1877c-125">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1877c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1877c-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1877c-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1877c-127">Request headers</span></span>

| <span data-ttu-id="1877c-128">Имя</span><span class="sxs-lookup"><span data-stu-id="1877c-128">Name</span></span>       | <span data-ttu-id="1877c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1877c-129">Type</span></span> | <span data-ttu-id="1877c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1877c-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1877c-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="1877c-131">Authorization</span></span>  | <span data-ttu-id="1877c-132">string</span><span class="sxs-lookup"><span data-stu-id="1877c-132">string</span></span>  | <span data-ttu-id="1877c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1877c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1877c-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1877c-135">Request body</span></span>

<span data-ttu-id="1877c-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1877c-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1877c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="1877c-137">Response</span></span>

<span data-ttu-id="1877c-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1877c-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1877c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1877c-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1877c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1877c-140">Request</span></span>

<span data-ttu-id="1877c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1877c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="1877c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="1877c-142">Response</span></span>

<span data-ttu-id="1877c-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1877c-143">Here is an example of the response.</span></span>
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
