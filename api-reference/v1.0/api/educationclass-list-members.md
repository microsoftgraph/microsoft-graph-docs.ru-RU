---
title: Перечисление участников
description: Получает преподавателей и учащихся для курса. Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.
ms.openlocfilehash: 8543f429fec359fe91275c8636e2eded686c9db5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027794"
---
# <a name="list-members"></a><span data-ttu-id="a87fb-104">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="a87fb-104">List members</span></span>

<span data-ttu-id="a87fb-105">Получает преподавателей и учащихся для курса.</span><span class="sxs-lookup"><span data-stu-id="a87fb-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="a87fb-106">Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.</span><span class="sxs-lookup"><span data-stu-id="a87fb-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="a87fb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a87fb-107">Permissions</span></span>
<span data-ttu-id="a87fb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a87fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a87fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a87fb-110">Permission type</span></span>      | <span data-ttu-id="a87fb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a87fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a87fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a87fb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a87fb-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a87fb-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a87fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a87fb-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a87fb-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a87fb-115">Not supported</span></span>  |
|<span data-ttu-id="a87fb-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a87fb-116">Application</span></span> | <span data-ttu-id="a87fb-117">EduRoster.Read.All, EduRoster.ReadWrite.All, а также Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="a87fb-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a87fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a87fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a87fb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a87fb-119">Optional query parameters</span></span>
<span data-ttu-id="a87fb-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a87fb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a87fb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a87fb-121">Request headers</span></span>
| <span data-ttu-id="a87fb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a87fb-122">Header</span></span>       | <span data-ttu-id="a87fb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a87fb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a87fb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a87fb-124">Authorization</span></span>  | <span data-ttu-id="a87fb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a87fb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a87fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a87fb-127">Request body</span></span>
<span data-ttu-id="a87fb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a87fb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a87fb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a87fb-129">Response</span></span>
<span data-ttu-id="a87fb-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a87fb-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a87fb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a87fb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a87fb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a87fb-132">Request</span></span>
<span data-ttu-id="a87fb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a87fb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
##### <a name="response"></a><span data-ttu-id="a87fb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a87fb-134">Response</span></span>
<span data-ttu-id="a87fb-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a87fb-135">The following is an example of the response.</span></span> 

><span data-ttu-id="a87fb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a87fb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
