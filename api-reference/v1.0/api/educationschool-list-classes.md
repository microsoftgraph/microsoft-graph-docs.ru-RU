---
title: Перечисление educationClasses
description: Получение списка курсов учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2a3f449c94138a3fa4b36fe3ca57eb9ee4728d54
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887721"
---
# <a name="list-educationclasses"></a><span data-ttu-id="1292d-103">Перечисление educationClasses</span><span class="sxs-lookup"><span data-stu-id="1292d-103">List educationClasses</span></span>

<span data-ttu-id="1292d-104">Получение списка курсов учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1292d-104">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="1292d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1292d-105">Permissions</span></span>
<span data-ttu-id="1292d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1292d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1292d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1292d-108">Permission type</span></span>      | <span data-ttu-id="1292d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1292d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1292d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1292d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1292d-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="1292d-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="1292d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1292d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1292d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1292d-113">Not supported.</span></span>  |
|<span data-ttu-id="1292d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1292d-114">Application</span></span> | <span data-ttu-id="1292d-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1292d-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1292d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1292d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1292d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1292d-117">Optional query parameters</span></span>
<span data-ttu-id="1292d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1292d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1292d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1292d-119">Request headers</span></span>
| <span data-ttu-id="1292d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1292d-120">Header</span></span>       | <span data-ttu-id="1292d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1292d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1292d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1292d-122">Authorization</span></span>  | <span data-ttu-id="1292d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1292d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1292d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1292d-125">Request body</span></span>
<span data-ttu-id="1292d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1292d-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1292d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1292d-127">Response</span></span>
<span data-ttu-id="1292d-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1292d-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1292d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1292d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1292d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1292d-130">Request</span></span>
<span data-ttu-id="1292d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1292d-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1292d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1292d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1292d-133">C#</span><span class="sxs-lookup"><span data-stu-id="1292d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1292d-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1292d-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1292d-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1292d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1292d-136">Java</span><span class="sxs-lookup"><span data-stu-id="1292d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1292d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1292d-137">Response</span></span>
<span data-ttu-id="1292d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1292d-138">The following is an example of the response.</span></span> 

><span data-ttu-id="1292d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1292d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
