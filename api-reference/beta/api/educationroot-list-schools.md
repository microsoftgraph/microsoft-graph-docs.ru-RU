---
title: Перечисление educationSchools
description: Получение списка всех объектов school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 304d9191cfb300b03e45c00b5caad2f516ca4501
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323978"
---
# <a name="list-educationschools"></a><span data-ttu-id="c1d49-103">Перечисление educationSchools</span><span class="sxs-lookup"><span data-stu-id="c1d49-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1d49-104">Получение списка всех объектов school.</span><span class="sxs-lookup"><span data-stu-id="c1d49-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1d49-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1d49-105">Permissions</span></span>
<span data-ttu-id="c1d49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1d49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1d49-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1d49-108">Permission type</span></span>      | <span data-ttu-id="c1d49-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1d49-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1d49-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1d49-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c1d49-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c1d49-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c1d49-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1d49-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c1d49-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1d49-113">Not supported.</span></span>  |
|<span data-ttu-id="c1d49-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1d49-114">Application</span></span> | <span data-ttu-id="c1d49-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1d49-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c1d49-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1d49-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http GET /education/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1d49-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c1d49-117">Optional query parameters</span></span>
<span data-ttu-id="c1d49-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c1d49-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1d49-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1d49-119">Request headers</span></span>
| <span data-ttu-id="c1d49-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1d49-120">Header</span></span>       | <span data-ttu-id="c1d49-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c1d49-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1d49-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1d49-122">Authorization</span></span>  | <span data-ttu-id="c1d49-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1d49-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1d49-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1d49-125">Request body</span></span>
<span data-ttu-id="c1d49-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1d49-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c1d49-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1d49-127">Response</span></span>
<span data-ttu-id="c1d49-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1d49-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1d49-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c1d49-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1d49-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1d49-130">Request</span></span>
<span data-ttu-id="c1d49-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1d49-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1d49-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1d49-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1d49-133">C#</span><span class="sxs-lookup"><span data-stu-id="c1d49-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1d49-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1d49-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1d49-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c1d49-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c1d49-136">Java</span><span class="sxs-lookup"><span data-stu-id="c1d49-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1d49-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1d49-137">Response</span></span>
<span data-ttu-id="c1d49-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1d49-138">The following is an example of the response.</span></span> 

><span data-ttu-id="c1d49-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1d49-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
