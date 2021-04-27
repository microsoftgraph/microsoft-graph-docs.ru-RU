---
title: Получение educationUser
description: Получение свойств и связей пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 893f484eaf03ef5102a22e70fdb946251af0cbd9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042893"
---
# <a name="get-educationuser"></a><span data-ttu-id="7bddc-103">Получение educationUser</span><span class="sxs-lookup"><span data-stu-id="7bddc-103">Get educationUser</span></span>

<span data-ttu-id="7bddc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bddc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bddc-105">Получение свойств и связей пользователя.</span><span class="sxs-lookup"><span data-stu-id="7bddc-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bddc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bddc-106">Permissions</span></span>

<span data-ttu-id="7bddc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> [!NOTE]
> <span data-ttu-id="7bddc-109">Если используется делегированная маркерная запись, участники могут видеть только сведения о своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7bddc-109">If the delegated token is used, members can only see information about their own account.</span></span> <span data-ttu-id="7bddc-110">В данном случае используйте ресурс `beta/education/me/users`.</span><span class="sxs-lookup"><span data-stu-id="7bddc-110">Use the `beta/education/me/users` resource in this case.</span></span>

| <span data-ttu-id="7bddc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bddc-111">Permission type</span></span>                        | <span data-ttu-id="7bddc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bddc-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7bddc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bddc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bddc-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="7bddc-114">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="7bddc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bddc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bddc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bddc-116">Not supported.</span></span>                              |
| <span data-ttu-id="7bddc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bddc-117">Application</span></span>                            | <span data-ttu-id="7bddc-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bddc-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="7bddc-119">При использовании областей делегирования разрешений Graph возвращает только ограниченный набор свойств: `id` `primaryRole` , , `accountEnabled` `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` `teacher/externalId` .</span><span class="sxs-lookup"><span data-stu-id="7bddc-119">When using Delegated permission scopes, Graph will only return a limited set of properties: `id`, `primaryRole`, `accountEnabled`, `displayName`, `givenName`, `surname`, `userPrincipalName`, `userType`, `onPremisesInfo`, `student/externalId`, `teacher/externalId`.</span></span> <span data-ttu-id="7bddc-120">Если вашему приложению необходимы дополнительные свойства, необходимо использовать области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="7bddc-120">If your application requires additional properties, you must use Application permission scopes.</span></span>

## <a name="http-request"></a><span data-ttu-id="7bddc-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bddc-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me
GET /education/users/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bddc-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7bddc-122">Optional query parameters</span></span>

<span data-ttu-id="7bddc-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7bddc-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bddc-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bddc-124">Request headers</span></span>

| <span data-ttu-id="7bddc-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bddc-125">Header</span></span>        | <span data-ttu-id="7bddc-126">Значение</span><span class="sxs-lookup"><span data-stu-id="7bddc-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7bddc-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bddc-127">Authorization</span></span> | <span data-ttu-id="7bddc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bddc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bddc-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bddc-130">Request body</span></span>

<span data-ttu-id="7bddc-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bddc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bddc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bddc-132">Response</span></span>

<span data-ttu-id="7bddc-133">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7bddc-133">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bddc-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7bddc-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7bddc-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bddc-135">Request</span></span>

<span data-ttu-id="7bddc-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bddc-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7bddc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bddc-137">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/13012
```

# <a name="c"></a>[<span data-ttu-id="7bddc-138">C#</span><span class="sxs-lookup"><span data-stu-id="7bddc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-2-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bddc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bddc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-2-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bddc-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bddc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-2-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7bddc-141">Java</span><span class="sxs-lookup"><span data-stu-id="7bddc-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7bddc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bddc-142">Response</span></span>

<span data-ttu-id="7bddc-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7bddc-143">The following is an example of the response.</span></span>

> <span data-ttu-id="7bddc-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7bddc-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
