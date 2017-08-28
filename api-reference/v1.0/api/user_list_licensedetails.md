# <a name="list-licensedetails"></a><span data-ttu-id="a539f-101">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="a539f-101">List licenseDetails</span></span>

<span data-ttu-id="a539f-102">Получение списка объектов licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="a539f-102">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a539f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a539f-103">Permissions</span></span>
<span data-ttu-id="a539f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a539f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a539f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a539f-106">Permission type</span></span>      | <span data-ttu-id="a539f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a539f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a539f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a539f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a539f-109">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a539f-109">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a539f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a539f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a539f-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="a539f-111">User.Read</span></span>    |
|<span data-ttu-id="a539f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a539f-112">Application</span></span> | <span data-ttu-id="a539f-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a539f-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a539f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a539f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a539f-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a539f-115">Optional query parameters</span></span>
<span data-ttu-id="a539f-116">Этот метод **не** поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="a539f-116">This method does **not** support [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a539f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a539f-117">Request headers</span></span>
| <span data-ttu-id="a539f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a539f-118">Name</span></span>      |<span data-ttu-id="a539f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a539f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a539f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a539f-120">Authorization</span></span>  | <span data-ttu-id="a539f-121">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="a539f-121">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="a539f-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a539f-122">Request body</span></span>
<span data-ttu-id="a539f-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a539f-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a539f-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="a539f-124">Response</span></span>

<span data-ttu-id="a539f-125">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [licenseDetails](../resources/licensedetails.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a539f-125">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a539f-126">Пример</span><span class="sxs-lookup"><span data-stu-id="a539f-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a539f-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="a539f-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="a539f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a539f-128">Response</span></span>
<span data-ttu-id="a539f-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a539f-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->