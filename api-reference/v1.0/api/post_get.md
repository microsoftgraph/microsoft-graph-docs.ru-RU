# <a name="get-post"></a><span data-ttu-id="e90fa-101">Вывод записи</span><span class="sxs-lookup"><span data-stu-id="e90fa-101">Get post</span></span>

<span data-ttu-id="e90fa-p101">Получение свойств и связей записи в указанной цепочке. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="e90fa-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="e90fa-104">Так как ресурс **post** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **post**.</span><span class="sxs-lookup"><span data-stu-id="e90fa-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e90fa-105">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="e90fa-105">Prerequisites</span></span>
<span data-ttu-id="e90fa-106">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="e90fa-106">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="e90fa-107">*Group.Read.All*, *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="e90fa-107">*Group.Read.All*, *Group.Readwrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e90fa-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e90fa-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e90fa-109">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e90fa-109">Optional query parameters</span></span>
<span data-ttu-id="e90fa-110">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e90fa-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e90fa-111">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e90fa-111">Request headers</span></span>
| <span data-ttu-id="e90fa-112">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e90fa-112">Header</span></span>       | <span data-ttu-id="e90fa-113">Значение</span><span class="sxs-lookup"><span data-stu-id="e90fa-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e90fa-114">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e90fa-114">Authorization</span></span>  | <span data-ttu-id="e90fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e90fa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e90fa-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e90fa-117">Request body</span></span>
<span data-ttu-id="e90fa-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e90fa-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e90fa-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="e90fa-119">Response</span></span>

<span data-ttu-id="e90fa-120">В случае успеха этот метод возвращает код отклика `200 OK` и объект [post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e90fa-120">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e90fa-121">Пример</span><span class="sxs-lookup"><span data-stu-id="e90fa-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e90fa-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="e90fa-122">Request</span></span>
<span data-ttu-id="e90fa-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e90fa-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="e90fa-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="e90fa-124">Response</span></span>
<span data-ttu-id="e90fa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e90fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

{
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "receivedDateTime": "datetime-value",
  "hasAttachments": true,
  "from": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  },
  "sender": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="e90fa-128">См. также</span><span class="sxs-lookup"><span data-stu-id="e90fa-128">See also</span></span>

- [<span data-ttu-id="e90fa-129">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e90fa-129">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e90fa-130">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e90fa-130">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
