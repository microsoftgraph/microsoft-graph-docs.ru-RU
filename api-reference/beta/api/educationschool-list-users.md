---
title: Перечисление EducationUsers
description: Получение списка пользователей в учебном заведении.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e70f7fcf86d37099c56e1e6638c7358dc22032f3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043376"
---
# <a name="list-educationusers"></a><span data-ttu-id="91bec-103">Перечисление EducationUsers</span><span class="sxs-lookup"><span data-stu-id="91bec-103">List educationUsers</span></span>

<span data-ttu-id="91bec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91bec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91bec-105">Получение списка пользователей в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="91bec-105">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="91bec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91bec-106">Permissions</span></span>
<span data-ttu-id="91bec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91bec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91bec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91bec-109">Permission type</span></span>      | <span data-ttu-id="91bec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91bec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91bec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91bec-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="91bec-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91bec-112">Not supported.</span></span>  |
|<span data-ttu-id="91bec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91bec-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="91bec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91bec-114">Not supported.</span></span>  |
|<span data-ttu-id="91bec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91bec-115">Application</span></span> | <span data-ttu-id="91bec-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91bec-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="91bec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91bec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91bec-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91bec-118">Optional query parameters</span></span>
<span data-ttu-id="91bec-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91bec-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91bec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91bec-120">Request headers</span></span>
| <span data-ttu-id="91bec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91bec-121">Header</span></span>       | <span data-ttu-id="91bec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="91bec-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91bec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91bec-123">Authorization</span></span>  | <span data-ttu-id="91bec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91bec-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91bec-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91bec-126">Request body</span></span>
<span data-ttu-id="91bec-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91bec-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="91bec-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="91bec-128">Response</span></span>
<span data-ttu-id="91bec-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91bec-129">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91bec-130">Пример</span><span class="sxs-lookup"><span data-stu-id="91bec-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91bec-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="91bec-131">Request</span></span>
<span data-ttu-id="91bec-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91bec-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91bec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="91bec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
# <a name="c"></a>[<span data-ttu-id="91bec-134">C#</span><span class="sxs-lookup"><span data-stu-id="91bec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91bec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91bec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91bec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91bec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91bec-137">Java</span><span class="sxs-lookup"><span data-stu-id="91bec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91bec-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="91bec-138">Response</span></span>
<span data-ttu-id="91bec-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91bec-139">The following is an example of the response.</span></span> 

><span data-ttu-id="91bec-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="91bec-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
