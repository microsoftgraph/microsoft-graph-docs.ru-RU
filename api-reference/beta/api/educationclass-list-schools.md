---
title: Перечисление учебных заведений
description: Получение списка учебных заведений, в которых доступен этот курс.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 3e63835e3595f4ebd27d6acf9065eda988a7083c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833686"
---
# <a name="list-schools"></a><span data-ttu-id="16021-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="16021-103">List schools</span></span>

> <span data-ttu-id="16021-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16021-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16021-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16021-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16021-106">Получение списка учебных заведений, в которых доступен этот курс.</span><span class="sxs-lookup"><span data-stu-id="16021-106">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="16021-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16021-107">Permissions</span></span>
<span data-ttu-id="16021-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16021-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16021-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16021-110">Permission type</span></span>      | <span data-ttu-id="16021-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16021-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16021-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16021-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="16021-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="16021-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="16021-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16021-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="16021-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="16021-115">Not supported</span></span>  |
|<span data-ttu-id="16021-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16021-116">Application</span></span> | <span data-ttu-id="16021-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16021-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="16021-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16021-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16021-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16021-119">Optional query parameters</span></span>
<span data-ttu-id="16021-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16021-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16021-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16021-121">Request headers</span></span>
| <span data-ttu-id="16021-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16021-122">Header</span></span>       | <span data-ttu-id="16021-123">Значение</span><span class="sxs-lookup"><span data-stu-id="16021-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16021-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16021-124">Authorization</span></span>  | <span data-ttu-id="16021-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16021-p103">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="16021-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16021-127">Request body</span></span>
<span data-ttu-id="16021-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16021-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="16021-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="16021-129">Response</span></span>
<span data-ttu-id="16021-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16021-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16021-131">Пример</span><span class="sxs-lookup"><span data-stu-id="16021-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16021-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="16021-132">Request</span></span>
<span data-ttu-id="16021-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16021-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/schools
```
##### <a name="response"></a><span data-ttu-id="16021-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="16021-134">Response</span></span>
<span data-ttu-id="16021-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16021-135">The following is an example of the response.</span></span> 

><span data-ttu-id="16021-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16021-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
