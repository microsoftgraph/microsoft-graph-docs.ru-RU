# <a name="list-memberof"></a><span data-ttu-id="c0346-101">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="c0346-101">List memberOf</span></span>

<span data-ttu-id="c0346-102">Получение групп, непосредственным членом которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="c0346-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="c0346-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Office 365", эта операция возвращает группы всех типов, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="c0346-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c0346-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0346-105">Permissions</span></span>
<span data-ttu-id="c0346-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0346-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c0346-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0346-108">Permission type</span></span>      | <span data-ttu-id="c0346-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0346-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0346-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0346-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0346-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0346-111">Group.Read.All</span></span>    |
|<span data-ttu-id="c0346-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0346-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0346-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0346-113">Not supported.</span></span>    |
|<span data-ttu-id="c0346-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0346-114">Application</span></span> | <span data-ttu-id="c0346-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0346-115">Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0346-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0346-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0346-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0346-117">Optional query parameters</span></span>
<span data-ttu-id="c0346-118">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0346-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c0346-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0346-119">Request headers</span></span>
| <span data-ttu-id="c0346-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c0346-120">Name</span></span>       | <span data-ttu-id="c0346-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c0346-121">Type</span></span> | <span data-ttu-id="c0346-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c0346-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0346-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0346-123">Authorization</span></span>  | <span data-ttu-id="c0346-124">string</span><span class="sxs-lookup"><span data-stu-id="c0346-124">string</span></span>  | <span data-ttu-id="c0346-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0346-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0346-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0346-127">Request body</span></span>
<span data-ttu-id="c0346-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0346-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0346-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0346-129">Response</span></span>

<span data-ttu-id="c0346-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0346-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0346-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c0346-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0346-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0346-132">Request</span></span>
<span data-ttu-id="c0346-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0346-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="c0346-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0346-134">Response</span></span>
<span data-ttu-id="c0346-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c0346-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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