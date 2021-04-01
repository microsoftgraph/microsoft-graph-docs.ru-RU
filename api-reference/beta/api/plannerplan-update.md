---
title: Планировщик обновленияPlan
description: Обновление свойств объекта **plannerPlan.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 0ac2b6e80a8111beb65c75c21bd7a93ae68738d3
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473943"
---
# <a name="update-plannerplan"></a><span data-ttu-id="9b46c-103">Планировщик обновленияPlan</span><span class="sxs-lookup"><span data-stu-id="9b46c-103">Update plannerPlan</span></span>

<span data-ttu-id="9b46c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b46c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b46c-105">Обновление свойств объекта **plannerPlan.**</span><span class="sxs-lookup"><span data-stu-id="9b46c-105">Update the properties of a **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b46c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b46c-106">Permissions</span></span>
<span data-ttu-id="9b46c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b46c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b46c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b46c-109">Permission type</span></span>      | <span data-ttu-id="9b46c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b46c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b46c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b46c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b46c-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b46c-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9b46c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b46c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b46c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b46c-114">Not supported.</span></span>    |
|<span data-ttu-id="9b46c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b46c-115">Application</span></span> | <span data-ttu-id="9b46c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b46c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b46c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b46c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{plan-id}
```

## <a name="request-headers"></a><span data-ttu-id="9b46c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b46c-118">Request headers</span></span>

| <span data-ttu-id="9b46c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9b46c-119">Name</span></span>       | <span data-ttu-id="9b46c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9b46c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9b46c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b46c-121">Authorization</span></span>  | <span data-ttu-id="9b46c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b46c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b46c-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="9b46c-124">If-Match</span></span>  | <span data-ttu-id="9b46c-p103">Последнее известное значение ETag обновляемого объекта plannerPlan. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b46c-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b46c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b46c-127">Request body</span></span>
<span data-ttu-id="9b46c-128">В теле запроса укажи значения для обновления соответствующих полей.</span><span class="sxs-lookup"><span data-stu-id="9b46c-128">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="9b46c-129">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="9b46c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9b46c-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9b46c-130">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="9b46c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b46c-131">Response</span></span>

<span data-ttu-id="9b46c-132">В случае успешной работы этот метод возвращает `204 No Content` отклик и пустой контент.</span><span class="sxs-lookup"><span data-stu-id="9b46c-132">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="9b46c-133">Если запрос указывает заголовщик с предпочтением, этот метод возвращает код ответа и обновленный объект `Prefer` `return=representation` `200 OK` [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9b46c-133">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and an updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="9b46c-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9b46c-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9b46c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9b46c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b46c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b46c-138">Request</span></span>
<span data-ttu-id="9b46c-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b46c-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b46c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b46c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/{id}
Content-type: application/json
Content-length: 29
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
# <a name="c"></a>[<span data-ttu-id="9b46c-141">C#</span><span class="sxs-lookup"><span data-stu-id="9b46c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b46c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b46c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b46c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b46c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b46c-144">Java</span><span class="sxs-lookup"><span data-stu-id="9b46c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9b46c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b46c-145">Response</span></span>
<span data-ttu-id="9b46c-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b46c-146">Here is an example of the response.</span></span> 

><span data-ttu-id="9b46c-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b46c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874",
    "containerId": "ebf3b108-5234-4e22-b93d-656d7dae5874",
    "type": "group"
  },
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


