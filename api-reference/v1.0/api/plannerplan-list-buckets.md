---
title: Перечисление сегментов
description: Получение списка объектов **plannerbucket**, содержащихся в объекте plannerPlan.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f781eb40dbf5bf7e33a99b3cff9b332a62502a29
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473390"
---
# <a name="list-buckets"></a><span data-ttu-id="35ab8-103">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="35ab8-103">List buckets</span></span>

<span data-ttu-id="35ab8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35ab8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35ab8-105">Извлечение списка [объектов plannerBucket,](../resources/plannerbucket.md) содержащихся в [объекте plannerPlan.](../resources/plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="35ab8-105">Retrieve a list of [plannerBucket](../resources/plannerbucket.md) objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="35ab8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35ab8-106">Permissions</span></span>
<span data-ttu-id="35ab8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35ab8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35ab8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35ab8-109">Permission type</span></span>      | <span data-ttu-id="35ab8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35ab8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35ab8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35ab8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35ab8-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35ab8-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="35ab8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35ab8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35ab8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35ab8-114">Not supported.</span></span>    |
|<span data-ttu-id="35ab8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35ab8-115">Application</span></span> | <span data-ttu-id="35ab8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35ab8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35ab8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35ab8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="35ab8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35ab8-118">Request headers</span></span>
| <span data-ttu-id="35ab8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="35ab8-119">Name</span></span>      |<span data-ttu-id="35ab8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="35ab8-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35ab8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35ab8-121">Authorization</span></span>  | <span data-ttu-id="35ab8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35ab8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35ab8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35ab8-124">Request body</span></span>
<span data-ttu-id="35ab8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35ab8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35ab8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="35ab8-126">Response</span></span>

<span data-ttu-id="35ab8-127">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="35ab8-127">If successful, this method returns a `200 OK` response code and a collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="35ab8-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="35ab8-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="35ab8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="35ab8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35ab8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="35ab8-132">Request</span></span>
<span data-ttu-id="35ab8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35ab8-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35ab8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="35ab8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
# <a name="c"></a>[<span data-ttu-id="35ab8-135">C#</span><span class="sxs-lookup"><span data-stu-id="35ab8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35ab8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35ab8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35ab8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35ab8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35ab8-138">Java</span><span class="sxs-lookup"><span data-stu-id="35ab8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-buckets-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="35ab8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="35ab8-139">Response</span></span>
<span data-ttu-id="35ab8-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35ab8-140">Here is an example of the response.</span></span> 

><span data-ttu-id="35ab8-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35ab8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

