---
title: Создание educationUser
description: Создание пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eae920389cf0336161ef755aed1da62a72e7bcb1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053134"
---
# <a name="create-educationuser"></a><span data-ttu-id="fe293-103">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="fe293-103">Create educationUser</span></span>

<span data-ttu-id="fe293-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe293-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe293-105">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="fe293-105">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="fe293-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe293-106">Permissions</span></span>
<span data-ttu-id="fe293-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe293-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe293-109">Permission type</span></span>      | <span data-ttu-id="fe293-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe293-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe293-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe293-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="fe293-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe293-112">Not supported.</span></span>  |
|<span data-ttu-id="fe293-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe293-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fe293-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe293-114">Not supported.</span></span>  |
|<span data-ttu-id="fe293-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe293-115">Application</span></span> | <span data-ttu-id="fe293-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe293-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fe293-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe293-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="fe293-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe293-118">Request headers</span></span>
| <span data-ttu-id="fe293-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe293-119">Header</span></span>       | <span data-ttu-id="fe293-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fe293-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe293-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe293-121">Authorization</span></span>  | <span data-ttu-id="fe293-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe293-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe293-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe293-124">Content-Type</span></span>  | <span data-ttu-id="fe293-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe293-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe293-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe293-126">Request body</span></span>
<span data-ttu-id="fe293-127">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe293-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="fe293-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe293-128">Response</span></span>
<span data-ttu-id="fe293-129">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fe293-129">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe293-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fe293-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe293-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe293-131">Request</span></span>
<span data-ttu-id="fe293-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe293-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe293-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe293-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fe293-134">C#</span><span class="sxs-lookup"><span data-stu-id="fe293-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe293-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe293-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe293-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe293-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe293-137">Java</span><span class="sxs-lookup"><span data-stu-id="fe293-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fe293-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe293-138">Response</span></span>
<span data-ttu-id="fe293-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fe293-139">The following is an example of the response.</span></span> 

><span data-ttu-id="fe293-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fe293-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->

