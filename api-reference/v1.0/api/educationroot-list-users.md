---
title: Перечисление пользователей
description: Получение списка объектов user. Эти объекты user будут содержать специальные свойства, связанные с образованием.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bb6503cfddf4fe3958c5cc8c455d2c6a26cdc0fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009760"
---
# <a name="list-users"></a><span data-ttu-id="fa309-104">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="fa309-104">List users</span></span>

<span data-ttu-id="fa309-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa309-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa309-106">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="fa309-106">Retrieve a list of user objects.</span></span> <span data-ttu-id="fa309-107">Эти объекты user будут содержать специальные свойства, связанные с образованием.</span><span class="sxs-lookup"><span data-stu-id="fa309-107">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa309-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa309-108">Permissions</span></span>
<span data-ttu-id="fa309-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa309-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa309-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa309-111">Permission type</span></span>      | <span data-ttu-id="fa309-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa309-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa309-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa309-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fa309-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa309-114">Not supported.</span></span>  |
|<span data-ttu-id="fa309-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa309-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fa309-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa309-116">Not supported.</span></span>  |
|<span data-ttu-id="fa309-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa309-117">Application</span></span> | <span data-ttu-id="fa309-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa309-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fa309-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa309-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa309-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa309-120">Optional query parameters</span></span>
<span data-ttu-id="fa309-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa309-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa309-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa309-122">Request headers</span></span>
| <span data-ttu-id="fa309-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa309-123">Header</span></span>       | <span data-ttu-id="fa309-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fa309-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa309-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa309-125">Authorization</span></span>  | <span data-ttu-id="fa309-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa309-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa309-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa309-128">Request body</span></span>
<span data-ttu-id="fa309-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa309-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fa309-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa309-130">Response</span></span>
<span data-ttu-id="fa309-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa309-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa309-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fa309-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa309-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa309-133">Request</span></span>
<span data-ttu-id="fa309-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa309-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa309-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa309-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationroot_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users
```
# <a name="c"></a>[<span data-ttu-id="fa309-136">C#</span><span class="sxs-lookup"><span data-stu-id="fa309-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationroot-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa309-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa309-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationroot-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa309-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa309-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationroot-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa309-139">Java</span><span class="sxs-lookup"><span data-stu-id="fa309-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationroot-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa309-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa309-140">Response</span></span>
<span data-ttu-id="fa309-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa309-141">The following is an example of the response.</span></span> 

><span data-ttu-id="fa309-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa309-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

