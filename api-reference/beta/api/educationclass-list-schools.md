---
title: Перечисление учебных заведений
description: Получение списка учебных заведений, в которых доступен этот курс.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 134b073e91136d1bd308b488db974f59140cb2dc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588166"
---
# <a name="list-schools"></a><span data-ttu-id="5ffbc-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="5ffbc-103">List schools</span></span>

<span data-ttu-id="5ffbc-104">Получение списка учебных заведений, в которых доступен этот курс.</span><span class="sxs-lookup"><span data-stu-id="5ffbc-104">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ffbc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ffbc-105">Permissions</span></span>
<span data-ttu-id="5ffbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ffbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ffbc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ffbc-108">Permission type</span></span>      | <span data-ttu-id="5ffbc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ffbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ffbc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ffbc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5ffbc-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5ffbc-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="5ffbc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ffbc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5ffbc-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5ffbc-113">Not supported</span></span>  |
|<span data-ttu-id="5ffbc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ffbc-114">Application</span></span> | <span data-ttu-id="5ffbc-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ffbc-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5ffbc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ffbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5ffbc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ffbc-117">Optional query parameters</span></span>
<span data-ttu-id="5ffbc-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ffbc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ffbc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ffbc-119">Request headers</span></span>
| <span data-ttu-id="5ffbc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ffbc-120">Header</span></span>       | <span data-ttu-id="5ffbc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5ffbc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ffbc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ffbc-122">Authorization</span></span>  | <span data-ttu-id="5ffbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ffbc-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="5ffbc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ffbc-125">Request body</span></span>
<span data-ttu-id="5ffbc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ffbc-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5ffbc-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ffbc-127">Response</span></span>
<span data-ttu-id="5ffbc-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5ffbc-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ffbc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5ffbc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ffbc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ffbc-130">Request</span></span>
<span data-ttu-id="5ffbc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ffbc-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/schools
```
##### <a name="response"></a><span data-ttu-id="5ffbc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ffbc-132">Response</span></span>
<span data-ttu-id="5ffbc-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5ffbc-133">The following is an example of the response.</span></span> 

><span data-ttu-id="5ffbc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ffbc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
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
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5ffbc-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5ffbc-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5ffbc-137">Языках</span><span class="sxs-lookup"><span data-stu-id="5ffbc-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_schools-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ffbc-138">Язык</span><span class="sxs-lookup"><span data-stu-id="5ffbc-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_schools-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-list-schools.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-list-schools.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
