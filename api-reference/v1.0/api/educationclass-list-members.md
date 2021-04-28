---
title: Список участников
description: Получает преподавателей и учащихся для курса. Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d24ada4c11aec3ceddac736146f8e70c4d9baf86
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048759"
---
# <a name="list-members"></a><span data-ttu-id="b9c58-104">Список участников</span><span class="sxs-lookup"><span data-stu-id="b9c58-104">List members</span></span>

<span data-ttu-id="b9c58-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c58-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9c58-106">Получает преподавателей и учащихся для курса.</span><span class="sxs-lookup"><span data-stu-id="b9c58-106">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="b9c58-107">Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.</span><span class="sxs-lookup"><span data-stu-id="b9c58-107">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9c58-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9c58-108">Permissions</span></span>
<span data-ttu-id="b9c58-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9c58-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9c58-111">Permission type</span></span>      | <span data-ttu-id="b9c58-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9c58-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9c58-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9c58-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9c58-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b9c58-114">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b9c58-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9c58-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b9c58-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b9c58-116">Not supported</span></span>  |
|<span data-ttu-id="b9c58-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9c58-117">Application</span></span> | <span data-ttu-id="b9c58-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="b9c58-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b9c58-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9c58-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9c58-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9c58-120">Optional query parameters</span></span>
<span data-ttu-id="b9c58-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b9c58-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9c58-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9c58-122">Request headers</span></span>
| <span data-ttu-id="b9c58-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9c58-123">Header</span></span>       | <span data-ttu-id="b9c58-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b9c58-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9c58-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9c58-125">Authorization</span></span>  | <span data-ttu-id="b9c58-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9c58-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9c58-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9c58-128">Request body</span></span>
<span data-ttu-id="b9c58-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9c58-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b9c58-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9c58-130">Response</span></span>
<span data-ttu-id="b9c58-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9c58-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9c58-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b9c58-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9c58-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9c58-133">Request</span></span>
<span data-ttu-id="b9c58-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9c58-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9c58-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9c58-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
# <a name="c"></a>[<span data-ttu-id="b9c58-136">C#</span><span class="sxs-lookup"><span data-stu-id="b9c58-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9c58-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9c58-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9c58-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9c58-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9c58-139">Java</span><span class="sxs-lookup"><span data-stu-id="b9c58-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9c58-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9c58-140">Response</span></span>
<span data-ttu-id="b9c58-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b9c58-141">The following is an example of the response.</span></span> 

><span data-ttu-id="b9c58-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b9c58-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
