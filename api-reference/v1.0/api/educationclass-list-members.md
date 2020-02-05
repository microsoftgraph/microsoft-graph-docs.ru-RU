---
title: Список участников
description: Получает преподавателей и учащихся для курса. Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 018cecb780cd5ebcb37b742f662d383213ccd7b1
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774524"
---
# <a name="list-members"></a><span data-ttu-id="9c5b0-104">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="9c5b0-104">List members</span></span>

<span data-ttu-id="9c5b0-105">Получает преподавателей и учащихся для курса.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="9c5b0-106">Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c5b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c5b0-107">Permissions</span></span>
<span data-ttu-id="9c5b0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c5b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c5b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c5b0-110">Permission type</span></span>      | <span data-ttu-id="9c5b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c5b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c5b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c5b0-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="9c5b0-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="9c5b0-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="9c5b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c5b0-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9c5b0-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9c5b0-115">Not supported</span></span>  |
|<span data-ttu-id="9c5b0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c5b0-116">Application</span></span> | <span data-ttu-id="9c5b0-117">EduRoster. Read. ALL, EduRoster. ReadWrite. ALL плюс Member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="9c5b0-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9c5b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c5b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c5b0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9c5b0-119">Optional query parameters</span></span>
<span data-ttu-id="9c5b0-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c5b0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c5b0-121">Request headers</span></span>
| <span data-ttu-id="9c5b0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c5b0-122">Header</span></span>       | <span data-ttu-id="9c5b0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9c5b0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c5b0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c5b0-124">Authorization</span></span>  | <span data-ttu-id="9c5b0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c5b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c5b0-127">Request body</span></span>
<span data-ttu-id="9c5b0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9c5b0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c5b0-129">Response</span></span>
<span data-ttu-id="9c5b0-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c5b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9c5b0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c5b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c5b0-132">Request</span></span>
<span data-ttu-id="9c5b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9c5b0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c5b0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9c5b0-135">C#</span><span class="sxs-lookup"><span data-stu-id="9c5b0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c5b0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c5b0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9c5b0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c5b0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9c5b0-138">Java</span><span class="sxs-lookup"><span data-stu-id="9c5b0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c5b0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c5b0-139">Response</span></span>
<span data-ttu-id="9c5b0-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-140">The following is an example of the response.</span></span> 

><span data-ttu-id="9c5b0-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c5b0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
