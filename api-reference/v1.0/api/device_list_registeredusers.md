# <a name="list-registeredusers"></a><span data-ttu-id="bedce-101">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="bedce-101">List registeredUsers</span></span>

<span data-ttu-id="bedce-102">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="bedce-102">Retrieve a list of users that are registered users of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="bedce-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bedce-103">Permissions</span></span>
<span data-ttu-id="bedce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bedce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
- <span data-ttu-id="bedce-106">*Device.ReadWrite.All* и *User.ReadBasic.All*</span><span class="sxs-lookup"><span data-stu-id="bedce-106">*Device.ReadWrite.All* and *User.ReadBasic.All*</span></span>
- <span data-ttu-id="bedce-107">*Directory.Read.All*</span><span class="sxs-lookup"><span data-stu-id="bedce-107">*Directory.Read.All*</span></span>
- <span data-ttu-id="bedce-108">*Directory.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="bedce-108">*Directory.ReadWrite.All*</span></span> 
- <span data-ttu-id="bedce-109">*Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="bedce-109">*Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="bedce-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bedce-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bedce-111">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bedce-111">Optional query parameters</span></span>
<span data-ttu-id="bedce-112">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bedce-112">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bedce-113">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bedce-113">Request headers</span></span>
| <span data-ttu-id="bedce-114">Имя</span><span class="sxs-lookup"><span data-stu-id="bedce-114">Name</span></span>       | <span data-ttu-id="bedce-115">Тип</span><span class="sxs-lookup"><span data-stu-id="bedce-115">Type</span></span> | <span data-ttu-id="bedce-116">Описание</span><span class="sxs-lookup"><span data-stu-id="bedce-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bedce-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="bedce-117">Authorization</span></span>  | <span data-ttu-id="bedce-118">string</span><span class="sxs-lookup"><span data-stu-id="bedce-118">string</span></span>  | <span data-ttu-id="bedce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bedce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bedce-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bedce-121">Request body</span></span>
<span data-ttu-id="bedce-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bedce-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bedce-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="bedce-123">Response</span></span>

<span data-ttu-id="bedce-124">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bedce-124">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bedce-125">Пример</span><span class="sxs-lookup"><span data-stu-id="bedce-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bedce-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="bedce-126">Request</span></span>
<span data-ttu-id="bedce-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bedce-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="bedce-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bedce-128">Response</span></span>
<span data-ttu-id="bedce-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bedce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->