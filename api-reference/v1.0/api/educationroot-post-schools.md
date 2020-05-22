---
title: Создание educationSchool
description: Создание учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1f3c35e04dddaa5f9b1e8e22ec5173d553f3332f
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345753"
---
# <a name="create-educationschool"></a><span data-ttu-id="ef41b-103">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="ef41b-103">Create educationSchool</span></span>

<span data-ttu-id="ef41b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef41b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef41b-105">Создание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ef41b-105">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef41b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef41b-106">Permissions</span></span>

<span data-ttu-id="ef41b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef41b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef41b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef41b-109">Permission type</span></span>                        | <span data-ttu-id="ef41b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef41b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ef41b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef41b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef41b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef41b-112">Not supported.</span></span>                              |
| <span data-ttu-id="ef41b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef41b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef41b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef41b-114">Not supported.</span></span>                              |
| <span data-ttu-id="ef41b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef41b-115">Application</span></span>                            | <span data-ttu-id="ef41b-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef41b-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="ef41b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef41b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="ef41b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef41b-118">Request headers</span></span>

| <span data-ttu-id="ef41b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef41b-119">Header</span></span>        | <span data-ttu-id="ef41b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ef41b-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ef41b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef41b-121">Authorization</span></span> | <span data-ttu-id="ef41b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef41b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef41b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef41b-124">Content-Type</span></span>  | <span data-ttu-id="ef41b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef41b-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="ef41b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef41b-126">Request body</span></span>

<span data-ttu-id="ef41b-127">В теле запроса предоставьте описание объекта [educationSchool](../resources/educationschool.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef41b-127">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ef41b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef41b-128">Response</span></span>

<span data-ttu-id="ef41b-129">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ef41b-129">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef41b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ef41b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ef41b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef41b-131">Request</span></span>

<span data-ttu-id="ef41b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef41b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef41b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef41b-133">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="ef41b-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef41b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef41b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef41b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef41b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef41b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef41b-137">Java</span><span class="sxs-lookup"><span data-stu-id="ef41b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ef41b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef41b-138">Response</span></span>

<span data-ttu-id="ef41b-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef41b-139">The following is an example of the response.</span></span>

><span data-ttu-id="ef41b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef41b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
