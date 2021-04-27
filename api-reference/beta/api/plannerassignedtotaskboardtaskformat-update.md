---
title: Обновление объекта plannerAssignedToTaskBoardTaskFormat
description: Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: b691c631115b5c66f414c029f2c6172d5aa0d083
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055339"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="171f1-103">Обновление объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="171f1-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="171f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="171f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="171f1-105">Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="171f1-105">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="171f1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="171f1-106">Permissions</span></span>
<span data-ttu-id="171f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="171f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="171f1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="171f1-109">Permission type</span></span>      | <span data-ttu-id="171f1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="171f1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="171f1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="171f1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="171f1-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="171f1-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="171f1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="171f1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="171f1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="171f1-114">Not supported.</span></span>    |
|<span data-ttu-id="171f1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="171f1-115">Application</span></span> | <span data-ttu-id="171f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="171f1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="171f1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="171f1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="171f1-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="171f1-118">Optional request headers</span></span>
| <span data-ttu-id="171f1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="171f1-119">Name</span></span>       | <span data-ttu-id="171f1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="171f1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="171f1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="171f1-121">Authorization</span></span>  | <span data-ttu-id="171f1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="171f1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="171f1-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="171f1-124">If-Match</span></span>  | <span data-ttu-id="171f1-p103">Последнее известное значение ETag обновляемого объекта **plannerAssignedToTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="171f1-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="171f1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="171f1-127">Request body</span></span>
<span data-ttu-id="171f1-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="171f1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="171f1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="171f1-131">Property</span></span>     | <span data-ttu-id="171f1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="171f1-132">Type</span></span>   |<span data-ttu-id="171f1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="171f1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="171f1-134">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="171f1-134">orderHintsByAssignee</span></span>|[<span data-ttu-id="171f1-135">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="171f1-135">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="171f1-136">Словарь подсказок, используемых для заказа задач в представлении AssignedTo для доски задач.</span><span class="sxs-lookup"><span data-stu-id="171f1-136">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="171f1-137">Ключ каждой записи — это один из пользователей, на который назначена задача, а значение — подсказка заказа.</span><span class="sxs-lookup"><span data-stu-id="171f1-137">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="171f1-138">Формат каждого значения определяется в [Using order hints in Planner(.). /resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="171f1-138">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="171f1-139">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="171f1-139">unassignedOrderHint</span></span>|<span data-ttu-id="171f1-140">Строка</span><span class="sxs-lookup"><span data-stu-id="171f1-140">String</span></span>|<span data-ttu-id="171f1-141">Значение подсказки, используемого для заказа задачи в представлении AssignedTo доски задач, когда задача никому не назначена, или если словарь orderHintsByAssignee не предоставляет пользователю подсказку заказа, на которую назначена задача.</span><span class="sxs-lookup"><span data-stu-id="171f1-141">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="171f1-142">Формат определяется в [подсказках по порядку в Planner.](../resources/planner-order-hint-format.md)</span><span class="sxs-lookup"><span data-stu-id="171f1-142">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="171f1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="171f1-143">Response</span></span>

<span data-ttu-id="171f1-144">В случае успешной работы этот метод возвращает `204 No Content` отклик и пустой контент.</span><span class="sxs-lookup"><span data-stu-id="171f1-144">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="171f1-145">Если запрос указывает заголовку с предпочтением, этот метод возвращает код ответа и обновленный объект `Prefer` `return=representation` `200 OK` [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="171f1-145">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="171f1-p108">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="171f1-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="171f1-149">Пример</span><span class="sxs-lookup"><span data-stu-id="171f1-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="171f1-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="171f1-150">Request</span></span>
<span data-ttu-id="171f1-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="171f1-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="171f1-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="171f1-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="171f1-153">C#</span><span class="sxs-lookup"><span data-stu-id="171f1-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="171f1-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="171f1-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="171f1-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="171f1-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="171f1-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="171f1-156">Response</span></span>
<span data-ttu-id="171f1-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="171f1-157">Here is an example of the response.</span></span> <span data-ttu-id="171f1-158">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="171f1-158">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


