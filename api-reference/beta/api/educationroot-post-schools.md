---
title: Создание educationSchool
description: Создание учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 439f85290d7f71179c8129597f3c659772c2c8b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887579"
---
# <a name="create-educationschool"></a><span data-ttu-id="9ee60-103">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="9ee60-103">Create educationSchool</span></span>

> <span data-ttu-id="9ee60-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ee60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ee60-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ee60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ee60-106">Создание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9ee60-106">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ee60-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ee60-107">Permissions</span></span>
<span data-ttu-id="9ee60-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ee60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ee60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ee60-110">Permission type</span></span>      | <span data-ttu-id="9ee60-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ee60-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ee60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ee60-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ee60-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ee60-113">Not supported.</span></span>  |
|<span data-ttu-id="9ee60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ee60-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ee60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ee60-115">Not supported.</span></span>  |
|<span data-ttu-id="9ee60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ee60-116">Application</span></span> | <span data-ttu-id="9ee60-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ee60-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9ee60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ee60-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="9ee60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ee60-119">Request headers</span></span>
| <span data-ttu-id="9ee60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ee60-120">Header</span></span>       | <span data-ttu-id="9ee60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9ee60-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ee60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ee60-122">Authorization</span></span>  | <span data-ttu-id="9ee60-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ee60-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ee60-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ee60-125">Content-Type</span></span>  | <span data-ttu-id="9ee60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ee60-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ee60-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ee60-127">Request body</span></span>
<span data-ttu-id="9ee60-128">В теле запроса предоставьте описание объекта [educationSchool](../resources/educationschool.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ee60-128">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9ee60-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ee60-129">Response</span></span>
<span data-ttu-id="9ee60-130">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9ee60-130">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ee60-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9ee60-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ee60-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ee60-132">Request</span></span>
<span data-ttu-id="9ee60-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ee60-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools
Content-type: application/json
Content-length: 292

{
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
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

##### <a name="response"></a><span data-ttu-id="9ee60-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ee60-134">Response</span></span>
<span data-ttu-id="9ee60-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ee60-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9ee60-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ee60-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 292

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
