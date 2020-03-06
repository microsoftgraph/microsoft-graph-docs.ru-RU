---
title: Перечисление курсов
description: 'Получение списка объектов курсов. Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 597fddd2f66a60dd5dfe83234873ee2df3498a80
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517420"
---
# <a name="list-classes"></a><span data-ttu-id="b048e-104">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="b048e-104">List classes</span></span>

<span data-ttu-id="b048e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b048e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b048e-106">Получение списка объектов курсов.</span><span class="sxs-lookup"><span data-stu-id="b048e-106">Retrieve a list of class objects.</span></span> <span data-ttu-id="b048e-107">Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах.</span><span class="sxs-lookup"><span data-stu-id="b048e-107">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="b048e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b048e-108">Permissions</span></span>
<span data-ttu-id="b048e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b048e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b048e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b048e-111">Permission type</span></span>      | <span data-ttu-id="b048e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b048e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b048e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b048e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b048e-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b048e-114">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b048e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b048e-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b048e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b048e-116">Not supported.</span></span>  |
|<span data-ttu-id="b048e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b048e-117">Application</span></span> | <span data-ttu-id="b048e-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b048e-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b048e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b048e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b048e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b048e-120">Optional query parameters</span></span>
<span data-ttu-id="b048e-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b048e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b048e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b048e-122">Request headers</span></span>
| <span data-ttu-id="b048e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b048e-123">Header</span></span>       | <span data-ttu-id="b048e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b048e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b048e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b048e-125">Authorization</span></span>  | <span data-ttu-id="b048e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b048e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b048e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b048e-128">Request body</span></span>
<span data-ttu-id="b048e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b048e-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b048e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b048e-130">Response</span></span>
<span data-ttu-id="b048e-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b048e-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b048e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b048e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b048e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b048e-133">Request</span></span>
<span data-ttu-id="b048e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b048e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b048e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b048e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/classes
```
# <a name="c"></a>[<span data-ttu-id="b048e-136">C#</span><span class="sxs-lookup"><span data-stu-id="b048e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b048e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b048e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b048e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b048e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b048e-139">Java</span><span class="sxs-lookup"><span data-stu-id="b048e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b048e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b048e-140">Response</span></span>
<span data-ttu-id="b048e-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b048e-141">The following is an example of the response.</span></span> 

><span data-ttu-id="b048e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b048e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
