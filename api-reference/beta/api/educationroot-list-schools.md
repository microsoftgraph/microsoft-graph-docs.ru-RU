---
title: Перечисление educationSchools
description: Получение списка всех объектов school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d719268a8b3e6ff044e928485449320b77bbeff4
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "37581217"
---
# <a name="list-educationschools"></a><span data-ttu-id="b74ad-103">Перечисление educationSchools</span><span class="sxs-lookup"><span data-stu-id="b74ad-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b74ad-104">Получение списка всех объектов school.</span><span class="sxs-lookup"><span data-stu-id="b74ad-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b74ad-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b74ad-105">Permissions</span></span>

<span data-ttu-id="b74ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b74ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b74ad-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b74ad-108">Permission type</span></span>                        | <span data-ttu-id="b74ad-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b74ad-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b74ad-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b74ad-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b74ad-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b74ad-111">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="b74ad-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b74ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b74ad-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b74ad-113">Not supported.</span></span>                              |
| <span data-ttu-id="b74ad-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b74ad-114">Application</span></span>                            | <span data-ttu-id="b74ad-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b74ad-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b74ad-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b74ad-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http GET /education/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b74ad-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b74ad-117">Optional query parameters</span></span>

<span data-ttu-id="b74ad-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b74ad-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b74ad-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b74ad-119">Request headers</span></span>

| <span data-ttu-id="b74ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b74ad-120">Header</span></span>        | <span data-ttu-id="b74ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b74ad-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="b74ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b74ad-122">Authorization</span></span> | <span data-ttu-id="b74ad-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b74ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b74ad-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b74ad-125">Request body</span></span>

<span data-ttu-id="b74ad-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b74ad-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b74ad-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b74ad-127">Response</span></span>

<span data-ttu-id="b74ad-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b74ad-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b74ad-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b74ad-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b74ad-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b74ad-130">Request</span></span>

<span data-ttu-id="b74ad-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b74ad-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b74ad-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b74ad-132">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="b74ad-133">C#</span><span class="sxs-lookup"><span data-stu-id="b74ad-133">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b74ad-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b74ad-134">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b74ad-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b74ad-135">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b74ad-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b74ad-136">Response</span></span>

<span data-ttu-id="b74ad-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b74ad-137">The following is an example of the response.</span></span>

><span data-ttu-id="b74ad-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b74ad-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
