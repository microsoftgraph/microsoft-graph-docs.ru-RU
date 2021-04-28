---
title: Обновление объекта plannerAssignedToTaskBoardTaskFormat
description: Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: b8b3c2c1cfe2c415400363e5b8951b5dd8ed1037
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054506"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="bd5ab-103">Обновление объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="bd5ab-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="bd5ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd5ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd5ab-105">Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-105">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd5ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd5ab-106">Permissions</span></span>
<span data-ttu-id="bd5ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd5ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd5ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd5ab-109">Permission type</span></span>      | <span data-ttu-id="bd5ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd5ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd5ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd5ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bd5ab-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd5ab-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd5ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd5ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd5ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-114">Not supported.</span></span>    |
|<span data-ttu-id="bd5ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd5ab-115">Application</span></span> | <span data-ttu-id="bd5ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd5ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd5ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="bd5ab-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd5ab-118">Optional request headers</span></span>
| <span data-ttu-id="bd5ab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bd5ab-119">Name</span></span>       | <span data-ttu-id="bd5ab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5ab-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bd5ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd5ab-121">Authorization</span></span>  | <span data-ttu-id="bd5ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd5ab-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="bd5ab-124">If-Match</span></span>  | <span data-ttu-id="bd5ab-p103">Последнее известное значение ETag обновляемого объекта **plannerAssignedToTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd5ab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd5ab-127">Request body</span></span>
<span data-ttu-id="bd5ab-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bd5ab-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd5ab-131">Property</span></span>     | <span data-ttu-id="bd5ab-132">Тип</span><span class="sxs-lookup"><span data-stu-id="bd5ab-132">Type</span></span>   |<span data-ttu-id="bd5ab-133">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5ab-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd5ab-134">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="bd5ab-134">orderHintsByAssignee</span></span>|[<span data-ttu-id="bd5ab-135">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="bd5ab-135">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="bd5ab-p105">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ab-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="bd5ab-139">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="bd5ab-139">unassignedOrderHint</span></span>|<span data-ttu-id="bd5ab-140">Строка</span><span class="sxs-lookup"><span data-stu-id="bd5ab-140">String</span></span>|<span data-ttu-id="bd5ab-p106">Указание, используемое для расположения задачи в окне "Кому назначено" доски задач, когда задача никому не назначена, или если в словаре orderHintsByAssignee нет указания order для пользователя, которому назначена задача. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ab-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="bd5ab-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd5ab-143">Response</span></span>

<span data-ttu-id="bd5ab-144">В случае успешной работы этот метод возвращает `204 No Content` отклик и пустой контент.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-144">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="bd5ab-145">Если запрос указывает заголовку с предпочтением, этот метод возвращает код ответа и обновленный объект `Prefer` `return=representation` `200 OK` [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-145">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="bd5ab-p108">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="bd5ab-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="bd5ab-149">Пример</span><span class="sxs-lookup"><span data-stu-id="bd5ab-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd5ab-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd5ab-150">Request</span></span>
<span data-ttu-id="bd5ab-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd5ab-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd5ab-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
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
# <a name="c"></a>[<span data-ttu-id="bd5ab-153">C#</span><span class="sxs-lookup"><span data-stu-id="bd5ab-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd5ab-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd5ab-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd5ab-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd5ab-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd5ab-156">Java</span><span class="sxs-lookup"><span data-stu-id="bd5ab-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerassignedtotaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bd5ab-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd5ab-157">Response</span></span>
<span data-ttu-id="bd5ab-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-158">Here is an example of the response.</span></span> <span data-ttu-id="bd5ab-159">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd5ab-159">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

