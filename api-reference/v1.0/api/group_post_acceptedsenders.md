# <a name="create-acceptedsender"></a><span data-ttu-id="55962-101">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="55962-101">Create acceptedSender</span></span>

<span data-ttu-id="55962-102">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="55962-102">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="55962-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="55962-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55962-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="55962-106">Prerequisites</span></span>
<span data-ttu-id="55962-107">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="55962-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="55962-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55962-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="55962-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55962-109">Request headers</span></span>
| <span data-ttu-id="55962-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55962-110">Header</span></span>       | <span data-ttu-id="55962-111">Значение</span><span class="sxs-lookup"><span data-stu-id="55962-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55962-112">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55962-112">Authorization</span></span>  | <span data-ttu-id="55962-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55962-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55962-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55962-115">Request body</span></span>
<span data-ttu-id="55962-116">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="55962-116">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="55962-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="55962-117">Response</span></span>

<span data-ttu-id="55962-118">Этот метод возвращает код отклика `204, No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="55962-118">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="55962-119">Пример</span><span class="sxs-lookup"><span data-stu-id="55962-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55962-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="55962-120">Request</span></span>
<span data-ttu-id="55962-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55962-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="55962-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="55962-122">Response</span></span>
<span data-ttu-id="55962-123">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55962-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
