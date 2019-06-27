---
title: Обновление объекта plannerBucketTaskBoardTaskFormat
description: Обновление свойств объекта **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9ced18dde9e8106f47c0a75cfb4c6785ab58e750
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268315"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="fe373-103">Обновление объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="fe373-103">Update plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe373-104">Обновление свойств объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="fe373-104">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe373-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe373-105">Permissions</span></span>
<span data-ttu-id="fe373-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe373-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe373-108">Permission type</span></span>      | <span data-ttu-id="fe373-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe373-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe373-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe373-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe373-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe373-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe373-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe373-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe373-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe373-113">Not supported.</span></span>    |
|<span data-ttu-id="fe373-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe373-114">Application</span></span> | <span data-ttu-id="fe373-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe373-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe373-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe373-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="fe373-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe373-117">Optional request headers</span></span>
| <span data-ttu-id="fe373-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fe373-118">Name</span></span>       | <span data-ttu-id="fe373-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fe373-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fe373-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe373-120">Authorization</span></span>  | <span data-ttu-id="fe373-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe373-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe373-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="fe373-123">If-Match</span></span>  | <span data-ttu-id="fe373-p103">Последнее известное значение ETag обновляемого объекта **plannerBucketTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe373-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe373-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe373-126">Request body</span></span>
<span data-ttu-id="fe373-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fe373-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fe373-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe373-130">Property</span></span>     | <span data-ttu-id="fe373-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe373-131">Type</span></span>   |<span data-ttu-id="fe373-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe373-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe373-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="fe373-133">orderHint</span></span>|<span data-ttu-id="fe373-134">String</span><span class="sxs-lookup"><span data-stu-id="fe373-134">String</span></span>|<span data-ttu-id="fe373-p105">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="fe373-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="fe373-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe373-137">Response</span></span>

<span data-ttu-id="fe373-138">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fe373-138">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="fe373-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="fe373-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="fe373-142">Пример</span><span class="sxs-lookup"><span data-stu-id="fe373-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe373-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe373-143">Request</span></span>
<span data-ttu-id="fe373-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe373-144">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fe373-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe373-145">Response</span></span>
<span data-ttu-id="fe373-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe373-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fe373-149">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fe373-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fe373-150">C#</span><span class="sxs-lookup"><span data-stu-id="fe373-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerbuckettaskboardtaskformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe373-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="fe373-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerbuckettaskboardtaskformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fe373-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fe373-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_plannerbuckettaskboardtaskformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
