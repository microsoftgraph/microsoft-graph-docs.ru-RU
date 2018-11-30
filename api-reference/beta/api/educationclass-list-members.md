---
title: Перечисление участников
description: Получает преподавателей и учащихся для курса. Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.
ms.openlocfilehash: e8f31720733fec3942d4ddb35fa7f2fdac1b26f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075339"
---
# <a name="list-members"></a><span data-ttu-id="648b5-104">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="648b5-104">List members</span></span>

> <span data-ttu-id="648b5-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="648b5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="648b5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="648b5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="648b5-107">Получает преподавателей и учащихся для курса.</span><span class="sxs-lookup"><span data-stu-id="648b5-107">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="648b5-108">Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.</span><span class="sxs-lookup"><span data-stu-id="648b5-108">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="648b5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="648b5-109">Permissions</span></span>
<span data-ttu-id="648b5-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="648b5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="648b5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="648b5-112">Permission type</span></span>      | <span data-ttu-id="648b5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="648b5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="648b5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="648b5-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="648b5-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="648b5-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="648b5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="648b5-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="648b5-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="648b5-117">Not supported</span></span>  |
|<span data-ttu-id="648b5-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="648b5-118">Application</span></span> | <span data-ttu-id="648b5-119">EduRoster.Read.All, EduRoster.ReadWrite.All, а также Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="648b5-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="648b5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="648b5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="648b5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="648b5-121">Optional query parameters</span></span>
<span data-ttu-id="648b5-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="648b5-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="648b5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="648b5-123">Request headers</span></span>
| <span data-ttu-id="648b5-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="648b5-124">Header</span></span>       | <span data-ttu-id="648b5-125">Значение</span><span class="sxs-lookup"><span data-stu-id="648b5-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="648b5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="648b5-126">Authorization</span></span>  | <span data-ttu-id="648b5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="648b5-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="648b5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="648b5-129">Request body</span></span>
<span data-ttu-id="648b5-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="648b5-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="648b5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="648b5-131">Response</span></span>
<span data-ttu-id="648b5-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="648b5-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="648b5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="648b5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="648b5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="648b5-134">Request</span></span>
<span data-ttu-id="648b5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="648b5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11016/members
```
##### <a name="response"></a><span data-ttu-id="648b5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="648b5-136">Response</span></span>
<span data-ttu-id="648b5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="648b5-137">The following is an example of the response.</span></span> 

><span data-ttu-id="648b5-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="648b5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
