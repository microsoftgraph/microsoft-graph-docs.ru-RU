---
title: Перечисление учебных заведений
description: Получение списка учебных заведений для этого пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 973412d50aef6e57ac9d985d9d6acee8af792d2b
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006809"
---
# <a name="list-schools"></a><span data-ttu-id="cb9d5-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="cb9d5-103">List schools</span></span>

<span data-ttu-id="cb9d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb9d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb9d5-105">Получение списка учебных заведений для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-105">Retrieve a list of schools for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb9d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb9d5-106">Permissions</span></span>

<span data-ttu-id="cb9d5-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cb9d5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb9d5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb9d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb9d5-109">Permission type</span></span>                        | <span data-ttu-id="cb9d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb9d5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cb9d5-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb9d5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb9d5-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="cb9d5-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="cb9d5-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb9d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb9d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-114">Not supported.</span></span>                              |
| <span data-ttu-id="cb9d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb9d5-115">Application</span></span>                            | <span data-ttu-id="cb9d5-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb9d5-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="cb9d5-117">При использовании делегированных разрешений возвращаются только те ресурсы educationSchool, которые является членом пользователя проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-117">When delegated permissions are used, only educationSchool resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="cb9d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb9d5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/schools
GET /education/users/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb9d5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb9d5-119">Optional query parameters</span></span>

<span data-ttu-id="cb9d5-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb9d5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb9d5-121">Request headers</span></span>

| <span data-ttu-id="cb9d5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb9d5-122">Header</span></span>        | <span data-ttu-id="cb9d5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cb9d5-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="cb9d5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb9d5-124">Authorization</span></span> | <span data-ttu-id="cb9d5-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-125">Bearer {token}.</span></span> <span data-ttu-id="cb9d5-126">Required.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb9d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb9d5-127">Request body</span></span>

<span data-ttu-id="cb9d5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb9d5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb9d5-129">Response</span></span>

<span data-ttu-id="cb9d5-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb9d5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cb9d5-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cb9d5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb9d5-132">Request</span></span>

<span data-ttu-id="cb9d5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb9d5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb9d5-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/schools
```

# <a name="c"></a>[<span data-ttu-id="cb9d5-135">C#</span><span class="sxs-lookup"><span data-stu-id="cb9d5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb9d5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb9d5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb9d5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb9d5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cb9d5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb9d5-138">Response</span></span>

<span data-ttu-id="cb9d5-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-139">The following is an example of the response.</span></span>

> <span data-ttu-id="cb9d5-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cb9d5-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="cb9d5-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
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
      "externalId": "10001",
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
