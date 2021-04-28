---
title: Перечисление учебных заведений
description: Получение списка учебных заведений, в которых доступен этот курс.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 477f6fa46d765020d43540e5ed5ddbbb950beae8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050502"
---
# <a name="list-schools"></a><span data-ttu-id="a248a-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="a248a-103">List schools</span></span>

<span data-ttu-id="a248a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a248a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a248a-105">Получение списка учебных заведений, в которых доступен этот курс.</span><span class="sxs-lookup"><span data-stu-id="a248a-105">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="a248a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a248a-106">Permissions</span></span>

<span data-ttu-id="a248a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a248a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a248a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a248a-109">Permission type</span></span>                        | <span data-ttu-id="a248a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a248a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a248a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a248a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a248a-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a248a-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="a248a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a248a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a248a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a248a-114">Not supported</span></span>                               |
| <span data-ttu-id="a248a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a248a-115">Application</span></span>                            | <span data-ttu-id="a248a-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a248a-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a248a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a248a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a248a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a248a-118">Optional query parameters</span></span>

<span data-ttu-id="a248a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a248a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a248a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a248a-120">Request headers</span></span>

| <span data-ttu-id="a248a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a248a-121">Header</span></span>        | <span data-ttu-id="a248a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a248a-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a248a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a248a-123">Authorization</span></span> | <span data-ttu-id="a248a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a248a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a248a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a248a-126">Request body</span></span>

<span data-ttu-id="a248a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a248a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a248a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a248a-128">Response</span></span>

<span data-ttu-id="a248a-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a248a-129">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a248a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a248a-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a248a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a248a-131">Request</span></span>

<span data-ttu-id="a248a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a248a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a248a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a248a-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/schools
```

# <a name="c"></a>[<span data-ttu-id="a248a-134">C#</span><span class="sxs-lookup"><span data-stu-id="a248a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a248a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a248a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a248a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a248a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a248a-137">Java</span><span class="sxs-lookup"><span data-stu-id="a248a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a248a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a248a-138">Response</span></span>

<span data-ttu-id="a248a-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a248a-139">The following is an example of the response.</span></span>

><span data-ttu-id="a248a-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a248a-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
