# <a name="list-schools"></a><span data-ttu-id="4bb96-101">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="4bb96-101">List schools</span></span>

<span data-ttu-id="4bb96-102">Получение списка учебных заведений для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4bb96-102">Retrieve a list of licenseDetails objects for a user.</span></span>

><span data-ttu-id="4bb96-103">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="4bb96-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="4bb96-104">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="4bb96-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bb96-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb96-105">Permissions</span></span>
<span data-ttu-id="4bb96-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bb96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4bb96-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb96-108">Permission type</span></span>      | <span data-ttu-id="4bb96-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bb96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bb96-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bb96-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4bb96-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="4bb96-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="4bb96-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bb96-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4bb96-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb96-113">Not supported.</span></span>  |
|<span data-ttu-id="4bb96-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bb96-114">Application</span></span> | <span data-ttu-id="4bb96-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bb96-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4bb96-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bb96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4bb96-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4bb96-117">Optional query parameters</span></span>
<span data-ttu-id="4bb96-118">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4bb96-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bb96-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bb96-119">Request headers</span></span>
| <span data-ttu-id="4bb96-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bb96-120">Header</span></span>       | <span data-ttu-id="4bb96-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4bb96-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4bb96-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bb96-122">Authorization</span></span>  | <span data-ttu-id="4bb96-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bb96-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4bb96-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bb96-125">Request body</span></span>
<span data-ttu-id="4bb96-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bb96-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4bb96-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bb96-127">Response</span></span>
<span data-ttu-id="4bb96-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4bb96-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4bb96-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4bb96-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bb96-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bb96-130">Request</span></span>
<span data-ttu-id="4bb96-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bb96-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="4bb96-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bb96-132">Response</span></span>
<span data-ttu-id="4bb96-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4bb96-133">The following is an example of the response.</span></span> 

><span data-ttu-id="4bb96-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bb96-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->