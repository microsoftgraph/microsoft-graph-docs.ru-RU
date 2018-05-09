# <a name="get-organization"></a><span data-ttu-id="d7a96-101">Получение организации</span><span class="sxs-lookup"><span data-stu-id="d7a96-101">Get organization</span></span>

<span data-ttu-id="d7a96-102">Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="d7a96-102">Retrieve the properties and relationships of currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7a96-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7a96-103">Permissions</span></span>
<span data-ttu-id="d7a96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d7a96-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7a96-106">Permission type</span></span>      | <span data-ttu-id="d7a96-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7a96-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7a96-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7a96-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d7a96-109">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a96-109">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="d7a96-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7a96-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7a96-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7a96-111">Not supported.</span></span>    |
|<span data-ttu-id="d7a96-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7a96-112">Application</span></span> | <span data-ttu-id="d7a96-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a96-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d7a96-114">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="d7a96-114">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="d7a96-115">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="d7a96-115">All other properties will return with `null` values.</span></span> <span data-ttu-id="d7a96-116">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="d7a96-116">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="d7a96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7a96-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization

```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7a96-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7a96-118">Optional query parameters</span></span>
<span data-ttu-id="d7a96-119">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d7a96-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d7a96-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7a96-120">Request headers</span></span>
| <span data-ttu-id="d7a96-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d7a96-121">Name</span></span>       | <span data-ttu-id="d7a96-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d7a96-122">Type</span></span> | <span data-ttu-id="d7a96-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d7a96-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7a96-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7a96-124">Authorization</span></span>  | <span data-ttu-id="d7a96-125">string</span><span class="sxs-lookup"><span data-stu-id="d7a96-125">string</span></span>  | <span data-ttu-id="d7a96-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7a96-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7a96-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7a96-128">Request body</span></span>
<span data-ttu-id="d7a96-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7a96-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7a96-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7a96-130">Response</span></span>

<span data-ttu-id="d7a96-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7a96-131">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7a96-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d7a96-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7a96-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7a96-133">Request</span></span>
<span data-ttu-id="d7a96-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7a96-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/v1.0/organization
```
##### <a name="response"></a><span data-ttu-id="d7a96-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7a96-135">Response</span></span>
<span data-ttu-id="d7a96-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d7a96-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->