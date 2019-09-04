---
title: Получение educationUser
description: Получение свойств и связей пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 26aec1bbf7185c02309c9069008bda606d74c993
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720265"
---
# <a name="get-educationuser"></a><span data-ttu-id="0b174-103">Получение educationUser</span><span class="sxs-lookup"><span data-stu-id="0b174-103">Get educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b174-104">Получение свойств и связей пользователя.</span><span class="sxs-lookup"><span data-stu-id="0b174-104">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b174-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b174-105">Permissions</span></span>
<span data-ttu-id="0b174-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b174-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b174-108">Permission type</span></span>      | <span data-ttu-id="0b174-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b174-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b174-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b174-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0b174-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="0b174-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="0b174-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b174-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0b174-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b174-113">Not supported.</span></span>  |
|<span data-ttu-id="0b174-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b174-114">Application</span></span> | <span data-ttu-id="0b174-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b174-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="0b174-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b174-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b174-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b174-117">Optional query parameters</span></span>
<span data-ttu-id="0b174-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0b174-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b174-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b174-119">Request headers</span></span>
| <span data-ttu-id="0b174-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b174-120">Header</span></span>       | <span data-ttu-id="0b174-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0b174-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b174-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b174-122">Authorization</span></span>  | <span data-ttu-id="0b174-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b174-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b174-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b174-125">Request body</span></span>
<span data-ttu-id="0b174-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b174-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0b174-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b174-127">Response</span></span>
<span data-ttu-id="0b174-128">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b174-128">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b174-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0b174-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b174-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b174-130">Request</span></span>
<span data-ttu-id="0b174-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b174-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b174-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b174-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/13012
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b174-133">C#</span><span class="sxs-lookup"><span data-stu-id="0b174-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b174-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b174-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b174-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0b174-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b174-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b174-136">Response</span></span>
<span data-ttu-id="0b174-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b174-137">The following is an example of the response.</span></span> 

><span data-ttu-id="0b174-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b174-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
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
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
