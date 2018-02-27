# <a name="list-educationusers"></a><span data-ttu-id="2f7fa-101">Перечисление EducationUsers</span><span class="sxs-lookup"><span data-stu-id="2f7fa-101">List educationUsers</span></span>

<span data-ttu-id="2f7fa-102">Получение списка пользователей в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-102">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f7fa-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f7fa-103">Permissions</span></span>
<span data-ttu-id="2f7fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f7fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f7fa-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f7fa-106">Permission type</span></span>      | <span data-ttu-id="2f7fa-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f7fa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f7fa-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f7fa-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f7fa-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2f7fa-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2f7fa-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f7fa-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f7fa-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-111">Not supported.</span></span>  |
|<span data-ttu-id="2f7fa-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f7fa-112">Application</span></span> | <span data-ttu-id="2f7fa-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7fa-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f7fa-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f7fa-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f7fa-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f7fa-115">Optional query parameters</span></span>
<span data-ttu-id="2f7fa-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f7fa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f7fa-117">Request headers</span></span>
| <span data-ttu-id="2f7fa-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f7fa-118">Header</span></span>       | <span data-ttu-id="2f7fa-119">Значение</span><span class="sxs-lookup"><span data-stu-id="2f7fa-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f7fa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f7fa-120">Authorization</span></span>  | <span data-ttu-id="2f7fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f7fa-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f7fa-123">Request body</span></span>
<span data-ttu-id="2f7fa-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2f7fa-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f7fa-125">Response</span></span>
<span data-ttu-id="2f7fa-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f7fa-127">Пример</span><span class="sxs-lookup"><span data-stu-id="2f7fa-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f7fa-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f7fa-128">Request</span></span>
<span data-ttu-id="2f7fa-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="2f7fa-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f7fa-130">Response</span></span>
<span data-ttu-id="2f7fa-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-131">The following is an example of the response.</span></span> 

><span data-ttu-id="2f7fa-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f7fa-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": " ",
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
