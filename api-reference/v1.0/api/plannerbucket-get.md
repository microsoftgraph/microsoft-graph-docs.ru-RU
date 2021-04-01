---
title: Получение объекта plannerBucket
description: Получение свойств и связей объекта **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: ea6943d810630ab97ca0a0d11b43ff2844733997
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473754"
---
# <a name="get-plannerbucket"></a><span data-ttu-id="ecb6b-103">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ecb6b-103">Get plannerBucket</span></span>

<span data-ttu-id="ecb6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecb6b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecb6b-105">Получение свойств и связей объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="ecb6b-105">Retrieve the properties and relationships of **plannerBucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ecb6b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecb6b-106">Permissions</span></span>
<span data-ttu-id="ecb6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb6b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecb6b-109">Permission type</span></span>      | <span data-ttu-id="ecb6b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecb6b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecb6b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecb6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ecb6b-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecb6b-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ecb6b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecb6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecb6b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecb6b-114">Not supported.</span></span>    |
|<span data-ttu-id="ecb6b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecb6b-115">Application</span></span> | <span data-ttu-id="ecb6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecb6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecb6b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecb6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ecb6b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecb6b-118">Request headers</span></span>
| <span data-ttu-id="ecb6b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ecb6b-119">Name</span></span>      |<span data-ttu-id="ecb6b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ecb6b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ecb6b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecb6b-121">Authorization</span></span>  | <span data-ttu-id="ecb6b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecb6b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecb6b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecb6b-124">Request body</span></span>
<span data-ttu-id="ecb6b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecb6b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecb6b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecb6b-126">Response</span></span>

<span data-ttu-id="ecb6b-127">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ecb6b-127">If successful, this method returns a `200 OK` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="ecb6b-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ecb6b-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ecb6b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ecb6b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ecb6b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecb6b-132">Request</span></span>
<span data-ttu-id="ecb6b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecb6b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ecb6b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecb6b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
```
# <a name="c"></a>[<span data-ttu-id="ecb6b-135">C#</span><span class="sxs-lookup"><span data-stu-id="ecb6b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecb6b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecb6b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecb6b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecb6b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecb6b-138">Java</span><span class="sxs-lookup"><span data-stu-id="ecb6b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ecb6b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecb6b-139">Response</span></span>
<span data-ttu-id="ecb6b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ecb6b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

