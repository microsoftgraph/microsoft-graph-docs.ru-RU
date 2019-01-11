---
title: Обновление объекта plannerbucket
description: Обновление свойств объекта **plannerbucket**.
localization_priority: Normal
ms.openlocfilehash: 84583df95d69f4b7f4beb604cd3cf61270c177ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814940"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="ff5b5-103">Обновление объекта plannerbucket</span><span class="sxs-lookup"><span data-stu-id="ff5b5-103">Update plannerbucket</span></span>

<span data-ttu-id="ff5b5-104">Обновление свойств объекта **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-104">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff5b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff5b5-105">Permissions</span></span>
<span data-ttu-id="ff5b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff5b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff5b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff5b5-108">Permission type</span></span>      | <span data-ttu-id="ff5b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff5b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff5b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff5b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff5b5-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5b5-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff5b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff5b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff5b5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-113">Not supported.</span></span>    |
|<span data-ttu-id="ff5b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff5b5-114">Application</span></span> | <span data-ttu-id="ff5b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff5b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff5b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ff5b5-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff5b5-117">Optional request headers</span></span>
| <span data-ttu-id="ff5b5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ff5b5-118">Name</span></span>       | <span data-ttu-id="ff5b5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ff5b5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ff5b5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff5b5-120">Authorization</span></span>  | <span data-ttu-id="ff5b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff5b5-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="ff5b5-123">If-Match</span></span>  | <span data-ttu-id="ff5b5-p103">Последнее известное значение ETag обновляемого объекта **plannerBucket**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff5b5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff5b5-126">Request body</span></span>
<span data-ttu-id="ff5b5-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff5b5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff5b5-130">Property</span></span>     | <span data-ttu-id="ff5b5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff5b5-131">Type</span></span>   |<span data-ttu-id="ff5b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff5b5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff5b5-133">name</span><span class="sxs-lookup"><span data-stu-id="ff5b5-133">name</span></span>|<span data-ttu-id="ff5b5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ff5b5-134">String</span></span>|<span data-ttu-id="ff5b5-135">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-135">Name of the bucket.</span></span>|
|<span data-ttu-id="ff5b5-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="ff5b5-136">orderHint</span></span>|<span data-ttu-id="ff5b5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ff5b5-137">String</span></span>|<span data-ttu-id="ff5b5-p105">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="ff5b5-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="ff5b5-140">planId</span><span class="sxs-lookup"><span data-stu-id="ff5b5-140">planId</span></span>|<span data-ttu-id="ff5b5-141">Строка</span><span class="sxs-lookup"><span data-stu-id="ff5b5-141">String</span></span>|<span data-ttu-id="ff5b5-142">Идентификатор плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-142">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="ff5b5-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff5b5-143">Response</span></span>

<span data-ttu-id="ff5b5-144">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-144">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="ff5b5-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ff5b5-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ff5b5-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ff5b5-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff5b5-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff5b5-149">Request</span></span>
<span data-ttu-id="ff5b5-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-150">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ff5b5-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff5b5-151">Response</span></span>
<span data-ttu-id="ff5b5-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ff5b5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
