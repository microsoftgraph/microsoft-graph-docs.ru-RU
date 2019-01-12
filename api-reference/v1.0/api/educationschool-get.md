---
title: Получение educationSchool
description: Получение свойств и связей объекта school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6b43360dd6582cb0f9c0f84166eb27e362dd0e0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976949"
---
# <a name="get-educationschool"></a><span data-ttu-id="d0b55-103">Получение educationSchool</span><span class="sxs-lookup"><span data-stu-id="d0b55-103">Get educationSchool</span></span>

<span data-ttu-id="d0b55-104">Получение свойств и связей объекта school.</span><span class="sxs-lookup"><span data-stu-id="d0b55-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0b55-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b55-105">Permissions</span></span>
<span data-ttu-id="d0b55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0b55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0b55-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b55-108">Permission type</span></span>      | <span data-ttu-id="d0b55-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0b55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0b55-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0b55-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d0b55-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d0b55-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="d0b55-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0b55-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d0b55-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b55-113">Not supported.</span></span>  |
|<span data-ttu-id="d0b55-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0b55-114">Application</span></span> | <span data-ttu-id="d0b55-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0b55-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d0b55-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0b55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d0b55-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d0b55-117">Optional query parameters</span></span>
<span data-ttu-id="d0b55-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d0b55-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0b55-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0b55-119">Request headers</span></span>
| <span data-ttu-id="d0b55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0b55-120">Header</span></span>       | <span data-ttu-id="d0b55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0b55-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0b55-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0b55-122">Authorization</span></span>  | <span data-ttu-id="d0b55-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0b55-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0b55-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0b55-125">Request body</span></span>
<span data-ttu-id="d0b55-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0b55-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d0b55-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b55-127">Response</span></span>
<span data-ttu-id="d0b55-128">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0b55-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0b55-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d0b55-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0b55-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0b55-130">Request</span></span>
<span data-ttu-id="d0b55-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0b55-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="d0b55-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0b55-132">Response</span></span>
<span data-ttu-id="d0b55-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0b55-133">The following is an example of the response.</span></span> 

><span data-ttu-id="d0b55-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0b55-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "principalEmail": "AmyRoebuck@contoso.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
