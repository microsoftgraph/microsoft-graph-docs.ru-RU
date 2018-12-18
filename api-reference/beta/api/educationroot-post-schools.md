---
title: Создание educationSchool
description: Создание учебного заведения.
author: mmast-msft
ms.openlocfilehash: 5be5d144f7e4a1887c9fde6196009963d9ce9893
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356128"
---
# <a name="create-educationschool"></a><span data-ttu-id="ca10a-103">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="ca10a-103">Create educationSchool</span></span>

> <span data-ttu-id="ca10a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca10a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca10a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca10a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca10a-106">Создание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ca10a-106">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca10a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca10a-107">Permissions</span></span>
<span data-ttu-id="ca10a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca10a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca10a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca10a-110">Permission type</span></span>      | <span data-ttu-id="ca10a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca10a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca10a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca10a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ca10a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca10a-113">Not supported.</span></span>  |
|<span data-ttu-id="ca10a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca10a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ca10a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca10a-115">Not supported.</span></span>  |
|<span data-ttu-id="ca10a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca10a-116">Application</span></span> | <span data-ttu-id="ca10a-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca10a-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ca10a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca10a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="ca10a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca10a-119">Request headers</span></span>
| <span data-ttu-id="ca10a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca10a-120">Header</span></span>       | <span data-ttu-id="ca10a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ca10a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca10a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca10a-122">Authorization</span></span>  | <span data-ttu-id="ca10a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca10a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ca10a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca10a-125">Content-Type</span></span>  | <span data-ttu-id="ca10a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca10a-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca10a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca10a-127">Request body</span></span>
<span data-ttu-id="ca10a-128">В теле запроса предоставьте описание объекта [educationSchool](../resources/educationschool.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca10a-128">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ca10a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca10a-129">Response</span></span>
<span data-ttu-id="ca10a-130">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ca10a-130">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca10a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ca10a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca10a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca10a-132">Request</span></span>
<span data-ttu-id="ca10a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca10a-133">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ca10a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca10a-134">Response</span></span>
<span data-ttu-id="ca10a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca10a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="ca10a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca10a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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