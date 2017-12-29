# <a name="create-rejectedsender"></a><span data-ttu-id="5ab44-101">Создание объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="5ab44-101">Create rejectedSender</span></span>
<span data-ttu-id="5ab44-102">Добавление пользователя или группы в список объектов rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="5ab44-102">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="5ab44-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса POST). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="5ab44-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ab44-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ab44-106">Permissions</span></span>
<span data-ttu-id="5ab44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5ab44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ab44-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ab44-109">Permission type</span></span>      | <span data-ttu-id="5ab44-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ab44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ab44-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ab44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ab44-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ab44-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ab44-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ab44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ab44-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ab44-114">Not supported.</span></span>    |
|<span data-ttu-id="5ab44-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ab44-115">Application</span></span> | <span data-ttu-id="5ab44-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ab44-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ab44-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ab44-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5ab44-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ab44-118">Request headers</span></span>
| <span data-ttu-id="5ab44-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ab44-119">Header</span></span>       | <span data-ttu-id="5ab44-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5ab44-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ab44-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ab44-121">Authorization</span></span>  | <span data-ttu-id="5ab44-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ab44-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ab44-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ab44-124">Request body</span></span>
<span data-ttu-id="5ab44-125">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="5ab44-125">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="5ab44-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ab44-126">Response</span></span>
<span data-ttu-id="5ab44-127">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="5ab44-127">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ab44-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5ab44-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5ab44-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ab44-129">Request</span></span>
<span data-ttu-id="5ab44-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ab44-130">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="5ab44-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ab44-131">Response</span></span>
<span data-ttu-id="5ab44-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5ab44-132">The following is an example of the response.</span></span>
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
