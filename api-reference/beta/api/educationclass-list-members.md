---
title: Список участников
description: Получает преподавателей и учащихся для курса. Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: be51648f2a6f3549059eb5d0d69bb82198d53328
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259810"
---
# <a name="list-members"></a><span data-ttu-id="84e17-104">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="84e17-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84e17-105">Получает преподавателей и учащихся для курса.</span><span class="sxs-lookup"><span data-stu-id="84e17-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="84e17-106">Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.</span><span class="sxs-lookup"><span data-stu-id="84e17-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="84e17-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84e17-107">Permissions</span></span>
<span data-ttu-id="84e17-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84e17-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84e17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84e17-110">Permission type</span></span>      | <span data-ttu-id="84e17-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84e17-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84e17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84e17-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="84e17-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="84e17-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="84e17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84e17-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="84e17-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84e17-115">Not supported</span></span>  |
|<span data-ttu-id="84e17-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84e17-116">Application</span></span> | <span data-ttu-id="84e17-117">EduRoster. Read. ALL, EduRoster. ReadWrite. ALL плюс Member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="84e17-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="84e17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84e17-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84e17-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84e17-119">Optional query parameters</span></span>
<span data-ttu-id="84e17-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84e17-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84e17-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84e17-121">Request headers</span></span>
| <span data-ttu-id="84e17-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84e17-122">Header</span></span>       | <span data-ttu-id="84e17-123">Значение</span><span class="sxs-lookup"><span data-stu-id="84e17-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="84e17-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84e17-124">Authorization</span></span>  | <span data-ttu-id="84e17-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84e17-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84e17-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84e17-127">Request body</span></span>
<span data-ttu-id="84e17-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84e17-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="84e17-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="84e17-129">Response</span></span>
<span data-ttu-id="84e17-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="84e17-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84e17-131">Пример</span><span class="sxs-lookup"><span data-stu-id="84e17-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84e17-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="84e17-132">Request</span></span>
<span data-ttu-id="84e17-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84e17-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11016/members
```
##### <a name="response"></a><span data-ttu-id="84e17-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="84e17-134">Response</span></span>
<span data-ttu-id="84e17-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84e17-135">The following is an example of the response.</span></span> 

><span data-ttu-id="84e17-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84e17-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "externalId": "13013",
      "teacherNumber": "8802",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
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
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z",
      "gender": "female",
      "grade": "9",
      "graduationYear": "2019",
      "studentNumber": "13005",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="84e17-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="84e17-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="84e17-139">C#</span><span class="sxs-lookup"><span data-stu-id="84e17-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84e17-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="84e17-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="84e17-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84e17-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationclass-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationclass-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
