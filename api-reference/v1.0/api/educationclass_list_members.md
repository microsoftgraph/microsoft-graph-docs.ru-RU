# <a name="list-members"></a><span data-ttu-id="50c67-101">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="50c67-101">List members</span></span>

<span data-ttu-id="50c67-102">Получает преподавателей и учащихся для курса.</span><span class="sxs-lookup"><span data-stu-id="50c67-102">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="50c67-103">Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.</span><span class="sxs-lookup"><span data-stu-id="50c67-103">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="50c67-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50c67-104">Permissions</span></span>
<span data-ttu-id="50c67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="50c67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="50c67-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50c67-107">Permission type</span></span>      | <span data-ttu-id="50c67-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50c67-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50c67-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50c67-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="50c67-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="50c67-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="50c67-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50c67-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="50c67-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50c67-112">Not supported</span></span>  |
|<span data-ttu-id="50c67-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50c67-113">Application</span></span> | <span data-ttu-id="50c67-114">EduRoster.Read.All, EduRoster.ReadWrite.All, а также Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="50c67-114">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="50c67-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50c67-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50c67-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50c67-116">Optional query parameters</span></span>
<span data-ttu-id="50c67-117">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50c67-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50c67-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50c67-118">Request headers</span></span>
| <span data-ttu-id="50c67-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50c67-119">Header</span></span>       | <span data-ttu-id="50c67-120">Значение</span><span class="sxs-lookup"><span data-stu-id="50c67-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50c67-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50c67-121">Authorization</span></span>  | <span data-ttu-id="50c67-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50c67-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50c67-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50c67-124">Request body</span></span>
<span data-ttu-id="50c67-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50c67-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="50c67-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="50c67-126">Response</span></span>
<span data-ttu-id="50c67-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="50c67-127">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50c67-128">Пример</span><span class="sxs-lookup"><span data-stu-id="50c67-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50c67-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="50c67-129">Request</span></span>
<span data-ttu-id="50c67-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50c67-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
##### <a name="response"></a><span data-ttu-id="50c67-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="50c67-131">Response</span></span>
<span data-ttu-id="50c67-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="50c67-132">The following is an example of the response.</span></span> 

><span data-ttu-id="50c67-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50c67-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
