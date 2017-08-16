# <a name="list-rejectedsenders"></a><span data-ttu-id="e9855-101">Список rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="e9855-101">List rejectedSenders</span></span>

<span data-ttu-id="e9855-102">Получение пользователей или групп из списка rejectedSenders для данной группы.</span><span class="sxs-lookup"><span data-stu-id="e9855-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="e9855-p101">Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса GET). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="e9855-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9855-105">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9855-105">Prerequisites</span></span>
<span data-ttu-id="e9855-106">Для применения этого API требуется одна из указанных **областей**:  *Group.Read.All* или *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="e9855-106">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="e9855-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9855-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9855-108">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e9855-108">Optional query parameters</span></span>
<span data-ttu-id="e9855-109">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e9855-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e9855-110">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9855-110">Request headers</span></span>
| <span data-ttu-id="e9855-111">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9855-111">Header</span></span>       | <span data-ttu-id="e9855-112">Значение</span><span class="sxs-lookup"><span data-stu-id="e9855-112">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9855-113">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9855-113">Authorization</span></span>  | <span data-ttu-id="e9855-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9855-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9855-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9855-116">Request body</span></span>
<span data-ttu-id="e9855-117">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9855-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9855-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9855-118">Response</span></span>

<span data-ttu-id="e9855-119">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9855-119">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9855-120">Пример</span><span class="sxs-lookup"><span data-stu-id="e9855-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9855-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9855-121">Request</span></span>
<span data-ttu-id="e9855-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9855-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
##### <a name="response"></a><span data-ttu-id="e9855-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9855-123">Response</span></span>
<span data-ttu-id="e9855-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9855-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->