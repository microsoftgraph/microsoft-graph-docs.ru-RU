---
title: Обновление объекта plannerBucketTaskBoardTaskFormat
description: Обновление свойств объекта **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 528dc105ac17ef62b9a1a2d000819e56db13d73e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037734"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="ccbce-103">Обновление объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ccbce-103">Update plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="ccbce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccbce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccbce-105">Обновление свойств объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="ccbce-105">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ccbce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccbce-106">Permissions</span></span>
<span data-ttu-id="ccbce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccbce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccbce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccbce-109">Permission type</span></span>      | <span data-ttu-id="ccbce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccbce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccbce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccbce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ccbce-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccbce-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ccbce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccbce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccbce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccbce-114">Not supported.</span></span>    |
|<span data-ttu-id="ccbce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccbce-115">Application</span></span> | <span data-ttu-id="ccbce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccbce-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccbce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccbce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="ccbce-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccbce-118">Optional request headers</span></span>
| <span data-ttu-id="ccbce-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ccbce-119">Name</span></span>       | <span data-ttu-id="ccbce-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ccbce-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ccbce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccbce-121">Authorization</span></span>  | <span data-ttu-id="ccbce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccbce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccbce-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="ccbce-124">If-Match</span></span>  | <span data-ttu-id="ccbce-p103">Последнее известное значение ETag обновляемого объекта **plannerBucketTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccbce-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccbce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccbce-127">Request body</span></span>
<span data-ttu-id="ccbce-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ccbce-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ccbce-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccbce-131">Property</span></span>     | <span data-ttu-id="ccbce-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ccbce-132">Type</span></span>   |<span data-ttu-id="ccbce-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ccbce-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccbce-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="ccbce-134">orderHint</span></span>|<span data-ttu-id="ccbce-135">String</span><span class="sxs-lookup"><span data-stu-id="ccbce-135">String</span></span>|<span data-ttu-id="ccbce-p105">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="ccbce-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ccbce-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccbce-138">Response</span></span>

<span data-ttu-id="ccbce-139">В случае успешной работы этот метод возвращает `204 No Content` отклик и пустой контент.</span><span class="sxs-lookup"><span data-stu-id="ccbce-139">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="ccbce-140">Если запрос указывает заголовку с предпочтением, этот метод возвращает код ответа и обновленный объект `Prefer` `return=representation` `200 OK` [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ccbce-140">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="ccbce-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ccbce-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ccbce-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ccbce-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccbce-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccbce-145">Request</span></span>
<span data-ttu-id="ccbce-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccbce-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ccbce-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccbce-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="ccbce-148">C#</span><span class="sxs-lookup"><span data-stu-id="ccbce-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccbce-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccbce-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccbce-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccbce-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccbce-151">Java</span><span class="sxs-lookup"><span data-stu-id="ccbce-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbuckettaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ccbce-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccbce-152">Response</span></span>
<span data-ttu-id="ccbce-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccbce-153">Here is an example of the response.</span></span> <span data-ttu-id="ccbce-154">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ccbce-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


