---
title: Получение educationUser
description: Получение свойств и связей пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8049bdf706e17193581b72fa1f6f3bc39359d195
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007065"
---
# <a name="get-educationuser"></a><span data-ttu-id="8d607-103">Получение educationUser</span><span class="sxs-lookup"><span data-stu-id="8d607-103">Get educationUser</span></span>

<span data-ttu-id="8d607-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d607-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d607-105">Получение свойств и связей пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d607-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d607-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d607-106">Permissions</span></span>

<span data-ttu-id="8d607-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> [!NOTE]
> <span data-ttu-id="8d607-109">Если используется делегированный маркер, участники могут видеть только сведения о своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="8d607-109">If the delegated token is used, members can only see information about their own account.</span></span> <span data-ttu-id="8d607-110">В данном случае используйте ресурс `beta/education/me/users`.</span><span class="sxs-lookup"><span data-stu-id="8d607-110">Use the `beta/education/me/users` resource in this case.</span></span>

| <span data-ttu-id="8d607-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d607-111">Permission type</span></span>                        | <span data-ttu-id="8d607-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d607-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8d607-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d607-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d607-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8d607-114">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="8d607-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d607-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d607-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d607-116">Not supported.</span></span>                              |
| <span data-ttu-id="8d607-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d607-117">Application</span></span>                            | <span data-ttu-id="8d607-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d607-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="8d607-119">При использовании делегированных областей разрешений Graph будет возвращать только ограниченный набор свойств:,,,,,,,,, `id` `primaryRole` `accountEnabled` `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` , `teacher/externalId` .</span><span class="sxs-lookup"><span data-stu-id="8d607-119">When using Delegated permission scopes, Graph will only return a limited set of properties: `id`, `primaryRole`, `accountEnabled`, `displayName`, `givenName`, `surname`, `userPrincipalName`, `userType`, `onPremisesInfo`, `student/externalId`, `teacher/externalId`.</span></span> <span data-ttu-id="8d607-120">Если для приложения требуются дополнительные свойства, необходимо использовать области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="8d607-120">If your application requires additional properties, you must use Application permission scopes.</span></span>

## <a name="http-request"></a><span data-ttu-id="8d607-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d607-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me
GET /education/users/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d607-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d607-122">Optional query parameters</span></span>

<span data-ttu-id="8d607-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8d607-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d607-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d607-124">Request headers</span></span>

| <span data-ttu-id="8d607-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d607-125">Header</span></span>        | <span data-ttu-id="8d607-126">Значение</span><span class="sxs-lookup"><span data-stu-id="8d607-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8d607-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d607-127">Authorization</span></span> | <span data-ttu-id="8d607-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d607-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d607-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d607-130">Request body</span></span>

<span data-ttu-id="8d607-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d607-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d607-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d607-132">Response</span></span>

<span data-ttu-id="8d607-133">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d607-133">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d607-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8d607-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8d607-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d607-135">Request</span></span>

<span data-ttu-id="8d607-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d607-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d607-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d607-137">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/13012
```

# <a name="c"></a>[<span data-ttu-id="8d607-138">C#</span><span class="sxs-lookup"><span data-stu-id="8d607-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d607-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d607-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d607-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d607-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8d607-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d607-141">Response</span></span>

<span data-ttu-id="8d607-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d607-142">The following is an example of the response.</span></span>

> <span data-ttu-id="8d607-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d607-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


