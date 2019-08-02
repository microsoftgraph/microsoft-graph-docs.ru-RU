---
title: Перечисление преподавателей
description: Получение списка преподавателей для класса. Чтобы делегированные маркеры могли получить список преподавателей, они должны принадлежать к классу.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b40c95e9a7cbf95ef518fa3f2c75a52b6ef3950d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006845"
---
# <a name="list-teachers"></a><span data-ttu-id="aeed6-104">Перечисление преподавателей</span><span class="sxs-lookup"><span data-stu-id="aeed6-104">List teachers</span></span>

<span data-ttu-id="aeed6-105">Получение списка преподавателей для класса.</span><span class="sxs-lookup"><span data-stu-id="aeed6-105">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="aeed6-106">Чтобы делегированные маркеры могли получить список преподавателей, они должны принадлежать к классу.</span><span class="sxs-lookup"><span data-stu-id="aeed6-106">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="aeed6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aeed6-107">Permissions</span></span>
<span data-ttu-id="aeed6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeed6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aeed6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aeed6-110">Permission type</span></span>      | <span data-ttu-id="aeed6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aeed6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aeed6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aeed6-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="aeed6-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="aeed6-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="aeed6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aeed6-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="aeed6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeed6-115">Not supported.</span></span>  |
|<span data-ttu-id="aeed6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aeed6-116">Application</span></span> | <span data-ttu-id="aeed6-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeed6-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aeed6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aeed6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aeed6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aeed6-119">Optional query parameters</span></span>
<span data-ttu-id="aeed6-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aeed6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aeed6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aeed6-121">Request headers</span></span>
| <span data-ttu-id="aeed6-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aeed6-122">Header</span></span>       | <span data-ttu-id="aeed6-123">Значение</span><span class="sxs-lookup"><span data-stu-id="aeed6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aeed6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aeed6-124">Authorization</span></span>  | <span data-ttu-id="aeed6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aeed6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aeed6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aeed6-127">Request body</span></span>
<span data-ttu-id="aeed6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aeed6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="aeed6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeed6-129">Response</span></span>
<span data-ttu-id="aeed6-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aeed6-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aeed6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aeed6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aeed6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aeed6-132">Request</span></span>
<span data-ttu-id="aeed6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aeed6-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aeed6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="aeed6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aeed6-135">C#</span><span class="sxs-lookup"><span data-stu-id="aeed6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teachers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aeed6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="aeed6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teachers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aeed6-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="aeed6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teachers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="aeed6-138">Java</span><span class="sxs-lookup"><span data-stu-id="aeed6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teachers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aeed6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeed6-139">Response</span></span>
<span data-ttu-id="aeed6-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aeed6-140">The following is an example of the response.</span></span> 

><span data-ttu-id="aeed6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aeed6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
