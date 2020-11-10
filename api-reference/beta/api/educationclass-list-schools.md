---
title: Перечисление учебных заведений
description: Получение списка учебных заведений, в которых доступен этот курс.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d46b01619272b390346da8fd4afc5171669e1cca
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966259"
---
# <a name="list-schools"></a><span data-ttu-id="22cad-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="22cad-103">List schools</span></span>

<span data-ttu-id="22cad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22cad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22cad-105">Получение списка учебных заведений, в которых доступен этот курс.</span><span class="sxs-lookup"><span data-stu-id="22cad-105">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="22cad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22cad-106">Permissions</span></span>

<span data-ttu-id="22cad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22cad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22cad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22cad-109">Permission type</span></span>                        | <span data-ttu-id="22cad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22cad-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="22cad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22cad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22cad-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="22cad-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="22cad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22cad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22cad-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="22cad-114">Not supported</span></span>                               |
| <span data-ttu-id="22cad-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="22cad-115">Application</span></span>                            | <span data-ttu-id="22cad-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22cad-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22cad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22cad-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22cad-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22cad-118">Optional query parameters</span></span>

<span data-ttu-id="22cad-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22cad-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22cad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22cad-120">Request headers</span></span>

| <span data-ttu-id="22cad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22cad-121">Header</span></span>        | <span data-ttu-id="22cad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22cad-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="22cad-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22cad-123">Authorization</span></span> | <span data-ttu-id="22cad-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22cad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22cad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22cad-126">Request body</span></span>

<span data-ttu-id="22cad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22cad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22cad-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="22cad-128">Response</span></span>

<span data-ttu-id="22cad-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="22cad-129">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22cad-130">Пример</span><span class="sxs-lookup"><span data-stu-id="22cad-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="22cad-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="22cad-131">Request</span></span>

<span data-ttu-id="22cad-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22cad-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22cad-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22cad-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11014/schools
```

# <a name="c"></a>[<span data-ttu-id="22cad-134">C#</span><span class="sxs-lookup"><span data-stu-id="22cad-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22cad-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22cad-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22cad-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22cad-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22cad-137">Java</span><span class="sxs-lookup"><span data-stu-id="22cad-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="22cad-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="22cad-138">Response</span></span>

<span data-ttu-id="22cad-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22cad-139">The following is an example of the response.</span></span>

><span data-ttu-id="22cad-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22cad-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
