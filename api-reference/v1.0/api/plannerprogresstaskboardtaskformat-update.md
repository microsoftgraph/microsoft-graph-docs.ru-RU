---
title: Обновление объекта plannerProgressTaskBoardTaskFormat
description: Обновление свойств объекта **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e31a78844b98080e91ec76e2e6c35ced3c78ac2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967900"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="d3c77-103">Обновление объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d3c77-103">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="d3c77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3c77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3c77-105">Обновление свойств объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d3c77-105">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3c77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3c77-106">Permissions</span></span>
<span data-ttu-id="d3c77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3c77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3c77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3c77-109">Permission type</span></span>      | <span data-ttu-id="d3c77-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3c77-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3c77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3c77-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3c77-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3c77-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3c77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3c77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3c77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3c77-114">Not supported.</span></span>    |
|<span data-ttu-id="d3c77-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3c77-115">Application</span></span> | <span data-ttu-id="d3c77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3c77-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3c77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3c77-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="d3c77-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3c77-118">Optional request headers</span></span>
| <span data-ttu-id="d3c77-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d3c77-119">Name</span></span>       | <span data-ttu-id="d3c77-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d3c77-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d3c77-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3c77-121">Authorization</span></span>  | <span data-ttu-id="d3c77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3c77-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3c77-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="d3c77-124">If-Match</span></span>  | <span data-ttu-id="d3c77-p103">Последнее известное значение ETag обновляемого объекта **plannerProgressTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3c77-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3c77-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3c77-127">Request body</span></span>
<span data-ttu-id="d3c77-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d3c77-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d3c77-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3c77-131">Property</span></span>     | <span data-ttu-id="d3c77-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d3c77-132">Type</span></span>   |<span data-ttu-id="d3c77-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d3c77-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c77-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="d3c77-134">orderHint</span></span>|<span data-ttu-id="d3c77-135">String</span><span class="sxs-lookup"><span data-stu-id="d3c77-135">String</span></span>|<span data-ttu-id="d3c77-p105">Указание, используемое для расположения задачи в окне "Ход выполнения" доски задач. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d3c77-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d3c77-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3c77-138">Response</span></span>

<span data-ttu-id="d3c77-139">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d3c77-139">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="d3c77-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d3c77-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d3c77-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d3c77-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3c77-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3c77-144">Request</span></span>
<span data-ttu-id="d3c77-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3c77-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3c77-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3c77-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="d3c77-147">C#</span><span class="sxs-lookup"><span data-stu-id="d3c77-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3c77-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3c77-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3c77-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3c77-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3c77-150">Java</span><span class="sxs-lookup"><span data-stu-id="d3c77-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerprogresstaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3c77-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3c77-151">Response</span></span>
<span data-ttu-id="d3c77-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3c77-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

