---
title: Обновление plannerPlan
description: Обновление свойств объекта **plannerPlan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: c9dda21c2cedb31d681d64a16ff0e4d1fdf9387e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020693"
---
# <a name="update-plannerplan"></a><span data-ttu-id="f0e2d-103">Обновление plannerPlan</span><span class="sxs-lookup"><span data-stu-id="f0e2d-103">Update plannerPlan</span></span>

<span data-ttu-id="f0e2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0e2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0e2d-105">Обновление свойств объекта **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="f0e2d-105">Update the properties of a **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0e2d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0e2d-106">Permissions</span></span>
<span data-ttu-id="f0e2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0e2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0e2d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0e2d-109">Permission type</span></span>      | <span data-ttu-id="f0e2d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0e2d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0e2d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0e2d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0e2d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0e2d-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0e2d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0e2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0e2d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-114">Not supported.</span></span>    |
|<span data-ttu-id="f0e2d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0e2d-115">Application</span></span> | <span data-ttu-id="f0e2d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0e2d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0e2d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{plan-id}
```

## <a name="request-headers"></a><span data-ttu-id="f0e2d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0e2d-118">Request headers</span></span>

| <span data-ttu-id="f0e2d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f0e2d-119">Name</span></span>       | <span data-ttu-id="f0e2d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f0e2d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f0e2d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0e2d-121">Authorization</span></span>  | <span data-ttu-id="f0e2d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0e2d-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="f0e2d-124">If-Match</span></span>  | <span data-ttu-id="f0e2d-p103">Последнее известное значение ETag обновляемого объекта plannerPlan. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0e2d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0e2d-127">Request body</span></span>
<span data-ttu-id="f0e2d-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-128">In the request body, supply the values for relevant fields to updated.</span></span> <span data-ttu-id="f0e2d-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f0e2d-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f0e2d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0e2d-131">Property</span></span>     | <span data-ttu-id="f0e2d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f0e2d-132">Type</span></span>   |<span data-ttu-id="f0e2d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f0e2d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0e2d-134">owner</span><span class="sxs-lookup"><span data-stu-id="f0e2d-134">owner</span></span>|<span data-ttu-id="f0e2d-135">String</span><span class="sxs-lookup"><span data-stu-id="f0e2d-135">String</span></span>|<span data-ttu-id="f0e2d-p105">Идентификатор `id` [группы](../resources/group.md), которой принадлежит план. Чтобы в этом поле можно было указать значение, должна существовать подходящая группа. Указанное значение может изменить только владелец.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="f0e2d-139">title</span><span class="sxs-lookup"><span data-stu-id="f0e2d-139">title</span></span>|<span data-ttu-id="f0e2d-140">String</span><span class="sxs-lookup"><span data-stu-id="f0e2d-140">String</span></span>|<span data-ttu-id="f0e2d-141">Название плана.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-141">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="f0e2d-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0e2d-142">Response</span></span>

<span data-ttu-id="f0e2d-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [plannerPlan](../resources/plannerplan.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-143">If successful, this method returns a `200 OK` response code and an updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="f0e2d-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f0e2d-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f0e2d-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f0e2d-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0e2d-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0e2d-148">Request</span></span>
<span data-ttu-id="f0e2d-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0e2d-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0e2d-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f0e2d-151">C#</span><span class="sxs-lookup"><span data-stu-id="f0e2d-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0e2d-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0e2d-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0e2d-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0e2d-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0e2d-154">Java</span><span class="sxs-lookup"><span data-stu-id="f0e2d-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0e2d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0e2d-155">Response</span></span>
<span data-ttu-id="f0e2d-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-156">Here is an example of the response.</span></span> 

><span data-ttu-id="f0e2d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0e2d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

