---
title: Обновление объекта plannerAssignedToTaskBoardTaskFormat
description: Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9133a12b93d1bfa3c8c9406711510f7061f6d8b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562036"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="3125b-103">Обновление объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3125b-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="3125b-104">Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="3125b-104">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3125b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3125b-105">Permissions</span></span>
<span data-ttu-id="3125b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3125b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3125b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3125b-108">Permission type</span></span>      | <span data-ttu-id="3125b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3125b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3125b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3125b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3125b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3125b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3125b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3125b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3125b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3125b-113">Not supported.</span></span>    |
|<span data-ttu-id="3125b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3125b-114">Application</span></span> | <span data-ttu-id="3125b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3125b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3125b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3125b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="3125b-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3125b-117">Optional request headers</span></span>
| <span data-ttu-id="3125b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3125b-118">Name</span></span>       | <span data-ttu-id="3125b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3125b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3125b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3125b-120">Authorization</span></span>  | <span data-ttu-id="3125b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3125b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3125b-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="3125b-123">If-Match</span></span>  | <span data-ttu-id="3125b-p103">Последнее известное значение ETag обновляемого объекта **plannerAssignedToTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3125b-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3125b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3125b-126">Request body</span></span>
<span data-ttu-id="3125b-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3125b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3125b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3125b-130">Property</span></span>     | <span data-ttu-id="3125b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3125b-131">Type</span></span>   |<span data-ttu-id="3125b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3125b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3125b-133">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="3125b-133">orderHintsByAssignee</span></span>|[<span data-ttu-id="3125b-134">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="3125b-134">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="3125b-p105">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="3125b-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="3125b-138">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="3125b-138">unassignedOrderHint</span></span>|<span data-ttu-id="3125b-139">Строка</span><span class="sxs-lookup"><span data-stu-id="3125b-139">String</span></span>|<span data-ttu-id="3125b-p106">Указание, используемое для расположения задачи в окне "Кому назначено" доски задач, когда задача никому не назначена, или если в словаре orderHintsByAssignee нет указания order для пользователя, которому назначена задача. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="3125b-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="3125b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3125b-142">Response</span></span>

<span data-ttu-id="3125b-143">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3125b-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="3125b-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="3125b-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3125b-147">Пример</span><span class="sxs-lookup"><span data-stu-id="3125b-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3125b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="3125b-148">Request</span></span>
<span data-ttu-id="3125b-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3125b-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
##### <a name="response"></a><span data-ttu-id="3125b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3125b-150">Response</span></span>
<span data-ttu-id="3125b-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3125b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
