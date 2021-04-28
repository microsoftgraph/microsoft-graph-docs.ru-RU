---
title: Перечисление пользователей
description: Получение списка объектов user. Эти объекты user будут содержать специальные свойства, связанные с образованием.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 48253e39c70ff481eaab450e96428d4af63d523a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053148"
---
# <a name="list-users"></a><span data-ttu-id="7986f-104">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="7986f-104">List users</span></span>

<span data-ttu-id="7986f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7986f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7986f-106">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="7986f-106">Retrieve a list of user objects.</span></span> <span data-ttu-id="7986f-107">Эти объекты user будут содержать специальные свойства, связанные с образованием.</span><span class="sxs-lookup"><span data-stu-id="7986f-107">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7986f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7986f-108">Permissions</span></span>
<span data-ttu-id="7986f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7986f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7986f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7986f-111">Permission type</span></span>      | <span data-ttu-id="7986f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7986f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7986f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7986f-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="7986f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7986f-114">Not supported.</span></span>  |
|<span data-ttu-id="7986f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7986f-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7986f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7986f-116">Not supported.</span></span>  |
|<span data-ttu-id="7986f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7986f-117">Application</span></span> | <span data-ttu-id="7986f-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7986f-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7986f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7986f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7986f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7986f-120">Optional query parameters</span></span>
<span data-ttu-id="7986f-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7986f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7986f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7986f-122">Request headers</span></span>
| <span data-ttu-id="7986f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7986f-123">Header</span></span>       | <span data-ttu-id="7986f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7986f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7986f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7986f-125">Authorization</span></span>  | <span data-ttu-id="7986f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7986f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7986f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7986f-128">Request body</span></span>
<span data-ttu-id="7986f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7986f-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7986f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7986f-130">Response</span></span>
<span data-ttu-id="7986f-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7986f-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7986f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7986f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7986f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7986f-133">Request</span></span>
<span data-ttu-id="7986f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7986f-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7986f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7986f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationroot_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users
```
# <a name="c"></a>[<span data-ttu-id="7986f-136">C#</span><span class="sxs-lookup"><span data-stu-id="7986f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationroot-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7986f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7986f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationroot-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7986f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7986f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationroot-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7986f-139">Java</span><span class="sxs-lookup"><span data-stu-id="7986f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationroot-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7986f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7986f-140">Response</span></span>
<span data-ttu-id="7986f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7986f-141">The following is an example of the response.</span></span> 

><span data-ttu-id="7986f-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7986f-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "middleName": null,
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
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
