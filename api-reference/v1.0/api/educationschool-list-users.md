---
title: Перечисление EducationUsers
description: Получение списка пользователей в учебном заведении.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2016034bed632210891cd872425ff000c3835c00
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726888"
---
# <a name="list-educationusers"></a><span data-ttu-id="d1ce9-103">Перечисление EducationUsers</span><span class="sxs-lookup"><span data-stu-id="d1ce9-103">List educationUsers</span></span>

<span data-ttu-id="d1ce9-104">Получение списка пользователей в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-104">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1ce9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1ce9-105">Permissions</span></span>
<span data-ttu-id="d1ce9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1ce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1ce9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1ce9-108">Permission type</span></span>      | <span data-ttu-id="d1ce9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1ce9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1ce9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1ce9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d1ce9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-111">Not supported.</span></span>  |
|<span data-ttu-id="d1ce9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1ce9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d1ce9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-113">Not supported.</span></span>  |
|<span data-ttu-id="d1ce9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1ce9-114">Application</span></span> | <span data-ttu-id="d1ce9-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1ce9-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d1ce9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1ce9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1ce9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1ce9-117">Optional query parameters</span></span>
<span data-ttu-id="d1ce9-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1ce9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1ce9-119">Request headers</span></span>
| <span data-ttu-id="d1ce9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1ce9-120">Header</span></span>       | <span data-ttu-id="d1ce9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d1ce9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1ce9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1ce9-122">Authorization</span></span>  | <span data-ttu-id="d1ce9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1ce9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1ce9-125">Request body</span></span>
<span data-ttu-id="d1ce9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d1ce9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1ce9-127">Response</span></span>
<span data-ttu-id="d1ce9-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-128">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1ce9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d1ce9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1ce9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1ce9-130">Request</span></span>
<span data-ttu-id="d1ce9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d1ce9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1ce9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1ce9-133">C#</span><span class="sxs-lookup"><span data-stu-id="d1ce9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1ce9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1ce9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1ce9-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d1ce9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d1ce9-136">Java</span><span class="sxs-lookup"><span data-stu-id="d1ce9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d1ce9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1ce9-137">Response</span></span>
<span data-ttu-id="d1ce9-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-138">The following is an example of the response.</span></span> 

><span data-ttu-id="d1ce9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1ce9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
