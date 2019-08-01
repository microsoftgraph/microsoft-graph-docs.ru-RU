---
title: Создание объекта plannerBucket
description: Используйте этот API, чтобы создать объект **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 397810c3590b9cd0feb1223e8a484bbf175ca266
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976210"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="d472b-103">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d472b-103">Create plannerBucket</span></span>

<span data-ttu-id="d472b-104">Используйте этот API, чтобы создать объект **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="d472b-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="d472b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d472b-105">Permissions</span></span>
<span data-ttu-id="d472b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d472b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d472b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d472b-108">Permission type</span></span>      | <span data-ttu-id="d472b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d472b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d472b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d472b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d472b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d472b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d472b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d472b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d472b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d472b-113">Not supported.</span></span>    |
|<span data-ttu-id="d472b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d472b-114">Application</span></span> | <span data-ttu-id="d472b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d472b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d472b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d472b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="d472b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d472b-117">Request headers</span></span>
| <span data-ttu-id="d472b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d472b-118">Name</span></span>       | <span data-ttu-id="d472b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d472b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d472b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d472b-120">Authorization</span></span>  | <span data-ttu-id="d472b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d472b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d472b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d472b-123">Request body</span></span>
<span data-ttu-id="d472b-124">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d472b-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d472b-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="d472b-125">Response</span></span>

<span data-ttu-id="d472b-126">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d472b-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="d472b-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d472b-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d472b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d472b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d472b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d472b-131">Request</span></span>
<span data-ttu-id="d472b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d472b-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d472b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d472b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d472b-134">C#</span><span class="sxs-lookup"><span data-stu-id="d472b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d472b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d472b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d472b-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d472b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d472b-137">Java</span><span class="sxs-lookup"><span data-stu-id="d472b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerbucket-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d472b-138">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d472b-138">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d472b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d472b-139">Response</span></span>
<span data-ttu-id="d472b-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d472b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

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
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
