# <a name="list-subscribedskus"></a><span data-ttu-id="41862-101">Список объектов SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="41862-101">List subscribedSkus</span></span>
<span data-ttu-id="41862-102">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="41862-102">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="41862-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41862-103">Permissions</span></span>
<span data-ttu-id="41862-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="41862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="41862-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41862-106">Permission type</span></span>      | <span data-ttu-id="41862-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41862-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41862-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41862-108">Delegated (work or school account)</span></span> | <span data-ttu-id="41862-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41862-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41862-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41862-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41862-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41862-111">Not supported.</span></span>    |
|<span data-ttu-id="41862-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41862-112">Application</span></span> | <span data-ttu-id="41862-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41862-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41862-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41862-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41862-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41862-115">Optional query parameters</span></span>
<span data-ttu-id="41862-116">Этот метод **не** поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="41862-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="41862-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41862-117">Request headers</span></span>
| <span data-ttu-id="41862-118">Имя</span><span class="sxs-lookup"><span data-stu-id="41862-118">Name</span></span>       | <span data-ttu-id="41862-119">Тип</span><span class="sxs-lookup"><span data-stu-id="41862-119">Type</span></span> | <span data-ttu-id="41862-120">Описание</span><span class="sxs-lookup"><span data-stu-id="41862-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41862-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41862-121">Authorization</span></span>  | <span data-ttu-id="41862-122">string</span><span class="sxs-lookup"><span data-stu-id="41862-122">string</span></span>  | <span data-ttu-id="41862-p102">&lt;Токен&gt; носителя. *Обязательный*</span><span class="sxs-lookup"><span data-stu-id="41862-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="41862-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41862-125">Request body</span></span>
<span data-ttu-id="41862-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41862-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41862-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="41862-127">Response</span></span>

<span data-ttu-id="41862-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41862-128">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41862-129">Пример</span><span class="sxs-lookup"><span data-stu-id="41862-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41862-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="41862-130">Request</span></span>
<span data-ttu-id="41862-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41862-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
##### <a name="response"></a><span data-ttu-id="41862-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="41862-132">Response</span></span>
<span data-ttu-id="41862-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="41862-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus",
    "value": [
        {
            "capabilityStatus": "Enabled",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
            "prepaidUnits": {
                "enabled": 25,
                "suspended": 0,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
                    "servicePlanName": "ADALLOM_S_O365",
                    "provisioningStatus": "Success",
                    "appliesTo": "User"
                }
            ],
            "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
            "skuPartNumber": "ENTERPRISEPREMIUM",
            "appliesTo": "User"
        },
        {
            "capabilityStatus": "Suspended",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_d17b27af-3f49-4822-99f9-56a661538792",
            "prepaidUnits": {
                "enabled": 0,
                "suspended": 25,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "f9646fb2-e3b2-4309-95de-dc4833737456",
                    "servicePlanName": "CRMSTANDARD",
                    "provisioningStatus": "Disabled",
                    "appliesTo": "User"
                }
            ],
            "skuId": "d17b27af-3f49-4822-99f9-56a661538792",
            "skuPartNumber": "CRMSTANDARD",
            "appliesTo": "User"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
