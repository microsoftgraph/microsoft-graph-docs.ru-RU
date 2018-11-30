---
title: Обновление объекта plannerbucket
description: Обновление свойств объекта **plannerbucket**.
ms.openlocfilehash: 22414bb7aaa3155974679a765eb4b83f1c98fd6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079983"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="1b5c4-103">Обновление объекта plannerbucket</span><span class="sxs-lookup"><span data-stu-id="1b5c4-103">Update plannerbucket</span></span>

> <span data-ttu-id="1b5c4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b5c4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b5c4-106">Обновление свойств объекта **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-106">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b5c4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5c4-107">Permissions</span></span>
<span data-ttu-id="1b5c4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b5c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b5c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5c4-110">Permission type</span></span>      | <span data-ttu-id="1b5c4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b5c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b5c4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5c4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b5c4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b5c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b5c4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-115">Not supported.</span></span>    |
|<span data-ttu-id="1b5c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b5c4-116">Application</span></span> | <span data-ttu-id="1b5c4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b5c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b5c4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="1b5c4-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b5c4-119">Optional request headers</span></span>
| <span data-ttu-id="1b5c4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1b5c4-120">Name</span></span>       | <span data-ttu-id="1b5c4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1b5c4-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1b5c4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b5c4-122">Authorization</span></span>  | <span data-ttu-id="1b5c4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b5c4-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="1b5c4-125">If-Match</span></span>  | <span data-ttu-id="1b5c4-p104">Последнее известное значение ETag обновляемого объекта **plannerBucket**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-p104">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b5c4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b5c4-128">Request body</span></span>
<span data-ttu-id="1b5c4-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1b5c4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b5c4-132">Property</span></span>     | <span data-ttu-id="1b5c4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1b5c4-133">Type</span></span>   |<span data-ttu-id="1b5c4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1b5c4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b5c4-135">name</span><span class="sxs-lookup"><span data-stu-id="1b5c4-135">name</span></span>|<span data-ttu-id="1b5c4-136">Строка</span><span class="sxs-lookup"><span data-stu-id="1b5c4-136">String</span></span>|<span data-ttu-id="1b5c4-137">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-137">Name of the bucket.</span></span>|
|<span data-ttu-id="1b5c4-138">orderHint</span><span class="sxs-lookup"><span data-stu-id="1b5c4-138">orderHint</span></span>|<span data-ttu-id="1b5c4-139">String</span><span class="sxs-lookup"><span data-stu-id="1b5c4-139">String</span></span>|<span data-ttu-id="1b5c4-p106">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="1b5c4-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="1b5c4-142">planId</span><span class="sxs-lookup"><span data-stu-id="1b5c4-142">planId</span></span>|<span data-ttu-id="1b5c4-143">Строка</span><span class="sxs-lookup"><span data-stu-id="1b5c4-143">String</span></span>|<span data-ttu-id="1b5c4-144">Идентификатор плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-144">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="1b5c4-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b5c4-145">Response</span></span>

<span data-ttu-id="1b5c4-146">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-146">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="1b5c4-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="1b5c4-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="1b5c4-150">Пример</span><span class="sxs-lookup"><span data-stu-id="1b5c4-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b5c4-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b5c4-151">Request</span></span>
<span data-ttu-id="1b5c4-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b5c4-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="1b5c4-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b5c4-153">Response</span></span>
<span data-ttu-id="1b5c4-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1b5c4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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