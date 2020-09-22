---
title: Обновление диаграммы
description: Обновление свойств объекта диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8636c09c12b0c505dd4b71f104fa6e2b8711ddee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059966"
---
# <a name="update-chart"></a><span data-ttu-id="e6552-103">Обновление диаграммы</span><span class="sxs-lookup"><span data-stu-id="e6552-103">Update chart</span></span>

<span data-ttu-id="e6552-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6552-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6552-105">Обновление свойств объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e6552-105">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6552-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6552-106">Permissions</span></span>
<span data-ttu-id="e6552-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6552-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6552-109">Permission type</span></span>      | <span data-ttu-id="e6552-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6552-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6552-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6552-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e6552-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6552-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6552-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6552-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6552-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6552-114">Not supported.</span></span>    |
|<span data-ttu-id="e6552-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6552-115">Application</span></span> | <span data-ttu-id="e6552-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6552-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6552-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6552-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e6552-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6552-118">Optional request headers</span></span>
| <span data-ttu-id="e6552-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e6552-119">Name</span></span>       | <span data-ttu-id="e6552-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e6552-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e6552-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6552-121">Authorization</span></span>  | <span data-ttu-id="e6552-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6552-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6552-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e6552-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e6552-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e6552-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6552-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6552-127">Request body</span></span>
<span data-ttu-id="e6552-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e6552-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e6552-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6552-131">Property</span></span>     | <span data-ttu-id="e6552-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e6552-132">Type</span></span>   |<span data-ttu-id="e6552-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e6552-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6552-134">height</span><span class="sxs-lookup"><span data-stu-id="e6552-134">height</span></span>|<span data-ttu-id="e6552-135">double</span><span class="sxs-lookup"><span data-stu-id="e6552-135">double</span></span>|<span data-ttu-id="e6552-136">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="e6552-136">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="e6552-137">left</span><span class="sxs-lookup"><span data-stu-id="e6552-137">left</span></span>|<span data-ttu-id="e6552-138">double</span><span class="sxs-lookup"><span data-stu-id="e6552-138">double</span></span>|<span data-ttu-id="e6552-139">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="e6552-139">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="e6552-140">name</span><span class="sxs-lookup"><span data-stu-id="e6552-140">name</span></span>|<span data-ttu-id="e6552-141">string</span><span class="sxs-lookup"><span data-stu-id="e6552-141">string</span></span>|<span data-ttu-id="e6552-142">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e6552-142">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="e6552-143">top</span><span class="sxs-lookup"><span data-stu-id="e6552-143">top</span></span>|<span data-ttu-id="e6552-144">double</span><span class="sxs-lookup"><span data-stu-id="e6552-144">double</span></span>|<span data-ttu-id="e6552-145">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="e6552-145">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="e6552-146">width</span><span class="sxs-lookup"><span data-stu-id="e6552-146">width</span></span>|<span data-ttu-id="e6552-147">double</span><span class="sxs-lookup"><span data-stu-id="e6552-147">double</span></span>|<span data-ttu-id="e6552-148">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="e6552-148">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="e6552-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6552-149">Response</span></span>

<span data-ttu-id="e6552-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчарт](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6552-150">If successful, this method returns a `200 OK` response code and updated [WorkbookChart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6552-151">Пример</span><span class="sxs-lookup"><span data-stu-id="e6552-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6552-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6552-152">Request</span></span>
<span data-ttu-id="e6552-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6552-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6552-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6552-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
# <a name="c"></a>[<span data-ttu-id="e6552-155">C#</span><span class="sxs-lookup"><span data-stu-id="e6552-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6552-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6552-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6552-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6552-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6552-158">Java</span><span class="sxs-lookup"><span data-stu-id="e6552-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e6552-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6552-159">Response</span></span>
<span data-ttu-id="e6552-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6552-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

