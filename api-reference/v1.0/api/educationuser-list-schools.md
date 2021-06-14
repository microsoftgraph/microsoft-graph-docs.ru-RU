---
title: Список школ educationUser
description: Получение списка учебных заведений для этого пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 180309cb87e3d8678e81235309338a1817fb0b91
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912000"
---
# <a name="list-schools-of-an-educationuser"></a><span data-ttu-id="92510-103">Список школ educationUser</span><span class="sxs-lookup"><span data-stu-id="92510-103">List schools of an educationUser</span></span>

<span data-ttu-id="92510-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92510-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92510-105">Получение списка учебных заведений для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="92510-105">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="92510-106">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="92510-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="92510-107">В данном случае используйте ресурс `...v1.0/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="92510-107">Use the `...v1.0/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="92510-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92510-108">Permissions</span></span>

<span data-ttu-id="92510-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92510-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92510-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92510-111">Permission type</span></span>                        | <span data-ttu-id="92510-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92510-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="92510-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92510-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="92510-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="92510-114">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="92510-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92510-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92510-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92510-116">Not supported.</span></span>                              |
| <span data-ttu-id="92510-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="92510-117">Application</span></span>                            | <span data-ttu-id="92510-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92510-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92510-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92510-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{educationUserId}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92510-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92510-120">Optional query parameters</span></span>

<span data-ttu-id="92510-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92510-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92510-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92510-122">Request headers</span></span>

| <span data-ttu-id="92510-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92510-123">Header</span></span>        | <span data-ttu-id="92510-124">Значение</span><span class="sxs-lookup"><span data-stu-id="92510-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="92510-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92510-125">Authorization</span></span> | <span data-ttu-id="92510-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92510-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92510-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="92510-128">Request body</span></span>

<span data-ttu-id="92510-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92510-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92510-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="92510-130">Response</span></span>

<span data-ttu-id="92510-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="92510-131">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92510-132">Пример</span><span class="sxs-lookup"><span data-stu-id="92510-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="92510-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="92510-133">Request</span></span>

<span data-ttu-id="92510-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92510-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92510-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="92510-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/schools
```

# <a name="c"></a>[<span data-ttu-id="92510-136">C#</span><span class="sxs-lookup"><span data-stu-id="92510-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92510-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92510-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92510-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92510-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92510-139">Java</span><span class="sxs-lookup"><span data-stu-id="92510-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92510-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="92510-140">Response</span></span>

<span data-ttu-id="92510-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="92510-141">The following is an example of the response.</span></span>

><span data-ttu-id="92510-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92510-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
