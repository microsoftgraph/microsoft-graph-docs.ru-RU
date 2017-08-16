# <a name="list-posts"></a><span data-ttu-id="070d7-101">Список записей</span><span class="sxs-lookup"><span data-stu-id="070d7-101">List posts</span></span>

<span data-ttu-id="070d7-p101">Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="070d7-p101">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="070d7-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="070d7-104">Prerequisites</span></span>
<span data-ttu-id="070d7-105">Для применения этого API требуется одна из указанных ниже **областей**. *Group.ReadWrite.All; Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="070d7-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All; Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="070d7-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="070d7-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="070d7-107">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="070d7-107">Optional query parameters</span></span>
<span data-ttu-id="070d7-108">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="070d7-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="070d7-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="070d7-109">Request headers</span></span>
| <span data-ttu-id="070d7-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="070d7-110">Header</span></span>       | <span data-ttu-id="070d7-111">Значение</span><span class="sxs-lookup"><span data-stu-id="070d7-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="070d7-112">Авторизация</span><span class="sxs-lookup"><span data-stu-id="070d7-112">Authorization</span></span>  | <span data-ttu-id="070d7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="070d7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="070d7-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="070d7-115">Request body</span></span>
<span data-ttu-id="070d7-116">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="070d7-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="070d7-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="070d7-117">Response</span></span>

<span data-ttu-id="070d7-118">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="070d7-118">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="070d7-119">Пример</span><span class="sxs-lookup"><span data-stu-id="070d7-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="070d7-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="070d7-120">Request</span></span>
<span data-ttu-id="070d7-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="070d7-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="070d7-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="070d7-122">Response</span></span>
<span data-ttu-id="070d7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="070d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
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
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
