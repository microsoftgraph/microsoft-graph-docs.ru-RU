---
title: Получение educationSchool
description: Получение свойств и связей объекта school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a44d447c927ce4a7a32fc5de892e82f3eea0204c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726902"
---
# <a name="get-educationschool"></a><span data-ttu-id="1682e-103">Получение educationSchool</span><span class="sxs-lookup"><span data-stu-id="1682e-103">Get educationSchool</span></span>

<span data-ttu-id="1682e-104">Получение свойств и связей объекта school.</span><span class="sxs-lookup"><span data-stu-id="1682e-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1682e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1682e-105">Permissions</span></span>
<span data-ttu-id="1682e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1682e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1682e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1682e-108">Permission type</span></span>      | <span data-ttu-id="1682e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1682e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1682e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1682e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1682e-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="1682e-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="1682e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1682e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1682e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1682e-113">Not supported.</span></span>  |
|<span data-ttu-id="1682e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1682e-114">Application</span></span> | <span data-ttu-id="1682e-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1682e-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1682e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1682e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1682e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1682e-117">Optional query parameters</span></span>
<span data-ttu-id="1682e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1682e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1682e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1682e-119">Request headers</span></span>
| <span data-ttu-id="1682e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1682e-120">Header</span></span>       | <span data-ttu-id="1682e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1682e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1682e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1682e-122">Authorization</span></span>  | <span data-ttu-id="1682e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1682e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1682e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1682e-125">Request body</span></span>
<span data-ttu-id="1682e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1682e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1682e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1682e-127">Response</span></span>
<span data-ttu-id="1682e-128">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1682e-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1682e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1682e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1682e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1682e-130">Request</span></span>
<span data-ttu-id="1682e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1682e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1682e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1682e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1682e-133">C#</span><span class="sxs-lookup"><span data-stu-id="1682e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1682e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1682e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1682e-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1682e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1682e-136">Java</span><span class="sxs-lookup"><span data-stu-id="1682e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1682e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1682e-137">Response</span></span>
<span data-ttu-id="1682e-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1682e-138">The following is an example of the response.</span></span> 

><span data-ttu-id="1682e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1682e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "principalEmail": "AmyRoebuck@contoso.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
