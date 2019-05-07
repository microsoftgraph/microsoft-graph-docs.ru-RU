---
title: Перечисление пользователей
description: Получение списка объектов user. Эти объекты user будут содержать специальные свойства, связанные с образованием.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 10ec2434232b963e3e88a6e52134e4550edff4b5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616196"
---
# <a name="list-users"></a><span data-ttu-id="beeda-104">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="beeda-104">List users</span></span>

<span data-ttu-id="beeda-105">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="beeda-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="beeda-106">Эти объекты user будут содержать специальные свойства, связанные с образованием.</span><span class="sxs-lookup"><span data-stu-id="beeda-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="beeda-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="beeda-107">Permissions</span></span>
<span data-ttu-id="beeda-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beeda-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beeda-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beeda-110">Permission type</span></span>      | <span data-ttu-id="beeda-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="beeda-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beeda-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beeda-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="beeda-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beeda-113">Not supported.</span></span>  |
|<span data-ttu-id="beeda-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beeda-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="beeda-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beeda-115">Not supported.</span></span>  |
|<span data-ttu-id="beeda-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beeda-116">Application</span></span> | <span data-ttu-id="beeda-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beeda-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="beeda-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beeda-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="beeda-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="beeda-119">Optional query parameters</span></span>
<span data-ttu-id="beeda-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="beeda-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="beeda-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beeda-121">Request headers</span></span>
| <span data-ttu-id="beeda-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="beeda-122">Header</span></span>       | <span data-ttu-id="beeda-123">Значение</span><span class="sxs-lookup"><span data-stu-id="beeda-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="beeda-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="beeda-124">Authorization</span></span>  | <span data-ttu-id="beeda-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beeda-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="beeda-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beeda-127">Request body</span></span>
<span data-ttu-id="beeda-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="beeda-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="beeda-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="beeda-129">Response</span></span>
<span data-ttu-id="beeda-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="beeda-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="beeda-131">Пример</span><span class="sxs-lookup"><span data-stu-id="beeda-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="beeda-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="beeda-132">Request</span></span>
<span data-ttu-id="beeda-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beeda-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users
```
##### <a name="response"></a><span data-ttu-id="beeda-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="beeda-134">Response</span></span>
<span data-ttu-id="beeda-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="beeda-135">The following is an example of the response.</span></span> 

><span data-ttu-id="beeda-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="beeda-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="beeda-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="beeda-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="beeda-139">Языках</span><span class="sxs-lookup"><span data-stu-id="beeda-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="beeda-140">Язык</span><span class="sxs-lookup"><span data-stu-id="beeda-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
