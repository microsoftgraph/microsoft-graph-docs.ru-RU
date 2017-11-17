# <a name="list-manager"></a><span data-ttu-id="4642d-101">Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="4642d-101">List manager</span></span>

<span data-ttu-id="4642d-p101">Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный руководителем пользователя.</span><span class="sxs-lookup"><span data-stu-id="4642d-p101">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="4642d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4642d-104">Permissions</span></span>
<span data-ttu-id="4642d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4642d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4642d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4642d-107">Permission type</span></span>      | <span data-ttu-id="4642d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4642d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4642d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4642d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4642d-110">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4642d-110">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4642d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4642d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4642d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4642d-112">Not supported.</span></span>    |
|<span data-ttu-id="4642d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4642d-113">Application</span></span> | <span data-ttu-id="4642d-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4642d-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4642d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4642d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4642d-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4642d-116">Optional query parameters</span></span>
<span data-ttu-id="4642d-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4642d-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4642d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4642d-118">Request headers</span></span>
| <span data-ttu-id="4642d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4642d-119">Header</span></span>       | <span data-ttu-id="4642d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4642d-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4642d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4642d-121">Authorization</span></span>  | <span data-ttu-id="4642d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4642d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4642d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4642d-124">Content-Type</span></span>   | <span data-ttu-id="4642d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4642d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4642d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4642d-126">Request body</span></span>
<span data-ttu-id="4642d-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4642d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4642d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4642d-128">Response</span></span>

<span data-ttu-id="4642d-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4642d-129">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4642d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4642d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4642d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4642d-131">Request</span></span>
<span data-ttu-id="4642d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4642d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="4642d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4642d-133">Response</span></span>
<span data-ttu-id="4642d-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4642d-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
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
