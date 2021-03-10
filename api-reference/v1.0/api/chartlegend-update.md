---
title: Обновление объекта chartlegend
description: Обновление свойств объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2afb32bfabdcf703e5c85867946ec196a290e0cd
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578026"
---
# <a name="update-chartlegend"></a><span data-ttu-id="f494a-103">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="f494a-103">Update chartlegend</span></span>

<span data-ttu-id="f494a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f494a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f494a-105">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="f494a-105">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f494a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f494a-106">Permissions</span></span>
<span data-ttu-id="f494a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f494a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f494a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f494a-109">Permission type</span></span>      | <span data-ttu-id="f494a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f494a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f494a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f494a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f494a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f494a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f494a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f494a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f494a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f494a-114">Not supported.</span></span>    |
|<span data-ttu-id="f494a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f494a-115">Application</span></span> | <span data-ttu-id="f494a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f494a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f494a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f494a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="f494a-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f494a-118">Optional request headers</span></span>
| <span data-ttu-id="f494a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f494a-119">Name</span></span>       | <span data-ttu-id="f494a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f494a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f494a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f494a-121">Authorization</span></span>  | <span data-ttu-id="f494a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f494a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f494a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f494a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f494a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f494a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f494a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f494a-127">Request body</span></span>
<span data-ttu-id="f494a-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f494a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f494a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f494a-131">Property</span></span>     | <span data-ttu-id="f494a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f494a-132">Type</span></span>   |<span data-ttu-id="f494a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f494a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f494a-134">overlay</span><span class="sxs-lookup"><span data-stu-id="f494a-134">overlay</span></span>|<span data-ttu-id="f494a-135">boolean</span><span class="sxs-lookup"><span data-stu-id="f494a-135">boolean</span></span>|<span data-ttu-id="f494a-136">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f494a-136">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="f494a-137">position</span><span class="sxs-lookup"><span data-stu-id="f494a-137">position</span></span>|<span data-ttu-id="f494a-138">string</span><span class="sxs-lookup"><span data-stu-id="f494a-138">string</span></span>|<span data-ttu-id="f494a-139">Представляет расположение легенды на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="f494a-139">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="f494a-140">Допустимые значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="f494a-140">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="f494a-141">visible</span><span class="sxs-lookup"><span data-stu-id="f494a-141">visible</span></span>|<span data-ttu-id="f494a-142">boolean</span><span class="sxs-lookup"><span data-stu-id="f494a-142">boolean</span></span>|<span data-ttu-id="f494a-143">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="f494a-143">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="f494a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f494a-144">Response</span></span>

<span data-ttu-id="f494a-145">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookChartLegend](../resources/chartlegend.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f494a-145">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f494a-146">Пример</span><span class="sxs-lookup"><span data-stu-id="f494a-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f494a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="f494a-147">Request</span></span>
<span data-ttu-id="f494a-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f494a-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f494a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="f494a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
# <a name="c"></a>[<span data-ttu-id="f494a-150">C#</span><span class="sxs-lookup"><span data-stu-id="f494a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f494a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f494a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f494a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f494a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f494a-153">Java</span><span class="sxs-lookup"><span data-stu-id="f494a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f494a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f494a-154">Response</span></span>
<span data-ttu-id="f494a-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f494a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

