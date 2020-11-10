---
title: Обновление объекта plannerBucketTaskBoardTaskFormat
description: Обновление свойств объекта **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f98bc9733aef4c2fb6122669857dc9d32118b5f4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981812"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="84d69-103">Обновление объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="84d69-103">Update plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="84d69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84d69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84d69-105">Обновление свойств объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="84d69-105">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="84d69-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84d69-106">Permissions</span></span>
<span data-ttu-id="84d69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84d69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84d69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84d69-109">Permission type</span></span>      | <span data-ttu-id="84d69-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84d69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84d69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84d69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84d69-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84d69-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="84d69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84d69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84d69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84d69-114">Not supported.</span></span>    |
|<span data-ttu-id="84d69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84d69-115">Application</span></span> | <span data-ttu-id="84d69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84d69-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84d69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84d69-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="84d69-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84d69-118">Optional request headers</span></span>
| <span data-ttu-id="84d69-119">Имя</span><span class="sxs-lookup"><span data-stu-id="84d69-119">Name</span></span>       | <span data-ttu-id="84d69-120">Описание</span><span class="sxs-lookup"><span data-stu-id="84d69-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="84d69-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84d69-121">Authorization</span></span>  | <span data-ttu-id="84d69-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84d69-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84d69-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="84d69-124">If-Match</span></span>  | <span data-ttu-id="84d69-p103">Последнее известное значение ETag обновляемого объекта **plannerBucketTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84d69-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84d69-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84d69-127">Request body</span></span>
<span data-ttu-id="84d69-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="84d69-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="84d69-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="84d69-131">Property</span></span>     | <span data-ttu-id="84d69-132">Тип</span><span class="sxs-lookup"><span data-stu-id="84d69-132">Type</span></span>   |<span data-ttu-id="84d69-133">Описание</span><span class="sxs-lookup"><span data-stu-id="84d69-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84d69-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="84d69-134">orderHint</span></span>|<span data-ttu-id="84d69-135">String</span><span class="sxs-lookup"><span data-stu-id="84d69-135">String</span></span>|<span data-ttu-id="84d69-p105">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="84d69-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="84d69-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="84d69-138">Response</span></span>

<span data-ttu-id="84d69-139">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="84d69-139">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="84d69-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="84d69-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="84d69-143">Пример</span><span class="sxs-lookup"><span data-stu-id="84d69-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84d69-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="84d69-144">Request</span></span>
<span data-ttu-id="84d69-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84d69-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84d69-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="84d69-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="84d69-147">C#</span><span class="sxs-lookup"><span data-stu-id="84d69-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84d69-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84d69-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84d69-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84d69-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84d69-150">Java</span><span class="sxs-lookup"><span data-stu-id="84d69-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbuckettaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84d69-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="84d69-151">Response</span></span>
<span data-ttu-id="84d69-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84d69-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


