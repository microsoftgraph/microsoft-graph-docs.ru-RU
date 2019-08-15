---
title: Обновление объекта plannerProgressTaskBoardTaskFormat
description: Обновление свойств объекта **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 3c390c72c2e770a547cbc634cfcf89c6866bcf84
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413163"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="d94c3-103">Обновление объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d94c3-103">Update plannerProgressTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d94c3-104">Обновление свойств объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d94c3-104">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d94c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d94c3-105">Permissions</span></span>
<span data-ttu-id="d94c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d94c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d94c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d94c3-108">Permission type</span></span>      | <span data-ttu-id="d94c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d94c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d94c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d94c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d94c3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d94c3-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d94c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d94c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d94c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d94c3-113">Not supported.</span></span>    |
|<span data-ttu-id="d94c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d94c3-114">Application</span></span> | <span data-ttu-id="d94c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d94c3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d94c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d94c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="d94c3-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d94c3-117">Optional request headers</span></span>
| <span data-ttu-id="d94c3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d94c3-118">Name</span></span>       | <span data-ttu-id="d94c3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d94c3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d94c3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d94c3-120">Authorization</span></span>  | <span data-ttu-id="d94c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d94c3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d94c3-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="d94c3-123">If-Match</span></span>  | <span data-ttu-id="d94c3-p103">Последнее известное значение ETag обновляемого объекта **plannerProgressTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d94c3-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d94c3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d94c3-126">Request body</span></span>
<span data-ttu-id="d94c3-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d94c3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d94c3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d94c3-130">Property</span></span>     | <span data-ttu-id="d94c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d94c3-131">Type</span></span>   |<span data-ttu-id="d94c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d94c3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d94c3-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="d94c3-133">orderHint</span></span>|<span data-ttu-id="d94c3-134">String</span><span class="sxs-lookup"><span data-stu-id="d94c3-134">String</span></span>|<span data-ttu-id="d94c3-135">Значение подсказки, используемое для упорядочивания задачи в представлении "ход выполнения" доски задач.</span><span class="sxs-lookup"><span data-stu-id="d94c3-135">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="d94c3-136">Формат определяется в разделе [Использование подсказок порядка в планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d94c3-136">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d94c3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d94c3-137">Response</span></span>

<span data-ttu-id="d94c3-138">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d94c3-138">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="d94c3-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d94c3-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d94c3-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d94c3-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d94c3-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d94c3-143">Request</span></span>
<span data-ttu-id="d94c3-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d94c3-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d94c3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d94c3-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d94c3-146">C#</span><span class="sxs-lookup"><span data-stu-id="d94c3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d94c3-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d94c3-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d94c3-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d94c3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d94c3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d94c3-149">Response</span></span>
<span data-ttu-id="d94c3-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d94c3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
