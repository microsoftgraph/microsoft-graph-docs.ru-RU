# <a name="create-rejectedsender"></a><span data-ttu-id="44780-101">Создание объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="44780-101">Create rejectedSender</span></span>

<span data-ttu-id="44780-102">Добавление пользователя или группы в список объектов rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="44780-102">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="44780-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса POST). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="44780-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44780-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="44780-106">Prerequisites</span></span>
<span data-ttu-id="44780-107">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="44780-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="44780-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44780-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="44780-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44780-109">Request headers</span></span>
| <span data-ttu-id="44780-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44780-110">Header</span></span>       | <span data-ttu-id="44780-111">Значение</span><span class="sxs-lookup"><span data-stu-id="44780-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44780-112">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44780-112">Authorization</span></span>  | <span data-ttu-id="44780-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44780-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44780-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44780-115">Request body</span></span>
<span data-ttu-id="44780-116">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="44780-116">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="44780-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="44780-117">Response</span></span>

<span data-ttu-id="44780-118">Этот метод возвращает код отклика `204, No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="44780-118">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="44780-119">Пример</span><span class="sxs-lookup"><span data-stu-id="44780-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44780-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="44780-120">Request</span></span>
<span data-ttu-id="44780-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44780-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="44780-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="44780-122">Response</span></span>
<span data-ttu-id="44780-123">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="44780-123">Here is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
