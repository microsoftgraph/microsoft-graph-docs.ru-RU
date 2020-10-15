---
title: Перечисление классов
description: 'Получение списка всех объектов class. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d5b38d804c0e56343456f380ef61f1470a98d66b
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460784"
---
# <a name="list-classes"></a><span data-ttu-id="2d0ef-103">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="2d0ef-103">List classes</span></span>

<span data-ttu-id="2d0ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d0ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d0ef-105">Получение списка всех объектов class.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-105">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2d0ef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d0ef-106">Permissions</span></span>
<span data-ttu-id="2d0ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d0ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d0ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d0ef-109">Permission type</span></span>      | <span data-ttu-id="2d0ef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d0ef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d0ef-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d0ef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d0ef-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2d0ef-112">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="2d0ef-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d0ef-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2d0ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-114">Not supported.</span></span>  |
|<span data-ttu-id="2d0ef-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2d0ef-115">Application</span></span> | <span data-ttu-id="2d0ef-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d0ef-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2d0ef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d0ef-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d0ef-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d0ef-118">Optional query parameters</span></span>
<span data-ttu-id="2d0ef-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d0ef-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d0ef-120">Request headers</span></span>
| <span data-ttu-id="2d0ef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d0ef-121">Header</span></span>       | <span data-ttu-id="2d0ef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2d0ef-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d0ef-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d0ef-123">Authorization</span></span>  | <span data-ttu-id="2d0ef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="2d0ef-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d0ef-126">Request body</span></span>
<span data-ttu-id="2d0ef-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2d0ef-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d0ef-128">Response</span></span>
<span data-ttu-id="2d0ef-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-129">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d0ef-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2d0ef-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d0ef-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d0ef-131">Request</span></span>
<span data-ttu-id="2d0ef-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d0ef-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d0ef-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes
```
# <a name="c"></a>[<span data-ttu-id="2d0ef-134">C#</span><span class="sxs-lookup"><span data-stu-id="2d0ef-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d0ef-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d0ef-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d0ef-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d0ef-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d0ef-137">Java</span><span class="sxs-lookup"><span data-stu-id="2d0ef-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2d0ef-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d0ef-138">Response</span></span>
<span data-ttu-id="2d0ef-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-139">The following is an example of the response.</span></span> 

><span data-ttu-id="2d0ef-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d0ef-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
