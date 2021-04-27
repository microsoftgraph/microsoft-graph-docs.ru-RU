---
title: Создание educationSchool
description: Создание учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0f4d91dc8756f74551a374151946d192ecf18b27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043647"
---
# <a name="create-educationschool"></a><span data-ttu-id="de66c-103">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="de66c-103">Create educationSchool</span></span>

<span data-ttu-id="de66c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de66c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de66c-105">Создание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="de66c-105">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="de66c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de66c-106">Permissions</span></span>

<span data-ttu-id="de66c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de66c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de66c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de66c-109">Permission type</span></span>                        | <span data-ttu-id="de66c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de66c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="de66c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de66c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de66c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de66c-112">Not supported.</span></span>                              |
| <span data-ttu-id="de66c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de66c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de66c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de66c-114">Not supported.</span></span>                              |
| <span data-ttu-id="de66c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de66c-115">Application</span></span>                            | <span data-ttu-id="de66c-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de66c-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="de66c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de66c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="de66c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de66c-118">Request headers</span></span>

| <span data-ttu-id="de66c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de66c-119">Header</span></span>        | <span data-ttu-id="de66c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="de66c-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="de66c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de66c-121">Authorization</span></span> | <span data-ttu-id="de66c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de66c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de66c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de66c-124">Content-Type</span></span>  | <span data-ttu-id="de66c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de66c-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="de66c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de66c-126">Request body</span></span>

<span data-ttu-id="de66c-127">В теле запроса предоставьте описание объекта [educationSchool](../resources/educationschool.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de66c-127">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="de66c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="de66c-128">Response</span></span>

<span data-ttu-id="de66c-129">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="de66c-129">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de66c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="de66c-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="de66c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="de66c-131">Request</span></span>

<span data-ttu-id="de66c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de66c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de66c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="de66c-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools
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

# <a name="c"></a>[<span data-ttu-id="de66c-134">C#</span><span class="sxs-lookup"><span data-stu-id="de66c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de66c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de66c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de66c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de66c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de66c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="de66c-137">Response</span></span>

<span data-ttu-id="de66c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="de66c-138">The following is an example of the response.</span></span>

><span data-ttu-id="de66c-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de66c-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


