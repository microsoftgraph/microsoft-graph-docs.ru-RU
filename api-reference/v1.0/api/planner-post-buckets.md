---
title: Создание объекта plannerBucket
description: Используйте этот API, чтобы создать объект **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9a72d4d330b83b1e11af66d67f7b1f44208d0c2b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274230"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="ff1ff-103">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ff1ff-103">Create plannerBucket</span></span>

<span data-ttu-id="ff1ff-104">Используйте этот API, чтобы создать объект **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff1ff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff1ff-105">Permissions</span></span>
<span data-ttu-id="ff1ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff1ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff1ff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff1ff-108">Permission type</span></span>      | <span data-ttu-id="ff1ff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff1ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff1ff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff1ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff1ff-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff1ff-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff1ff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff1ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff1ff-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-113">Not supported.</span></span>    |
|<span data-ttu-id="ff1ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff1ff-114">Application</span></span> | <span data-ttu-id="ff1ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff1ff-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff1ff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="ff1ff-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff1ff-117">Request headers</span></span>
| <span data-ttu-id="ff1ff-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ff1ff-118">Name</span></span>       | <span data-ttu-id="ff1ff-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ff1ff-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ff1ff-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff1ff-120">Authorization</span></span>  | <span data-ttu-id="ff1ff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff1ff-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff1ff-123">Request body</span></span>
<span data-ttu-id="ff1ff-124">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ff1ff-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff1ff-125">Response</span></span>

<span data-ttu-id="ff1ff-126">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="ff1ff-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ff1ff-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ff1ff-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ff1ff-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff1ff-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff1ff-131">Request</span></span>
<span data-ttu-id="ff1ff-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="ff1ff-133">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-133">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ff1ff-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff1ff-134">Response</span></span>
<span data-ttu-id="ff1ff-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff1ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ff1ff-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ff1ff-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ff1ff-139">C#</span><span class="sxs-lookup"><span data-stu-id="ff1ff-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_plannerbucket_from_planner-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff1ff-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff1ff-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_plannerbucket_from_planner-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ff1ff-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ff1ff-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_plannerbucket_from_planner-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/planner-post-buckets.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/planner-post-buckets.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/planner-post-buckets.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
