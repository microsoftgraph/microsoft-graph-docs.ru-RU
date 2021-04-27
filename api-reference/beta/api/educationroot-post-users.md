---
title: Создание educationUser
description: Создание пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 18ced2a58fa4974ddca18bfc5b31d3e5e39fb46c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043586"
---
# <a name="create-educationuser"></a><span data-ttu-id="18dbb-103">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="18dbb-103">Create educationUser</span></span>

<span data-ttu-id="18dbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18dbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18dbb-105">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="18dbb-105">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="18dbb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18dbb-106">Permissions</span></span>
<span data-ttu-id="18dbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18dbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18dbb-109">Permission type</span></span>      | <span data-ttu-id="18dbb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18dbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18dbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18dbb-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="18dbb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18dbb-112">Not supported.</span></span>  |
|<span data-ttu-id="18dbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18dbb-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="18dbb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18dbb-114">Not supported.</span></span>  |
|<span data-ttu-id="18dbb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18dbb-115">Application</span></span> | <span data-ttu-id="18dbb-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18dbb-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="18dbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18dbb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="18dbb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18dbb-118">Request headers</span></span>
| <span data-ttu-id="18dbb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18dbb-119">Header</span></span>       | <span data-ttu-id="18dbb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="18dbb-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18dbb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18dbb-121">Authorization</span></span>  | <span data-ttu-id="18dbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18dbb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18dbb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18dbb-124">Content-Type</span></span>  | <span data-ttu-id="18dbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18dbb-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18dbb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18dbb-126">Request body</span></span>
<span data-ttu-id="18dbb-127">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18dbb-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="18dbb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="18dbb-128">Response</span></span>
<span data-ttu-id="18dbb-129">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18dbb-129">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18dbb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="18dbb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18dbb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="18dbb-131">Request</span></span>
<span data-ttu-id="18dbb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18dbb-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18dbb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="18dbb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/users
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
# <a name="c"></a>[<span data-ttu-id="18dbb-134">C#</span><span class="sxs-lookup"><span data-stu-id="18dbb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18dbb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18dbb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18dbb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18dbb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18dbb-137">Java</span><span class="sxs-lookup"><span data-stu-id="18dbb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="18dbb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="18dbb-138">Response</span></span>
<span data-ttu-id="18dbb-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18dbb-139">The following is an example of the response.</span></span> 

><span data-ttu-id="18dbb-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="18dbb-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


