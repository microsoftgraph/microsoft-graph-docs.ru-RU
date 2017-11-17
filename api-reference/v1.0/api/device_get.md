# <a name="get-device"></a><span data-ttu-id="5c647-101">Получение устройства</span><span class="sxs-lookup"><span data-stu-id="5c647-101">Get device</span></span>

<span data-ttu-id="5c647-102">Получение свойств и связей объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="5c647-102">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c647-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c647-103">Permissions</span></span>
<span data-ttu-id="5c647-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5c647-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c647-106">Permission type</span></span>      | <span data-ttu-id="5c647-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c647-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c647-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c647-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5c647-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c647-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c647-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c647-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c647-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c647-111">Not supported.</span></span>    |
|<span data-ttu-id="5c647-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c647-112">Application</span></span> | <span data-ttu-id="5c647-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c647-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c647-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c647-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="5c647-115">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="5c647-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="5c647-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c647-116">Optional query parameters</span></span>
<span data-ttu-id="5c647-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c647-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c647-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c647-118">Request headers</span></span>
| <span data-ttu-id="5c647-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5c647-119">Name</span></span>       | <span data-ttu-id="5c647-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5c647-120">Type</span></span> | <span data-ttu-id="5c647-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5c647-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5c647-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c647-122">Authorization</span></span>  | <span data-ttu-id="5c647-123">string</span><span class="sxs-lookup"><span data-stu-id="5c647-123">string</span></span>  | <span data-ttu-id="5c647-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c647-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c647-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c647-126">Request body</span></span>
<span data-ttu-id="5c647-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c647-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c647-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c647-128">Response</span></span>

<span data-ttu-id="5c647-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c647-129">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c647-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5c647-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c647-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c647-131">Request</span></span>
<span data-ttu-id="5c647-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c647-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="5c647-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c647-133">Response</span></span>
<span data-ttu-id="5c647-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c647-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
