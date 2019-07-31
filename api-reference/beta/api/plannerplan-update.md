---
title: Обновление plannerPlan
description: Обновление свойств объекта **plannerPlan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 65233ac4976c5e495dc9d0a6ef60d6605ab34305
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979050"
---
# <a name="update-plannerplan"></a><span data-ttu-id="3556c-103">Обновление plannerPlan</span><span class="sxs-lookup"><span data-stu-id="3556c-103">Update plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3556c-104">Обновление свойств объекта **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="3556c-104">Update the properties of a **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3556c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3556c-105">Permissions</span></span>
<span data-ttu-id="3556c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3556c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3556c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3556c-108">Permission type</span></span>      | <span data-ttu-id="3556c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3556c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3556c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3556c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3556c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3556c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3556c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3556c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3556c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3556c-113">Not supported.</span></span>    |
|<span data-ttu-id="3556c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3556c-114">Application</span></span> | <span data-ttu-id="3556c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3556c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3556c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3556c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{plan-id}
```

## <a name="request-headers"></a><span data-ttu-id="3556c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3556c-117">Request headers</span></span>

| <span data-ttu-id="3556c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3556c-118">Name</span></span>       | <span data-ttu-id="3556c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3556c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3556c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3556c-120">Authorization</span></span>  | <span data-ttu-id="3556c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3556c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3556c-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="3556c-123">If-Match</span></span>  | <span data-ttu-id="3556c-p103">Последнее известное значение ETag обновляемого объекта plannerPlan. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3556c-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3556c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3556c-126">Request body</span></span>
<span data-ttu-id="3556c-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3556c-127">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="3556c-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3556c-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3556c-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3556c-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3556c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3556c-130">Property</span></span>     | <span data-ttu-id="3556c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3556c-131">Type</span></span>   |<span data-ttu-id="3556c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3556c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3556c-133">owner</span><span class="sxs-lookup"><span data-stu-id="3556c-133">owner</span></span>|<span data-ttu-id="3556c-134">String</span><span class="sxs-lookup"><span data-stu-id="3556c-134">String</span></span>|<span data-ttu-id="3556c-p105">Идентификатор `id` [группы](../resources/group.md), которой принадлежит план. Чтобы в этом поле можно было указать значение, должна существовать подходящая группа. Указанное значение может изменить только владелец.</span><span class="sxs-lookup"><span data-stu-id="3556c-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="3556c-138">title</span><span class="sxs-lookup"><span data-stu-id="3556c-138">title</span></span>|<span data-ttu-id="3556c-139">String</span><span class="sxs-lookup"><span data-stu-id="3556c-139">String</span></span>|<span data-ttu-id="3556c-140">Название плана.</span><span class="sxs-lookup"><span data-stu-id="3556c-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="3556c-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="3556c-141">Response</span></span>

<span data-ttu-id="3556c-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [plannerPlan](../resources/plannerplan.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3556c-142">If successful, this method returns a `200 OK` response code and an updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="3556c-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="3556c-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3556c-146">Пример</span><span class="sxs-lookup"><span data-stu-id="3556c-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3556c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="3556c-147">Request</span></span>
<span data-ttu-id="3556c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3556c-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3556c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="3556c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/<id>
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3556c-150">C#</span><span class="sxs-lookup"><span data-stu-id="3556c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3556c-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="3556c-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3556c-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3556c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3556c-153">Java</span><span class="sxs-lookup"><span data-stu-id="3556c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3556c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="3556c-154">Response</span></span>
<span data-ttu-id="3556c-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3556c-155">Here is an example of the response.</span></span> 

><span data-ttu-id="3556c-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3556c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
