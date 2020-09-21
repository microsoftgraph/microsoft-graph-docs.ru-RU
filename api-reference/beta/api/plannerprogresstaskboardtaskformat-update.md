---
title: Обновление объекта plannerProgressTaskBoardTaskFormat
description: Обновление свойств объекта **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 022668412ee3f511ac69de46e342dcf24798d1e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966837"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="f1a50-103">Обновление объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f1a50-103">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="f1a50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1a50-105">Обновление свойств объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="f1a50-105">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1a50-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a50-106">Permissions</span></span>
<span data-ttu-id="f1a50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a50-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a50-109">Permission type</span></span>      | <span data-ttu-id="f1a50-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1a50-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1a50-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1a50-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f1a50-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a50-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1a50-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1a50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a50-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a50-114">Not supported.</span></span>    |
|<span data-ttu-id="f1a50-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1a50-115">Application</span></span> | <span data-ttu-id="f1a50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a50-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1a50-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1a50-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="f1a50-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1a50-118">Optional request headers</span></span>
| <span data-ttu-id="f1a50-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f1a50-119">Name</span></span>       | <span data-ttu-id="f1a50-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a50-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f1a50-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1a50-121">Authorization</span></span>  | <span data-ttu-id="f1a50-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a50-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1a50-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="f1a50-124">If-Match</span></span>  | <span data-ttu-id="f1a50-p103">Последнее известное значение ETag обновляемого объекта **plannerProgressTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a50-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1a50-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1a50-127">Request body</span></span>
<span data-ttu-id="f1a50-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f1a50-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f1a50-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1a50-131">Property</span></span>     | <span data-ttu-id="f1a50-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f1a50-132">Type</span></span>   |<span data-ttu-id="f1a50-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a50-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1a50-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="f1a50-134">orderHint</span></span>|<span data-ttu-id="f1a50-135">String</span><span class="sxs-lookup"><span data-stu-id="f1a50-135">String</span></span>|<span data-ttu-id="f1a50-136">Значение подсказки, используемое для упорядочивания задачи в представлении "ход выполнения" доски задач.</span><span class="sxs-lookup"><span data-stu-id="f1a50-136">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="f1a50-137">Формат определяется в разделе [Использование подсказок порядка в планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="f1a50-137">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="f1a50-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a50-138">Response</span></span>

<span data-ttu-id="f1a50-139">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f1a50-139">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="f1a50-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f1a50-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f1a50-143">Пример</span><span class="sxs-lookup"><span data-stu-id="f1a50-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1a50-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1a50-144">Request</span></span>
<span data-ttu-id="f1a50-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a50-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1a50-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a50-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/{id}/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="f1a50-147">C#</span><span class="sxs-lookup"><span data-stu-id="f1a50-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1a50-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1a50-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1a50-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1a50-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1a50-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a50-150">Response</span></span>
<span data-ttu-id="f1a50-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1a50-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


