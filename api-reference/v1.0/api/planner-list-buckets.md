---
title: Перечисление сегментов
description: Получение списка объектов **plannerbucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 26da0ec336de9b33dc87edf14584c9deb739ee9d
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458957"
---
# <a name="list-buckets"></a><span data-ttu-id="60034-103">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="60034-103">List buckets</span></span>

<span data-ttu-id="60034-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60034-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60034-105">Получение списка объектов **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="60034-105">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="60034-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60034-106">Permissions</span></span>
<span data-ttu-id="60034-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60034-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60034-109">Permission type</span></span>      | <span data-ttu-id="60034-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60034-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60034-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60034-111">Delegated (work or school account)</span></span> | <span data-ttu-id="60034-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60034-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60034-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60034-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60034-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60034-114">Not supported.</span></span>    |
|<span data-ttu-id="60034-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60034-115">Application</span></span> | <span data-ttu-id="60034-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60034-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60034-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60034-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="60034-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60034-118">Optional query parameters</span></span>
<span data-ttu-id="60034-119">Этот метод требует указания [фильтра](/graph/query-parameters) по идентификатору плана.</span><span class="sxs-lookup"><span data-stu-id="60034-119">This method requires planId [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60034-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60034-120">Request headers</span></span>
| <span data-ttu-id="60034-121">Имя</span><span class="sxs-lookup"><span data-stu-id="60034-121">Name</span></span>      |<span data-ttu-id="60034-122">Описание</span><span class="sxs-lookup"><span data-stu-id="60034-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60034-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60034-123">Authorization</span></span>  | <span data-ttu-id="60034-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60034-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60034-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60034-126">Request body</span></span>
<span data-ttu-id="60034-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60034-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60034-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="60034-128">Response</span></span>

<span data-ttu-id="60034-129">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="60034-129">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="60034-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="60034-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="60034-133">Пример</span><span class="sxs-lookup"><span data-stu-id="60034-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60034-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="60034-134">Request</span></span>
<span data-ttu-id="60034-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60034-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60034-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="60034-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/buckets
```
# <a name="c"></a>[<span data-ttu-id="60034-137">C#</span><span class="sxs-lookup"><span data-stu-id="60034-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60034-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60034-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60034-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60034-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60034-140">Java</span><span class="sxs-lookup"><span data-stu-id="60034-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-buckets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="60034-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="60034-141">Response</span></span>
<span data-ttu-id="60034-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60034-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
