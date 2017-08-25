# <a name="list-posts"></a><span data-ttu-id="00db1-101">Список записей</span><span class="sxs-lookup"><span data-stu-id="00db1-101">List posts</span></span>

<span data-ttu-id="00db1-p101">Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="00db1-p101">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="00db1-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00db1-104">Permissions</span></span>
<span data-ttu-id="00db1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="00db1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00db1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00db1-107">Permission type</span></span>      | <span data-ttu-id="00db1-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00db1-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="00db1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00db1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="00db1-110">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="00db1-110">Group.ReadWrite.All, Group.Read.All</span></span>    | 
|<span data-ttu-id="00db1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00db1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00db1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00db1-112">Not supported.</span></span>    | 
|<span data-ttu-id="00db1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00db1-113">Application</span></span> | <span data-ttu-id="00db1-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="00db1-114">Group.ReadWrite.All, Group.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="00db1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00db1-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="00db1-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="00db1-116">Optional query parameters</span></span>
<span data-ttu-id="00db1-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="00db1-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="00db1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00db1-118">Request headers</span></span>
| <span data-ttu-id="00db1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00db1-119">Header</span></span>       | <span data-ttu-id="00db1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="00db1-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00db1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00db1-121">Authorization</span></span>  | <span data-ttu-id="00db1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00db1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00db1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00db1-124">Request body</span></span>
<span data-ttu-id="00db1-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00db1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00db1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="00db1-126">Response</span></span>

<span data-ttu-id="00db1-127">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00db1-127">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00db1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="00db1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00db1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="00db1-129">Request</span></span>
<span data-ttu-id="00db1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00db1-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="00db1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="00db1-131">Response</span></span>
<span data-ttu-id="00db1-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00db1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
