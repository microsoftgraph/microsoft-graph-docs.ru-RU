---
title: Получение educationSchool
description: Получение свойств и связей объекта school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a845fc4cfc5390e9af50002479dd03afc00173af
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401337"
---
# <a name="get-educationschool"></a><span data-ttu-id="95bb2-103">Получение educationSchool</span><span class="sxs-lookup"><span data-stu-id="95bb2-103">Get educationSchool</span></span>

<span data-ttu-id="95bb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95bb2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95bb2-105">Получение свойств и связей объекта school.</span><span class="sxs-lookup"><span data-stu-id="95bb2-105">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95bb2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95bb2-106">Permissions</span></span>
<span data-ttu-id="95bb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95bb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95bb2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95bb2-109">Permission type</span></span>      | <span data-ttu-id="95bb2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95bb2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95bb2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95bb2-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="95bb2-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="95bb2-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="95bb2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95bb2-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="95bb2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95bb2-114">Not supported.</span></span>  |
|<span data-ttu-id="95bb2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95bb2-115">Application</span></span> | <span data-ttu-id="95bb2-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95bb2-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="95bb2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95bb2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95bb2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="95bb2-118">Optional query parameters</span></span>
<span data-ttu-id="95bb2-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="95bb2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95bb2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95bb2-120">Request headers</span></span>
| <span data-ttu-id="95bb2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95bb2-121">Header</span></span>       | <span data-ttu-id="95bb2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="95bb2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95bb2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95bb2-123">Authorization</span></span>  | <span data-ttu-id="95bb2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95bb2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95bb2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95bb2-126">Request body</span></span>
<span data-ttu-id="95bb2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95bb2-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="95bb2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="95bb2-128">Response</span></span>
<span data-ttu-id="95bb2-129">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95bb2-129">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95bb2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="95bb2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95bb2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="95bb2-131">Request</span></span>
<span data-ttu-id="95bb2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95bb2-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95bb2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="95bb2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="c"></a>[<span data-ttu-id="95bb2-134">C#</span><span class="sxs-lookup"><span data-stu-id="95bb2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95bb2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95bb2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95bb2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95bb2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95bb2-137">Java</span><span class="sxs-lookup"><span data-stu-id="95bb2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="95bb2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="95bb2-138">Response</span></span>
<span data-ttu-id="95bb2-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="95bb2-139">The following is an example of the response.</span></span> 

><span data-ttu-id="95bb2-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95bb2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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