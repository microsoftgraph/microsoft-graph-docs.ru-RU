---
title: Получение educationUser
description: Получение свойств и связей пользователя.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: cad5ea40eb7923bf6c8fe657d0ec783d80ef9990
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818643"
---
# <a name="get-educationuser"></a><span data-ttu-id="3a2ec-103">Получение educationUser</span><span class="sxs-lookup"><span data-stu-id="3a2ec-103">Get educationUser</span></span>

> <span data-ttu-id="3a2ec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a2ec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a2ec-106">Получение свойств и связей пользователя.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-106">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a2ec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a2ec-107">Permissions</span></span>
<span data-ttu-id="3a2ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a2ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a2ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a2ec-110">Permission type</span></span>      | <span data-ttu-id="3a2ec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a2ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a2ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a2ec-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3a2ec-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="3a2ec-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="3a2ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a2ec-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3a2ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-115">Not supported.</span></span>  |
|<span data-ttu-id="3a2ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a2ec-116">Application</span></span> | <span data-ttu-id="3a2ec-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a2ec-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="3a2ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a2ec-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a2ec-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a2ec-119">Optional query parameters</span></span>
<span data-ttu-id="3a2ec-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a2ec-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a2ec-121">Request headers</span></span>
| <span data-ttu-id="3a2ec-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a2ec-122">Header</span></span>       | <span data-ttu-id="3a2ec-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3a2ec-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a2ec-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a2ec-124">Authorization</span></span>  | <span data-ttu-id="3a2ec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a2ec-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a2ec-127">Request body</span></span>
<span data-ttu-id="3a2ec-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3a2ec-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a2ec-129">Response</span></span>
<span data-ttu-id="3a2ec-130">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-130">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a2ec-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3a2ec-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a2ec-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a2ec-132">Request</span></span>
<span data-ttu-id="3a2ec-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/beta/education/users/13012
```
##### <a name="response"></a><span data-ttu-id="3a2ec-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a2ec-134">Response</span></span>
<span data-ttu-id="3a2ec-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-135">The following is an example of the response.</span></span> 

><span data-ttu-id="3a2ec-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a2ec-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
