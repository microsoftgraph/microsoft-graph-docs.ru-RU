---
title: Обновление объекта plannerAssignedToTaskBoardTaskFormat
description: Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.
ms.openlocfilehash: 7bf559b5962c895c1ce7b5d3192ab743bca3acb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077338"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="d9800-103">Обновление объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d9800-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

> <span data-ttu-id="d9800-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d9800-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9800-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9800-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9800-106">Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d9800-106">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9800-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9800-107">Permissions</span></span>
<span data-ttu-id="d9800-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9800-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9800-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9800-110">Permission type</span></span>      | <span data-ttu-id="d9800-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9800-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9800-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9800-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9800-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9800-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9800-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9800-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9800-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9800-115">Not supported.</span></span>    |
|<span data-ttu-id="d9800-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9800-116">Application</span></span> | <span data-ttu-id="d9800-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9800-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9800-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9800-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="d9800-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9800-119">Optional request headers</span></span>
| <span data-ttu-id="d9800-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d9800-120">Name</span></span>       | <span data-ttu-id="d9800-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d9800-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d9800-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9800-122">Authorization</span></span>  | <span data-ttu-id="d9800-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9800-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9800-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="d9800-125">If-Match</span></span>  | <span data-ttu-id="d9800-p104">Последнее известное значение ETag обновляемого объекта **plannerAssignedToTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9800-p104">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9800-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9800-128">Request body</span></span>
<span data-ttu-id="d9800-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d9800-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d9800-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9800-132">Property</span></span>     | <span data-ttu-id="d9800-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d9800-133">Type</span></span>   |<span data-ttu-id="d9800-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d9800-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9800-135">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d9800-135">orderHintsByAssignee</span></span>|[<span data-ttu-id="d9800-136">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d9800-136">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="d9800-137">Словарь подсказки используется для задачи заказа на просмотр AssignedTo панели задач.</span><span class="sxs-lookup"><span data-stu-id="d9800-137">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="d9800-138">Ключ каждой записи — один пользователей, которым назначена эта задача, а значение — подсказка order.</span><span class="sxs-lookup"><span data-stu-id="d9800-138">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="d9800-139">Формат каждое значение определяется в [с помощью подсказки порядке в планировщике (.. / resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="d9800-139">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="d9800-140">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="d9800-140">unassignedOrderHint</span></span>|<span data-ttu-id="d9800-141">String</span><span class="sxs-lookup"><span data-stu-id="d9800-141">String</span></span>|<span data-ttu-id="d9800-142">Присваивается значение подсказку для упорядочивания задачи в представлении AssignedTo Доска задач при всем пользователям, не назначена задача или orderHintsByAssignee словаря не предоставляет подсказку порядке для пользователя задачи.</span><span class="sxs-lookup"><span data-stu-id="d9800-142">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="d9800-143">Формат определяется в [с помощью подсказки порядке в планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d9800-143">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d9800-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9800-144">Response</span></span>

<span data-ttu-id="d9800-145">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d9800-145">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="d9800-p108">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d9800-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d9800-149">Пример</span><span class="sxs-lookup"><span data-stu-id="d9800-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9800-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9800-150">Request</span></span>
<span data-ttu-id="d9800-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9800-151">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d9800-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9800-152">Response</span></span>
<span data-ttu-id="d9800-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d9800-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->