---
title: Перечисление учебных заведений
description: Получение списка учебных заведений для этого пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a2782a9a9b4fd3c27b6b694888994d6518ba402e
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "37581211"
---
# <a name="list-schools"></a><span data-ttu-id="ca3e8-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="ca3e8-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca3e8-104">Получение списка учебных заведений для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-104">Retrieve a list of schools for a user.</span></span>

>[!Note]
><span data-ttu-id="ca3e8-105">Если используется делегированный маркер, участники могут видеть только сведения о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-105">If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="ca3e8-106">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca3e8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca3e8-107">Permissions</span></span>

<span data-ttu-id="ca3e8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca3e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca3e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca3e8-110">Permission type</span></span>                        | <span data-ttu-id="ca3e8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca3e8-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ca3e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca3e8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca3e8-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ca3e8-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="ca3e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca3e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca3e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-115">Not supported.</span></span>                              |
| <span data-ttu-id="ca3e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca3e8-116">Application</span></span>                            | <span data-ttu-id="ca3e8-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca3e8-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca3e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca3e8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca3e8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca3e8-119">Optional query parameters</span></span>

<span data-ttu-id="ca3e8-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca3e8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca3e8-121">Request headers</span></span>

| <span data-ttu-id="ca3e8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca3e8-122">Header</span></span>        | <span data-ttu-id="ca3e8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ca3e8-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ca3e8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca3e8-124">Authorization</span></span> | <span data-ttu-id="ca3e8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca3e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca3e8-127">Request body</span></span>

<span data-ttu-id="ca3e8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca3e8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca3e8-129">Response</span></span>

<span data-ttu-id="ca3e8-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca3e8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ca3e8-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ca3e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca3e8-132">Request</span></span>

<span data-ttu-id="ca3e8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ca3e8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca3e8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ca3e8-135">C#</span><span class="sxs-lookup"><span data-stu-id="ca3e8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca3e8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca3e8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ca3e8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca3e8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ca3e8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca3e8-138">Response</span></span>

<span data-ttu-id="ca3e8-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-139">The following is an example of the response.</span></span>

><span data-ttu-id="ca3e8-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca3e8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
