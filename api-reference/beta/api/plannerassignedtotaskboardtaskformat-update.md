---
title: Обновление объекта plannerAssignedToTaskBoardTaskFormat
description: Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b3ea3d89356d0a9b312a2c445197ad93e757bf82
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537311"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="4a98d-103">Обновление объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="4a98d-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a98d-104">Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="4a98d-104">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a98d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a98d-105">Permissions</span></span>
<span data-ttu-id="4a98d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a98d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a98d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a98d-108">Permission type</span></span>      | <span data-ttu-id="4a98d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a98d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a98d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a98d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a98d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a98d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a98d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a98d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a98d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a98d-113">Not supported.</span></span>    |
|<span data-ttu-id="4a98d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a98d-114">Application</span></span> | <span data-ttu-id="4a98d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a98d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a98d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a98d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="4a98d-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a98d-117">Optional request headers</span></span>
| <span data-ttu-id="4a98d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4a98d-118">Name</span></span>       | <span data-ttu-id="4a98d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4a98d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4a98d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a98d-120">Authorization</span></span>  | <span data-ttu-id="4a98d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a98d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a98d-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="4a98d-123">If-Match</span></span>  | <span data-ttu-id="4a98d-p103">Последнее известное значение ETag обновляемого объекта **plannerAssignedToTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a98d-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a98d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a98d-126">Request body</span></span>
<span data-ttu-id="4a98d-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4a98d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4a98d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a98d-130">Property</span></span>     | <span data-ttu-id="4a98d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4a98d-131">Type</span></span>   |<span data-ttu-id="4a98d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4a98d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a98d-133">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="4a98d-133">orderHintsByAssignee</span></span>|[<span data-ttu-id="4a98d-134">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="4a98d-134">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="4a98d-135">Словарь подсказок, используемых для упорядочивания задач в представлении AssignedTo доски задач.</span><span class="sxs-lookup"><span data-stu-id="4a98d-135">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="4a98d-136">Ключом каждой записи является один из пользователей, которому назначена задача, а значением является подсказка порядка.</span><span class="sxs-lookup"><span data-stu-id="4a98d-136">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="4a98d-137">Формат каждого значения определяется в разделе [использование подсказок порядка в планировщике (.. /ресаурцес/планнер_ордер_хинт_формат.МД).</span><span class="sxs-lookup"><span data-stu-id="4a98d-137">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="4a98d-138">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="4a98d-138">unassignedOrderHint</span></span>|<span data-ttu-id="4a98d-139">Строка</span><span class="sxs-lookup"><span data-stu-id="4a98d-139">String</span></span>|<span data-ttu-id="4a98d-140">Значение подсказки используется для упорядочивания задачи в представлении AssignedTo доски задач, когда задача не назначена никому, или если словарь Ордерхинтсбяссигни не предоставляет подсказку порядка для пользователя, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="4a98d-140">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="4a98d-141">Формат определяется в разделе [Использование подсказок порядка в планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="4a98d-141">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4a98d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a98d-142">Response</span></span>

<span data-ttu-id="4a98d-143">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a98d-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="4a98d-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4a98d-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4a98d-147">Пример</span><span class="sxs-lookup"><span data-stu-id="4a98d-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a98d-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a98d-148">Request</span></span>
<span data-ttu-id="4a98d-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a98d-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
##### <a name="response"></a><span data-ttu-id="4a98d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a98d-150">Response</span></span>
<span data-ttu-id="4a98d-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a98d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4a98d-154">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4a98d-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a98d-155">C#</span><span class="sxs-lookup"><span data-stu-id="4a98d-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerassignedtotaskboardtaskformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a98d-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a98d-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerassignedtotaskboardtaskformat-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/plannerassignedtotaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannerassignedtotaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
