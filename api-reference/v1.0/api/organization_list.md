# <a name="list-organization"></a><span data-ttu-id="7cbdd-101">Список организаций</span><span class="sxs-lookup"><span data-stu-id="7cbdd-101">List organization</span></span>

> <span data-ttu-id="7cbdd-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cbdd-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-103">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7cbdd-104">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7cbdd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cbdd-105">Permissions</span></span>
<span data-ttu-id="7cbdd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7cbdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7cbdd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cbdd-108">Permission type</span></span>      | <span data-ttu-id="7cbdd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cbdd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cbdd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cbdd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7cbdd-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cbdd-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="7cbdd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cbdd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cbdd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-113">Not supported.</span></span>    |
|<span data-ttu-id="7cbdd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cbdd-114">Application</span></span> | <span data-ttu-id="7cbdd-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cbdd-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="7cbdd-116">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="7cbdd-117">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="7cbdd-118">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="7cbdd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cbdd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7cbdd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7cbdd-120">Optional query parameters</span></span>
<span data-ttu-id="7cbdd-121">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7cbdd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cbdd-122">Request headers</span></span>
| <span data-ttu-id="7cbdd-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7cbdd-123">Name</span></span>       | <span data-ttu-id="7cbdd-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7cbdd-124">Type</span></span> | <span data-ttu-id="7cbdd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7cbdd-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7cbdd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cbdd-126">Authorization</span></span>  | <span data-ttu-id="7cbdd-127">string</span><span class="sxs-lookup"><span data-stu-id="7cbdd-127">string</span></span>  | <span data-ttu-id="7cbdd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cbdd-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cbdd-130">Request body</span></span>
<span data-ttu-id="7cbdd-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cbdd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cbdd-132">Response</span></span>

<span data-ttu-id="7cbdd-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7cbdd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7cbdd-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cbdd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cbdd-135">Request</span></span>
<span data-ttu-id="7cbdd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cbdd-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="7cbdd-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cbdd-137">Response</span></span>
<span data-ttu-id="7cbdd-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7cbdd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->