---
title: Перечисление EducationUsers
description: Получение списка пользователей в учебном заведении.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 717e2a0611601f4664a46e153d13a6e87bf8a87e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425361"
---
# <a name="list-educationusers"></a><span data-ttu-id="28365-103">Перечисление EducationUsers</span><span class="sxs-lookup"><span data-stu-id="28365-103">List educationUsers</span></span>

<span data-ttu-id="28365-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="28365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28365-105">Получение списка пользователей в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="28365-105">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="28365-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28365-106">Permissions</span></span>
<span data-ttu-id="28365-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28365-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28365-109">Permission type</span></span>      | <span data-ttu-id="28365-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28365-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28365-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28365-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="28365-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28365-112">Not supported.</span></span>  |
|<span data-ttu-id="28365-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28365-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="28365-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28365-114">Not supported.</span></span>  |
|<span data-ttu-id="28365-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28365-115">Application</span></span> | <span data-ttu-id="28365-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28365-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="28365-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28365-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28365-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28365-118">Optional query parameters</span></span>
<span data-ttu-id="28365-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="28365-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28365-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28365-120">Request headers</span></span>
| <span data-ttu-id="28365-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28365-121">Header</span></span>       | <span data-ttu-id="28365-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28365-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28365-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28365-123">Authorization</span></span>  | <span data-ttu-id="28365-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28365-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28365-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28365-126">Request body</span></span>
<span data-ttu-id="28365-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28365-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="28365-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="28365-128">Response</span></span>
<span data-ttu-id="28365-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28365-129">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28365-130">Пример</span><span class="sxs-lookup"><span data-stu-id="28365-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28365-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="28365-131">Request</span></span>
<span data-ttu-id="28365-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28365-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28365-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="28365-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
# <a name="c"></a>[<span data-ttu-id="28365-134">C#</span><span class="sxs-lookup"><span data-stu-id="28365-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28365-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28365-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28365-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28365-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28365-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="28365-137">Response</span></span>
<span data-ttu-id="28365-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28365-138">The following is an example of the response.</span></span> 

><span data-ttu-id="28365-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28365-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
          "id": "14012",
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
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
