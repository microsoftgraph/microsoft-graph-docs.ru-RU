# <a name="list-devices"></a><span data-ttu-id="d8809-101">Список устройств</span><span class="sxs-lookup"><span data-stu-id="d8809-101">List devices</span></span>

<span data-ttu-id="d8809-102">Получение списка объектов устройств, зарегистрированных в организации.</span><span class="sxs-lookup"><span data-stu-id="d8809-102">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8809-103">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8809-103">Prerequisites</span></span>
<span data-ttu-id="d8809-104">Для выполнения этого API требуется одно из следующих **разрешений**: *Device.ReadWrite.All*, *Directory.Read.All*, *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="d8809-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="d8809-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8809-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8809-106">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8809-106">Optional query parameters</span></span>
<span data-ttu-id="d8809-107">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8809-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8809-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8809-108">Request headers</span></span>
| <span data-ttu-id="d8809-109">Имя</span><span class="sxs-lookup"><span data-stu-id="d8809-109">Name</span></span>       | <span data-ttu-id="d8809-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d8809-110">Type</span></span> | <span data-ttu-id="d8809-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8809-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d8809-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8809-112">Authorization</span></span>  | <span data-ttu-id="d8809-113">string</span><span class="sxs-lookup"><span data-stu-id="d8809-113">string</span></span>  | <span data-ttu-id="d8809-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8809-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8809-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8809-116">Request body</span></span>
<span data-ttu-id="d8809-117">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8809-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8809-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8809-118">Response</span></span>

<span data-ttu-id="d8809-119">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8809-119">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8809-120">Пример</span><span class="sxs-lookup"><span data-stu-id="d8809-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8809-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8809-121">Request</span></span>
<span data-ttu-id="d8809-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8809-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="d8809-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8809-123">Response</span></span>
<span data-ttu-id="d8809-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d8809-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "alternativeSecurityIds":
      [
        {
          "type":2,
          "key":"Y3YxN2E1MWFlYw==",
          "identityProvider": null
        }
      ],
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
