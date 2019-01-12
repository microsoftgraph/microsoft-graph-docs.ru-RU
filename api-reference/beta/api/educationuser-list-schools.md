---
title: Перечисление учебных заведений
description: Получение списка учебных заведений для этого пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1608ce9085bfcdb52cd781192e67714789780743
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980659"
---
# <a name="list-schools"></a><span data-ttu-id="0f830-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="0f830-103">List schools</span></span>

> <span data-ttu-id="0f830-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f830-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f830-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f830-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f830-106">Получение списка учебных заведений для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f830-106">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="0f830-107">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="0f830-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="0f830-108">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="0f830-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f830-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f830-109">Permissions</span></span>
<span data-ttu-id="0f830-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f830-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f830-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f830-112">Permission type</span></span>      | <span data-ttu-id="0f830-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f830-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f830-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f830-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="0f830-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="0f830-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="0f830-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f830-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0f830-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f830-117">Not supported.</span></span>  |
|<span data-ttu-id="0f830-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f830-118">Application</span></span> | <span data-ttu-id="0f830-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f830-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0f830-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f830-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0f830-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0f830-121">Optional query parameters</span></span>
<span data-ttu-id="0f830-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0f830-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f830-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f830-123">Request headers</span></span>
| <span data-ttu-id="0f830-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f830-124">Header</span></span>       | <span data-ttu-id="0f830-125">Значение</span><span class="sxs-lookup"><span data-stu-id="0f830-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f830-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f830-126">Authorization</span></span>  | <span data-ttu-id="0f830-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f830-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f830-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f830-129">Request body</span></span>
<span data-ttu-id="0f830-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f830-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0f830-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f830-131">Response</span></span>
<span data-ttu-id="0f830-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0f830-132">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f830-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0f830-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f830-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f830-134">Request</span></span>
<span data-ttu-id="0f830-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f830-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="0f830-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f830-136">Response</span></span>
<span data-ttu-id="0f830-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0f830-137">The following is an example of the response.</span></span> 

><span data-ttu-id="0f830-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f830-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
