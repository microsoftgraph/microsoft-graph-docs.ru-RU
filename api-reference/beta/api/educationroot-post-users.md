---
title: Создание educationUser
description: Создание пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 42da2ebdd8b5c2f71bff174b38e60508c85030c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426033"
---
# <a name="create-educationuser"></a><span data-ttu-id="aba16-103">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="aba16-103">Create educationUser</span></span>

<span data-ttu-id="aba16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aba16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aba16-105">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="aba16-105">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="aba16-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aba16-106">Permissions</span></span>
<span data-ttu-id="aba16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aba16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aba16-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aba16-109">Permission type</span></span>      | <span data-ttu-id="aba16-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aba16-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aba16-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aba16-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="aba16-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aba16-112">Not supported.</span></span>  |
|<span data-ttu-id="aba16-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aba16-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aba16-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aba16-114">Not supported.</span></span>  |
|<span data-ttu-id="aba16-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aba16-115">Application</span></span> | <span data-ttu-id="aba16-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aba16-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aba16-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aba16-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="aba16-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aba16-118">Request headers</span></span>
| <span data-ttu-id="aba16-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aba16-119">Header</span></span>       | <span data-ttu-id="aba16-120">Значение</span><span class="sxs-lookup"><span data-stu-id="aba16-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aba16-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aba16-121">Authorization</span></span>  | <span data-ttu-id="aba16-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aba16-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aba16-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aba16-124">Content-Type</span></span>  | <span data-ttu-id="aba16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aba16-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aba16-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aba16-126">Request body</span></span>
<span data-ttu-id="aba16-127">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aba16-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="aba16-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="aba16-128">Response</span></span>
<span data-ttu-id="aba16-129">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aba16-129">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aba16-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aba16-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aba16-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aba16-131">Request</span></span>
<span data-ttu-id="aba16-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aba16-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aba16-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aba16-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="aba16-134">C#</span><span class="sxs-lookup"><span data-stu-id="aba16-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aba16-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aba16-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aba16-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aba16-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aba16-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="aba16-137">Response</span></span>
<span data-ttu-id="aba16-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aba16-138">The following is an example of the response.</span></span> 

><span data-ttu-id="aba16-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aba16-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
