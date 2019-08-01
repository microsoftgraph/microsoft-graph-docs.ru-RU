---
title: Создание educationUser
description: Создание пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e98261776d967c93a94ecf30afa57bc5e1d97381
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015210"
---
# <a name="create-educationuser"></a><span data-ttu-id="97ade-103">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="97ade-103">Create educationUser</span></span>

<span data-ttu-id="97ade-104">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="97ade-104">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="97ade-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97ade-105">Permissions</span></span>
<span data-ttu-id="97ade-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97ade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97ade-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97ade-108">Permission type</span></span>      | <span data-ttu-id="97ade-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97ade-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97ade-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97ade-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="97ade-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97ade-111">Not supported.</span></span>  |
|<span data-ttu-id="97ade-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97ade-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="97ade-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97ade-113">Not supported.</span></span>  |
|<span data-ttu-id="97ade-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97ade-114">Application</span></span> | <span data-ttu-id="97ade-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97ade-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="97ade-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97ade-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="97ade-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97ade-117">Request headers</span></span>
| <span data-ttu-id="97ade-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97ade-118">Header</span></span>       | <span data-ttu-id="97ade-119">Значение</span><span class="sxs-lookup"><span data-stu-id="97ade-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97ade-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97ade-120">Authorization</span></span>  | <span data-ttu-id="97ade-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97ade-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97ade-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97ade-123">Content-Type</span></span>  | <span data-ttu-id="97ade-124">application/json</span><span class="sxs-lookup"><span data-stu-id="97ade-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97ade-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97ade-125">Request body</span></span>
<span data-ttu-id="97ade-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97ade-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="97ade-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="97ade-127">Response</span></span>
<span data-ttu-id="97ade-128">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="97ade-128">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97ade-129">Пример</span><span class="sxs-lookup"><span data-stu-id="97ade-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97ade-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="97ade-130">Request</span></span>
<span data-ttu-id="97ade-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97ade-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="97ade-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="97ade-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="97ade-133">C#</span><span class="sxs-lookup"><span data-stu-id="97ade-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97ade-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="97ade-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97ade-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="97ade-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97ade-136">Java</span><span class="sxs-lookup"><span data-stu-id="97ade-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="97ade-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="97ade-137">Response</span></span>
<span data-ttu-id="97ade-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97ade-138">The following is an example of the response.</span></span> 

><span data-ttu-id="97ade-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97ade-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
