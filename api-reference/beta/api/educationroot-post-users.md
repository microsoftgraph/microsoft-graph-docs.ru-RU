---
title: Создание educationUser
description: Создание пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c228b476d9fb29853787fe7978877e6a89a090c2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441522"
---
# <a name="create-educationuser"></a><span data-ttu-id="d1551-103">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="d1551-103">Create educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1551-104">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="d1551-104">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="d1551-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1551-105">Permissions</span></span>
<span data-ttu-id="d1551-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1551-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1551-108">Permission type</span></span>      | <span data-ttu-id="d1551-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1551-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1551-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1551-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d1551-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1551-111">Not supported.</span></span>  |
|<span data-ttu-id="d1551-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1551-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d1551-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1551-113">Not supported.</span></span>  |
|<span data-ttu-id="d1551-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1551-114">Application</span></span> | <span data-ttu-id="d1551-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1551-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d1551-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1551-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="d1551-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1551-117">Request headers</span></span>
| <span data-ttu-id="d1551-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1551-118">Header</span></span>       | <span data-ttu-id="d1551-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d1551-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1551-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1551-120">Authorization</span></span>  | <span data-ttu-id="d1551-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1551-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d1551-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1551-123">Content-Type</span></span>  | <span data-ttu-id="d1551-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d1551-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1551-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1551-125">Request body</span></span>
<span data-ttu-id="d1551-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1551-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d1551-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1551-127">Response</span></span>
<span data-ttu-id="d1551-128">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d1551-128">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1551-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d1551-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1551-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1551-130">Request</span></span>
<span data-ttu-id="d1551-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1551-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d1551-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1551-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1551-133">C#</span><span class="sxs-lookup"><span data-stu-id="d1551-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1551-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1551-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1551-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d1551-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d1551-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1551-136">Response</span></span>
<span data-ttu-id="d1551-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1551-137">The following is an example of the response.</span></span> 

><span data-ttu-id="d1551-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1551-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
