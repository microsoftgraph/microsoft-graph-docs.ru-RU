# <a name="create-educationschool"></a><span data-ttu-id="c1913-101">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="c1913-101">Create educationSchool</span></span>

<span data-ttu-id="c1913-102">Создание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="c1913-102">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1913-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1913-103">Permissions</span></span>
<span data-ttu-id="c1913-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1913-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1913-106">Permission type</span></span>      | <span data-ttu-id="c1913-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1913-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1913-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1913-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="c1913-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1913-109">Not supported.</span></span>  |
|<span data-ttu-id="c1913-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1913-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c1913-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1913-111">Not supported.</span></span>  |
|<span data-ttu-id="c1913-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1913-112">Application</span></span> | <span data-ttu-id="c1913-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1913-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c1913-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1913-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="c1913-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1913-115">Request headers</span></span>
| <span data-ttu-id="c1913-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1913-116">Header</span></span>       | <span data-ttu-id="c1913-117">Значение</span><span class="sxs-lookup"><span data-stu-id="c1913-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1913-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1913-118">Authorization</span></span>  | <span data-ttu-id="c1913-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1913-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1913-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1913-121">Content-Type</span></span>  | <span data-ttu-id="c1913-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c1913-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1913-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1913-123">Request body</span></span>
<span data-ttu-id="c1913-124">В теле запроса предоставьте описание объекта [educationSchool](../resources/educationschool.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1913-124">In the request body, supply a JSON representation of an [invitation](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c1913-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1913-125">Response</span></span>
<span data-ttu-id="c1913-126">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1913-126">If successful, this method returns a `201 Created` response code and an [event](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1913-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c1913-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1913-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1913-128">Request</span></span>
<span data-ttu-id="c1913-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1913-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

##### <a name="response"></a><span data-ttu-id="c1913-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1913-130">Response</span></span>
<span data-ttu-id="c1913-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1913-131">The following is an example of the response.</span></span> 

><span data-ttu-id="c1913-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1913-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
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
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->