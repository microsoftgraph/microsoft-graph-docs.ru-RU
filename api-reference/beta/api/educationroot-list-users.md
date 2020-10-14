---
title: Перечисление пользователей
description: Получение списка объектов user. Эти объекты user будут содержать специальные свойства, связанные с образованием.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9bb5a5a6972519ebcb2e067960aa712adc75f719
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457656"
---
# <a name="list-users"></a><span data-ttu-id="d951c-104">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="d951c-104">List users</span></span>

<span data-ttu-id="d951c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d951c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d951c-106">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="d951c-106">Retrieve a list of user objects.</span></span> <span data-ttu-id="d951c-107">Эти объекты user будут содержать специальные свойства, связанные с образованием.</span><span class="sxs-lookup"><span data-stu-id="d951c-107">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d951c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d951c-108">Permissions</span></span>
<span data-ttu-id="d951c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d951c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d951c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d951c-111">Permission type</span></span>      | <span data-ttu-id="d951c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d951c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d951c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d951c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="d951c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d951c-114">Not supported.</span></span>  |
|<span data-ttu-id="d951c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d951c-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d951c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d951c-116">Not supported.</span></span>  |
|<span data-ttu-id="d951c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d951c-117">Application</span></span> | <span data-ttu-id="d951c-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d951c-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d951c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d951c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d951c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d951c-120">Optional query parameters</span></span>
<span data-ttu-id="d951c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d951c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d951c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d951c-122">Request headers</span></span>
| <span data-ttu-id="d951c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d951c-123">Header</span></span>       | <span data-ttu-id="d951c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d951c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d951c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d951c-125">Authorization</span></span>  | <span data-ttu-id="d951c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d951c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d951c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d951c-128">Request body</span></span>
<span data-ttu-id="d951c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d951c-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d951c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d951c-130">Response</span></span>
<span data-ttu-id="d951c-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d951c-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d951c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d951c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d951c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d951c-133">Request</span></span>
<span data-ttu-id="d951c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d951c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d951c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d951c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationroot_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users
```
# <a name="c"></a>[<span data-ttu-id="d951c-136">C#</span><span class="sxs-lookup"><span data-stu-id="d951c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationroot-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d951c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d951c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationroot-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d951c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d951c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationroot-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d951c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d951c-139">Response</span></span>
<span data-ttu-id="d951c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d951c-140">The following is an example of the response.</span></span> 

><span data-ttu-id="d951c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d951c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
