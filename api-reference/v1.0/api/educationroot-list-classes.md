---
title: Перечисление классов
description: 'Получение списка всех объектов class. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ccae0bd85a8c09dade3ee7aa91b8db4594ee1cc5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721042"
---
# <a name="list-classes"></a><span data-ttu-id="84915-103">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="84915-103">List classes</span></span>

<span data-ttu-id="84915-104">Получение списка всех объектов class.</span><span class="sxs-lookup"><span data-stu-id="84915-104">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="84915-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84915-105">Permissions</span></span>
<span data-ttu-id="84915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84915-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84915-108">Permission type</span></span>      | <span data-ttu-id="84915-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84915-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84915-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84915-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84915-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="84915-111">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="84915-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84915-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="84915-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84915-113">Not supported.</span></span>  |
|<span data-ttu-id="84915-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84915-114">Application</span></span> | <span data-ttu-id="84915-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84915-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="84915-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84915-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84915-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84915-117">Optional query parameters</span></span>
<span data-ttu-id="84915-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84915-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84915-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84915-119">Request headers</span></span>
| <span data-ttu-id="84915-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84915-120">Header</span></span>       | <span data-ttu-id="84915-121">Значение</span><span class="sxs-lookup"><span data-stu-id="84915-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="84915-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84915-122">Authorization</span></span>  | <span data-ttu-id="84915-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84915-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="84915-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84915-125">Request body</span></span>
<span data-ttu-id="84915-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84915-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="84915-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="84915-127">Response</span></span>
<span data-ttu-id="84915-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="84915-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84915-129">Пример</span><span class="sxs-lookup"><span data-stu-id="84915-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84915-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="84915-130">Request</span></span>
<span data-ttu-id="84915-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84915-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84915-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="84915-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84915-133">C#</span><span class="sxs-lookup"><span data-stu-id="84915-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84915-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84915-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84915-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84915-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="84915-136">Java</span><span class="sxs-lookup"><span data-stu-id="84915-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84915-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="84915-137">Response</span></span>
<span data-ttu-id="84915-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84915-138">The following is an example of the response.</span></span> 

><span data-ttu-id="84915-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84915-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
