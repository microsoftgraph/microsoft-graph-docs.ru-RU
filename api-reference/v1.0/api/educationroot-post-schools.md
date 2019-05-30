---
title: Создание educationSchool
description: Создание учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 085392ae1829769f15213c0ac8360d8da3910b70
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537186"
---
# <a name="create-educationschool"></a><span data-ttu-id="191b2-103">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="191b2-103">Create educationSchool</span></span>

<span data-ttu-id="191b2-104">Создание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="191b2-104">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="191b2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="191b2-105">Permissions</span></span>
<span data-ttu-id="191b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="191b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="191b2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="191b2-108">Permission type</span></span>      | <span data-ttu-id="191b2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="191b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="191b2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="191b2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="191b2-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="191b2-111">Not supported.</span></span>  |
|<span data-ttu-id="191b2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="191b2-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="191b2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="191b2-113">Not supported.</span></span>  |
|<span data-ttu-id="191b2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="191b2-114">Application</span></span> | <span data-ttu-id="191b2-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="191b2-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="191b2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="191b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="191b2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="191b2-117">Request headers</span></span>
| <span data-ttu-id="191b2-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="191b2-118">Header</span></span>       | <span data-ttu-id="191b2-119">Значение</span><span class="sxs-lookup"><span data-stu-id="191b2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="191b2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="191b2-120">Authorization</span></span>  | <span data-ttu-id="191b2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="191b2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="191b2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="191b2-123">Content-Type</span></span>  | <span data-ttu-id="191b2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="191b2-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="191b2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="191b2-125">Request body</span></span>
<span data-ttu-id="191b2-126">В теле запроса предоставьте описание объекта [educationSchool](../resources/educationschool.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="191b2-126">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="191b2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="191b2-127">Response</span></span>
<span data-ttu-id="191b2-128">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="191b2-128">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="191b2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="191b2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="191b2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="191b2-130">Request</span></span>
<span data-ttu-id="191b2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="191b2-131">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="191b2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="191b2-132">Response</span></span>
<span data-ttu-id="191b2-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="191b2-133">The following is an example of the response.</span></span> 

><span data-ttu-id="191b2-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="191b2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="191b2-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="191b2-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="191b2-137">C#</span><span class="sxs-lookup"><span data-stu-id="191b2-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_educationschool_from_educationroot-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="191b2-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="191b2-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationschool_from_educationroot-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationroot-post-schools.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationroot-post-schools.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
