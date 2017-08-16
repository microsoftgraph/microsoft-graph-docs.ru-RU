# <a name="get-device"></a><span data-ttu-id="662dd-101">Получение устройства</span><span class="sxs-lookup"><span data-stu-id="662dd-101">Get device</span></span>

<span data-ttu-id="662dd-102">Получение свойств и связей объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="662dd-102">Get the properties and relationships of a device object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="662dd-103">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="662dd-103">Prerequisites</span></span>
<span data-ttu-id="662dd-104">Для выполнения этого API требуется одно из следующих **разрешений**: *Device.ReadWrite.All*, *Directory.Read.All*, *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="662dd-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="662dd-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="662dd-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="662dd-106">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="662dd-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="662dd-107">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="662dd-107">Optional query parameters</span></span>
<span data-ttu-id="662dd-108">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="662dd-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="662dd-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="662dd-109">Request headers</span></span>
| <span data-ttu-id="662dd-110">Имя</span><span class="sxs-lookup"><span data-stu-id="662dd-110">Name</span></span>       | <span data-ttu-id="662dd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="662dd-111">Type</span></span> | <span data-ttu-id="662dd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="662dd-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="662dd-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="662dd-113">Authorization</span></span>  | <span data-ttu-id="662dd-114">string</span><span class="sxs-lookup"><span data-stu-id="662dd-114">string</span></span>  | <span data-ttu-id="662dd-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="662dd-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="662dd-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="662dd-117">Request body</span></span>
<span data-ttu-id="662dd-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="662dd-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="662dd-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="662dd-119">Response</span></span>

<span data-ttu-id="662dd-120">В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="662dd-120">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="662dd-121">Пример</span><span class="sxs-lookup"><span data-stu-id="662dd-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="662dd-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="662dd-122">Request</span></span>
<span data-ttu-id="662dd-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="662dd-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="662dd-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="662dd-124">Response</span></span>
<span data-ttu-id="662dd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="662dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type": 2,
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
