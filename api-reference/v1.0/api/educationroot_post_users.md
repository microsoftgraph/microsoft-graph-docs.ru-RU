# <a name="create-educationuser"></a><span data-ttu-id="75f46-101">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="75f46-101">Create educationUser</span></span>

<span data-ttu-id="75f46-102">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="75f46-102">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="75f46-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75f46-103">Permissions</span></span>
<span data-ttu-id="75f46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75f46-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75f46-106">Permission type</span></span>      | <span data-ttu-id="75f46-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75f46-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75f46-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75f46-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="75f46-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f46-109">Not supported.</span></span>  |
|<span data-ttu-id="75f46-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75f46-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="75f46-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f46-111">Not supported.</span></span>  |
|<span data-ttu-id="75f46-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75f46-112">Application</span></span> | <span data-ttu-id="75f46-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f46-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="75f46-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75f46-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="75f46-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75f46-115">Request headers</span></span>
| <span data-ttu-id="75f46-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75f46-116">Header</span></span>       | <span data-ttu-id="75f46-117">Значение</span><span class="sxs-lookup"><span data-stu-id="75f46-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75f46-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75f46-118">Authorization</span></span>  | <span data-ttu-id="75f46-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75f46-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="75f46-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75f46-121">Content-Type</span></span>  | <span data-ttu-id="75f46-122">application/json</span><span class="sxs-lookup"><span data-stu-id="75f46-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75f46-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75f46-123">Request body</span></span>
<span data-ttu-id="75f46-124">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75f46-124">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="75f46-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f46-125">Response</span></span>
<span data-ttu-id="75f46-126">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="75f46-126">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75f46-127">Пример</span><span class="sxs-lookup"><span data-stu-id="75f46-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75f46-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f46-128">Request</span></span>
<span data-ttu-id="75f46-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75f46-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/users
Content-type: application/json
Content-length: 508

{
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": null,
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
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
```

##### <a name="response"></a><span data-ttu-id="75f46-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f46-130">Response</span></span>
<span data-ttu-id="75f46-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75f46-131">The following is an example of the response.</span></span> 

><span data-ttu-id="75f46-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75f46-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 508

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->