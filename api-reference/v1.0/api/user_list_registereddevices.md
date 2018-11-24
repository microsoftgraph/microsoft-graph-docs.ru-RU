# <a name="list-registereddevices"></a><span data-ttu-id="5d313-101">Список registeredDevices</span><span class="sxs-lookup"><span data-stu-id="5d313-101">List registeredDevices</span></span>

<span data-ttu-id="5d313-102">Получение списка зарегистрированных устройств пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d313-102">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d313-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d313-103">Permissions</span></span>
<span data-ttu-id="5d313-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d313-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d313-106">Permission type</span></span>      | <span data-ttu-id="5d313-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d313-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d313-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d313-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5d313-109">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d313-109">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d313-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d313-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d313-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d313-111">Not supported.</span></span>    |
|<span data-ttu-id="5d313-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d313-112">Application</span></span> | <span data-ttu-id="5d313-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d313-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d313-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d313-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d313-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5d313-115">Optional query parameters</span></span>
<span data-ttu-id="5d313-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5d313-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5d313-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d313-117">Request headers</span></span>
| <span data-ttu-id="5d313-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d313-118">Header</span></span>       | <span data-ttu-id="5d313-119">Значение</span><span class="sxs-lookup"><span data-stu-id="5d313-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d313-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d313-120">Authorization</span></span>  | <span data-ttu-id="5d313-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d313-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5d313-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5d313-123">Accept</span></span>  | <span data-ttu-id="5d313-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5d313-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d313-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d313-125">Request body</span></span>
<span data-ttu-id="5d313-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d313-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d313-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d313-127">Response</span></span>

<span data-ttu-id="5d313-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d313-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d313-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5d313-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d313-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d313-130">Request</span></span>
<span data-ttu-id="5d313-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d313-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="5d313-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d313-132">Response</span></span>
<span data-ttu-id="5d313-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5d313-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->