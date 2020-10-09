---
title: Перечисление educationSchools
description: Получение списка всех объектов school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9a9cac76b5b59cffcd535e4f7ff96dc78bc3e657
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403467"
---
# <a name="list-educationschools"></a><span data-ttu-id="6be0c-103">Перечисление educationSchools</span><span class="sxs-lookup"><span data-stu-id="6be0c-103">List educationSchools</span></span>

<span data-ttu-id="6be0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6be0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6be0c-105">Получение списка всех объектов school.</span><span class="sxs-lookup"><span data-stu-id="6be0c-105">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6be0c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6be0c-106">Permissions</span></span>

<span data-ttu-id="6be0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6be0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6be0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6be0c-109">Permission type</span></span>                        | <span data-ttu-id="6be0c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6be0c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6be0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6be0c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6be0c-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="6be0c-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="6be0c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6be0c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6be0c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be0c-114">Not supported.</span></span>                              |
| <span data-ttu-id="6be0c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6be0c-115">Application</span></span>                            | <span data-ttu-id="6be0c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6be0c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6be0c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6be0c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http 
GET /education/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6be0c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6be0c-118">Optional query parameters</span></span>

<span data-ttu-id="6be0c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6be0c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6be0c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6be0c-120">Request headers</span></span>

| <span data-ttu-id="6be0c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6be0c-121">Header</span></span>        | <span data-ttu-id="6be0c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6be0c-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6be0c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6be0c-123">Authorization</span></span> | <span data-ttu-id="6be0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6be0c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6be0c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6be0c-126">Request body</span></span>

<span data-ttu-id="6be0c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6be0c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6be0c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6be0c-128">Response</span></span>

<span data-ttu-id="6be0c-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6be0c-129">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6be0c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6be0c-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6be0c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6be0c-131">Request</span></span>

<span data-ttu-id="6be0c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6be0c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6be0c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6be0c-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools
```

# <a name="c"></a>[<span data-ttu-id="6be0c-134">C#</span><span class="sxs-lookup"><span data-stu-id="6be0c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6be0c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6be0c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6be0c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6be0c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6be0c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6be0c-137">Response</span></span>

<span data-ttu-id="6be0c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6be0c-138">The following is an example of the response.</span></span>

><span data-ttu-id="6be0c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6be0c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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