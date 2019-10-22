---
title: Создание educationSchool
description: Создание учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9f144c13bfb3973af96b10d78e69bb1c21ce09a7
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2019
ms.locfileid: "37553973"
---
# <a name="create-educationschool"></a><span data-ttu-id="1db7c-103">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="1db7c-103">Create educationSchool</span></span>

<span data-ttu-id="1db7c-104">Создание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1db7c-104">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="1db7c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1db7c-105">Permissions</span></span>

<span data-ttu-id="1db7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1db7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1db7c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1db7c-108">Permission type</span></span>                        | <span data-ttu-id="1db7c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1db7c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1db7c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1db7c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1db7c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1db7c-111">Not supported.</span></span>                              |
| <span data-ttu-id="1db7c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1db7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1db7c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1db7c-113">Not supported.</span></span>                              |
| <span data-ttu-id="1db7c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1db7c-114">Application</span></span>                            | <span data-ttu-id="1db7c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1db7c-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="1db7c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1db7c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="1db7c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1db7c-117">Request headers</span></span>

| <span data-ttu-id="1db7c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1db7c-118">Header</span></span>        | <span data-ttu-id="1db7c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1db7c-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="1db7c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1db7c-120">Authorization</span></span> | <span data-ttu-id="1db7c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1db7c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1db7c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1db7c-123">Content-Type</span></span>  | <span data-ttu-id="1db7c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1db7c-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="1db7c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1db7c-125">Request body</span></span>

<span data-ttu-id="1db7c-126">В теле запроса предоставьте описание объекта [educationSchool](../resources/educationschool.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1db7c-126">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1db7c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1db7c-127">Response</span></span>

<span data-ttu-id="1db7c-128">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1db7c-128">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1db7c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1db7c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1db7c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1db7c-130">Request</span></span>

<span data-ttu-id="1db7c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1db7c-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1db7c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1db7c-132">HTTP</span></span>](#tab/http)

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
  "phone": "+1 (253) 555-0102",
}
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="1db7c-133">C#</span><span class="sxs-lookup"><span data-stu-id="1db7c-133">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1db7c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1db7c-134">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1db7c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1db7c-135">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1db7c-136">Java</span><span class="sxs-lookup"><span data-stu-id="1db7c-136">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1db7c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1db7c-137">Response</span></span>

<span data-ttu-id="1db7c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1db7c-138">The following is an example of the response.</span></span>

><span data-ttu-id="1db7c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1db7c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
