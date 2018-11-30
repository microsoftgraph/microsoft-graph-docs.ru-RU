---
title: Обновление объекта plannerbucket
description: Обновление свойств объекта **plannerbucket**.
ms.openlocfilehash: 88c4cd83be2c76ab7f7d220d4a35bd5b90f7edb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026797"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="4cb4e-103">Обновление объекта plannerbucket</span><span class="sxs-lookup"><span data-stu-id="4cb4e-103">Update plannerbucket</span></span>

<span data-ttu-id="4cb4e-104">Обновление свойств объекта **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-104">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cb4e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cb4e-105">Permissions</span></span>
<span data-ttu-id="4cb4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cb4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb4e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cb4e-108">Permission type</span></span>      | <span data-ttu-id="4cb4e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cb4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cb4e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cb4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4cb4e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cb4e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4cb4e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cb4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cb4e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-113">Not supported.</span></span>    |
|<span data-ttu-id="4cb4e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cb4e-114">Application</span></span> | <span data-ttu-id="4cb4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cb4e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cb4e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4cb4e-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cb4e-117">Optional request headers</span></span>
| <span data-ttu-id="4cb4e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4cb4e-118">Name</span></span>       | <span data-ttu-id="4cb4e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb4e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4cb4e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cb4e-120">Authorization</span></span>  | <span data-ttu-id="4cb4e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cb4e-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="4cb4e-123">If-Match</span></span>  | <span data-ttu-id="4cb4e-p103">Последнее известное значение ETag обновляемого объекта **plannerBucket**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cb4e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cb4e-126">Request body</span></span>
<span data-ttu-id="4cb4e-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4cb4e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cb4e-130">Property</span></span>     | <span data-ttu-id="4cb4e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4cb4e-131">Type</span></span>   |<span data-ttu-id="4cb4e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb4e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cb4e-133">name</span><span class="sxs-lookup"><span data-stu-id="4cb4e-133">name</span></span>|<span data-ttu-id="4cb4e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4cb4e-134">String</span></span>|<span data-ttu-id="4cb4e-135">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-135">Name of the bucket.</span></span>|
|<span data-ttu-id="4cb4e-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="4cb4e-136">orderHint</span></span>|<span data-ttu-id="4cb4e-137">String</span><span class="sxs-lookup"><span data-stu-id="4cb4e-137">String</span></span>|<span data-ttu-id="4cb4e-p105">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="4cb4e-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="4cb4e-140">planId</span><span class="sxs-lookup"><span data-stu-id="4cb4e-140">planId</span></span>|<span data-ttu-id="4cb4e-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4cb4e-141">String</span></span>|<span data-ttu-id="4cb4e-142">Идентификатор плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-142">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="4cb4e-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cb4e-143">Response</span></span>

<span data-ttu-id="4cb4e-144">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-144">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="4cb4e-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4cb4e-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4cb4e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4cb4e-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cb4e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cb4e-149">Request</span></span>
<span data-ttu-id="4cb4e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cb4e-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="4cb4e-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cb4e-151">Response</span></span>
<span data-ttu-id="4cb4e-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4cb4e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->