---
title: Обновление объекта plannerbucket
description: Обновление свойств объекта **plannerbucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 99694abe6e8640d821e116a204328f4f69cfdba8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053960"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="c3c26-103">Обновление объекта plannerbucket</span><span class="sxs-lookup"><span data-stu-id="c3c26-103">Update plannerbucket</span></span>

<span data-ttu-id="c3c26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3c26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3c26-105">Обновление свойств объекта **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="c3c26-105">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3c26-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3c26-106">Permissions</span></span>
<span data-ttu-id="c3c26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3c26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3c26-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3c26-109">Permission type</span></span>      | <span data-ttu-id="c3c26-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3c26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3c26-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3c26-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3c26-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3c26-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3c26-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3c26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3c26-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c26-114">Not supported.</span></span>    |
|<span data-ttu-id="c3c26-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3c26-115">Application</span></span> | <span data-ttu-id="c3c26-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c26-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3c26-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3c26-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c3c26-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3c26-118">Optional request headers</span></span>
| <span data-ttu-id="c3c26-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c3c26-119">Name</span></span>       | <span data-ttu-id="c3c26-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c3c26-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c3c26-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3c26-121">Authorization</span></span>  | <span data-ttu-id="c3c26-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3c26-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3c26-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="c3c26-124">If-Match</span></span>  | <span data-ttu-id="c3c26-p103">Последнее известное значение ETag обновляемого объекта **plannerBucket**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3c26-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3c26-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3c26-127">Request body</span></span>
<span data-ttu-id="c3c26-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c3c26-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c3c26-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3c26-131">Property</span></span>     | <span data-ttu-id="c3c26-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c3c26-132">Type</span></span>   |<span data-ttu-id="c3c26-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c3c26-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3c26-134">name</span><span class="sxs-lookup"><span data-stu-id="c3c26-134">name</span></span>|<span data-ttu-id="c3c26-135">String</span><span class="sxs-lookup"><span data-stu-id="c3c26-135">String</span></span>|<span data-ttu-id="c3c26-136">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="c3c26-136">Name of the bucket.</span></span>|
|<span data-ttu-id="c3c26-137">orderHint</span><span class="sxs-lookup"><span data-stu-id="c3c26-137">orderHint</span></span>|<span data-ttu-id="c3c26-138">String</span><span class="sxs-lookup"><span data-stu-id="c3c26-138">String</span></span>|<span data-ttu-id="c3c26-p105">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c3c26-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="c3c26-141">planId</span><span class="sxs-lookup"><span data-stu-id="c3c26-141">planId</span></span>|<span data-ttu-id="c3c26-142">Строка</span><span class="sxs-lookup"><span data-stu-id="c3c26-142">String</span></span>|<span data-ttu-id="c3c26-143">Идентификатор плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="c3c26-143">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="c3c26-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3c26-144">Response</span></span>

<span data-ttu-id="c3c26-145">В случае успешной работы этот метод возвращает `204 No Content` отклик и пустой контент.</span><span class="sxs-lookup"><span data-stu-id="c3c26-145">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="c3c26-146">Если запрос указывает заголовку с предпочтением, этот метод возвращает код ответа и обновленный `Prefer` `return=representation` объект `200 OK` [plannerBucket](../resources/plannerbucket.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c3c26-146">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="c3c26-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c3c26-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c3c26-150">Пример</span><span class="sxs-lookup"><span data-stu-id="c3c26-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3c26-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3c26-151">Request</span></span>
<span data-ttu-id="c3c26-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3c26-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3c26-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3c26-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
Content-type: application/json
Content-length: 27
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
# <a name="c"></a>[<span data-ttu-id="c3c26-154">C#</span><span class="sxs-lookup"><span data-stu-id="c3c26-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3c26-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3c26-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3c26-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3c26-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3c26-157">Java</span><span class="sxs-lookup"><span data-stu-id="c3c26-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3c26-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3c26-158">Response</span></span>
<span data-ttu-id="c3c26-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3c26-159">Here is an example of the response.</span></span> <span data-ttu-id="c3c26-160">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3c26-160">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

