---
title: Получение educationSchool
description: Получение свойств и связей объекта school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 98a68ad8ab85c9d798fd41cf497413ed314e472b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887747"
---
# <a name="get-educationschool"></a><span data-ttu-id="39264-103">Получение educationSchool</span><span class="sxs-lookup"><span data-stu-id="39264-103">Get educationSchool</span></span>

<span data-ttu-id="39264-104">Получение свойств и связей объекта school.</span><span class="sxs-lookup"><span data-stu-id="39264-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39264-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39264-105">Permissions</span></span>
<span data-ttu-id="39264-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39264-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39264-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39264-108">Permission type</span></span>      | <span data-ttu-id="39264-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39264-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39264-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39264-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="39264-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="39264-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="39264-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39264-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="39264-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39264-113">Not supported.</span></span>  |
|<span data-ttu-id="39264-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39264-114">Application</span></span> | <span data-ttu-id="39264-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39264-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="39264-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39264-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="39264-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="39264-117">Optional query parameters</span></span>
<span data-ttu-id="39264-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="39264-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39264-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39264-119">Request headers</span></span>
| <span data-ttu-id="39264-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39264-120">Header</span></span>       | <span data-ttu-id="39264-121">Значение</span><span class="sxs-lookup"><span data-stu-id="39264-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="39264-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39264-122">Authorization</span></span>  | <span data-ttu-id="39264-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39264-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39264-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39264-125">Request body</span></span>
<span data-ttu-id="39264-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39264-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="39264-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="39264-127">Response</span></span>
<span data-ttu-id="39264-128">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="39264-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39264-129">Пример</span><span class="sxs-lookup"><span data-stu-id="39264-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39264-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="39264-130">Request</span></span>
<span data-ttu-id="39264-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39264-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="39264-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="39264-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="39264-133">C#</span><span class="sxs-lookup"><span data-stu-id="39264-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39264-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="39264-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="39264-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="39264-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="39264-136">Java</span><span class="sxs-lookup"><span data-stu-id="39264-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="39264-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="39264-137">Response</span></span>
<span data-ttu-id="39264-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39264-138">The following is an example of the response.</span></span> 

><span data-ttu-id="39264-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39264-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
