---
title: Перечисление educationSchools
description: Получение списка всех объектов school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ecee29a46f6a03b15508963ef6f436122392a0bd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955287"
---
# <a name="list-educationschools"></a><span data-ttu-id="1929b-103">Перечисление educationSchools</span><span class="sxs-lookup"><span data-stu-id="1929b-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1929b-104">Получение списка всех объектов school.</span><span class="sxs-lookup"><span data-stu-id="1929b-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1929b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1929b-105">Permissions</span></span>
<span data-ttu-id="1929b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1929b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1929b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1929b-108">Permission type</span></span>      | <span data-ttu-id="1929b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1929b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1929b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1929b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1929b-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="1929b-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="1929b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1929b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1929b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1929b-113">Not supported.</span></span>  |
|<span data-ttu-id="1929b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1929b-114">Application</span></span> | <span data-ttu-id="1929b-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1929b-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1929b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1929b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http GET /education/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1929b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1929b-117">Optional query parameters</span></span>
<span data-ttu-id="1929b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1929b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1929b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1929b-119">Request headers</span></span>
| <span data-ttu-id="1929b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1929b-120">Header</span></span>       | <span data-ttu-id="1929b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1929b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1929b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1929b-122">Authorization</span></span>  | <span data-ttu-id="1929b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1929b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1929b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1929b-125">Request body</span></span>
<span data-ttu-id="1929b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1929b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1929b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1929b-127">Response</span></span>
<span data-ttu-id="1929b-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1929b-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1929b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1929b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1929b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1929b-130">Request</span></span>
<span data-ttu-id="1929b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1929b-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1929b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1929b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1929b-133">C#</span><span class="sxs-lookup"><span data-stu-id="1929b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1929b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1929b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1929b-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1929b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1929b-136">Java</span><span class="sxs-lookup"><span data-stu-id="1929b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1929b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1929b-137">Response</span></span>
<span data-ttu-id="1929b-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1929b-138">The following is an example of the response.</span></span> 

><span data-ttu-id="1929b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1929b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
