---
title: Перечисление сегментов
description: Получение списка объектов **plannerbucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a747068211f1f5843cec71dc5d793be82efa023a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454176"
---
# <a name="list-buckets"></a><span data-ttu-id="10c69-103">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="10c69-103">List buckets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10c69-104">Получение списка объектов **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="10c69-104">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="10c69-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10c69-105">Permissions</span></span>
<span data-ttu-id="10c69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10c69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10c69-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10c69-108">Permission type</span></span>      | <span data-ttu-id="10c69-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10c69-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10c69-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10c69-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10c69-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10c69-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="10c69-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10c69-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10c69-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10c69-113">Not supported.</span></span>    |
|<span data-ttu-id="10c69-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10c69-114">Application</span></span> | <span data-ttu-id="10c69-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10c69-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10c69-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10c69-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10c69-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10c69-117">Optional query parameters</span></span>
<span data-ttu-id="10c69-118">Этот метод требует указания [фильтра](https://developer.microsoft.com/graph/docs/concepts/query_parameters) по идентификатору плана.</span><span class="sxs-lookup"><span data-stu-id="10c69-118">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10c69-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10c69-119">Request headers</span></span>
| <span data-ttu-id="10c69-120">Имя</span><span class="sxs-lookup"><span data-stu-id="10c69-120">Name</span></span>      |<span data-ttu-id="10c69-121">Описание</span><span class="sxs-lookup"><span data-stu-id="10c69-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10c69-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10c69-122">Authorization</span></span>  | <span data-ttu-id="10c69-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10c69-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10c69-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10c69-125">Request body</span></span>
<span data-ttu-id="10c69-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10c69-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10c69-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="10c69-127">Response</span></span>

<span data-ttu-id="10c69-128">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="10c69-128">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="10c69-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="10c69-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="10c69-132">Пример</span><span class="sxs-lookup"><span data-stu-id="10c69-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10c69-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="10c69-133">Request</span></span>
<span data-ttu-id="10c69-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10c69-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="10c69-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="10c69-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/beta/planner/buckets
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="10c69-136">C#</span><span class="sxs-lookup"><span data-stu-id="10c69-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10c69-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="10c69-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="10c69-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="10c69-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="10c69-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="10c69-139">Response</span></span>
<span data-ttu-id="10c69-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10c69-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
