# <a name="list-memberof"></a><span data-ttu-id="c0414-101">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="c0414-101">List memberOf</span></span>

<span data-ttu-id="c0414-102">Получение групп, непосредственным членом которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="c0414-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="c0414-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Office 365", эта операция возвращает группы всех типов, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="c0414-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="c0414-105">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c0414-105">Prerequisites</span></span>
<span data-ttu-id="c0414-106">Для применения этого API требуется одна из указанных **областей**: *Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="c0414-106">One of the following **scopes** is required to execute this API: *Group.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="c0414-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0414-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0414-108">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0414-108">Optional query parameters</span></span>
<span data-ttu-id="c0414-109">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0414-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c0414-110">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0414-110">Request headers</span></span>
| <span data-ttu-id="c0414-111">Имя</span><span class="sxs-lookup"><span data-stu-id="c0414-111">Name</span></span>       | <span data-ttu-id="c0414-112">Тип</span><span class="sxs-lookup"><span data-stu-id="c0414-112">Type</span></span> | <span data-ttu-id="c0414-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c0414-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0414-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0414-114">Authorization</span></span>  | <span data-ttu-id="c0414-115">string</span><span class="sxs-lookup"><span data-stu-id="c0414-115">string</span></span>  | <span data-ttu-id="c0414-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0414-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0414-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0414-118">Request body</span></span>
<span data-ttu-id="c0414-119">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0414-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0414-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0414-120">Response</span></span>

<span data-ttu-id="c0414-121">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0414-121">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0414-122">Пример</span><span class="sxs-lookup"><span data-stu-id="c0414-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0414-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0414-123">Request</span></span>
<span data-ttu-id="c0414-124">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0414-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="c0414-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0414-125">Response</span></span>
<span data-ttu-id="c0414-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c0414-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->