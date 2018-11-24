# <a name="list-directreports"></a><span data-ttu-id="69a49-101">Список directReports</span><span class="sxs-lookup"><span data-stu-id="69a49-101">List directReports</span></span>

<span data-ttu-id="69a49-p101">Получение подчиненных пользователя. Возвращает пользователей и контакты, для которых данный пользователь назначен руководителем.</span><span class="sxs-lookup"><span data-stu-id="69a49-p101">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="69a49-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69a49-104">Permissions</span></span>
<span data-ttu-id="69a49-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69a49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="69a49-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69a49-107">Permission type</span></span>      | <span data-ttu-id="69a49-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69a49-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69a49-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69a49-109">Delegated (work or school account)</span></span> | <span data-ttu-id="69a49-110">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="69a49-110">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="69a49-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69a49-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69a49-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69a49-112">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="69a49-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69a49-113">Application</span></span> | <span data-ttu-id="69a49-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69a49-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69a49-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69a49-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69a49-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="69a49-116">Optional query parameters</span></span>
<span data-ttu-id="69a49-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="69a49-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="69a49-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69a49-118">Request headers</span></span>
| <span data-ttu-id="69a49-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69a49-119">Header</span></span>       | <span data-ttu-id="69a49-120">Значение</span><span class="sxs-lookup"><span data-stu-id="69a49-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="69a49-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69a49-121">Authorization</span></span>  | <span data-ttu-id="69a49-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69a49-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="69a49-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69a49-124">Content-Type</span></span>   | <span data-ttu-id="69a49-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69a49-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69a49-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69a49-126">Request body</span></span>
<span data-ttu-id="69a49-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69a49-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69a49-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="69a49-128">Response</span></span>

<span data-ttu-id="69a49-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69a49-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69a49-130">Пример</span><span class="sxs-lookup"><span data-stu-id="69a49-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69a49-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="69a49-131">Request</span></span>
<span data-ttu-id="69a49-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69a49-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
##### <a name="response"></a><span data-ttu-id="69a49-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="69a49-133">Response</span></span>
<span data-ttu-id="69a49-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="69a49-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->