---
title: Обновление объекта chartlegend
description: Обновление свойств объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0fa24737053c821ed636a898b56b2ed8879bf25c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518422"
---
# <a name="update-chartlegend"></a><span data-ttu-id="42350-103">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="42350-103">Update chartlegend</span></span>

<span data-ttu-id="42350-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42350-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42350-105">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="42350-105">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="42350-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42350-106">Permissions</span></span>
<span data-ttu-id="42350-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42350-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42350-109">Permission type</span></span>      | <span data-ttu-id="42350-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42350-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42350-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42350-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42350-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42350-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42350-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42350-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42350-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42350-114">Not supported.</span></span>    |
|<span data-ttu-id="42350-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42350-115">Application</span></span> | <span data-ttu-id="42350-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42350-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42350-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42350-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="42350-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42350-118">Optional request headers</span></span>
| <span data-ttu-id="42350-119">Имя</span><span class="sxs-lookup"><span data-stu-id="42350-119">Name</span></span>       | <span data-ttu-id="42350-120">Описание</span><span class="sxs-lookup"><span data-stu-id="42350-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="42350-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42350-121">Authorization</span></span>  | <span data-ttu-id="42350-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42350-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42350-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="42350-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="42350-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="42350-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42350-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42350-127">Request body</span></span>
<span data-ttu-id="42350-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="42350-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="42350-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="42350-131">Property</span></span>     | <span data-ttu-id="42350-132">Тип</span><span class="sxs-lookup"><span data-stu-id="42350-132">Type</span></span>   |<span data-ttu-id="42350-133">Описание</span><span class="sxs-lookup"><span data-stu-id="42350-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42350-134">overlay</span><span class="sxs-lookup"><span data-stu-id="42350-134">overlay</span></span>|<span data-ttu-id="42350-135">boolean</span><span class="sxs-lookup"><span data-stu-id="42350-135">boolean</span></span>|<span data-ttu-id="42350-136">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="42350-136">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="42350-137">position</span><span class="sxs-lookup"><span data-stu-id="42350-137">position</span></span>|<span data-ttu-id="42350-138">string</span><span class="sxs-lookup"><span data-stu-id="42350-138">string</span></span>|<span data-ttu-id="42350-139">Представляет расположение легенды на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="42350-139">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="42350-140">Допустимые значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="42350-140">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="42350-141">visible</span><span class="sxs-lookup"><span data-stu-id="42350-141">visible</span></span>|<span data-ttu-id="42350-142">boolean</span><span class="sxs-lookup"><span data-stu-id="42350-142">boolean</span></span>|<span data-ttu-id="42350-143">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="42350-143">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="42350-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="42350-144">Response</span></span>

<span data-ttu-id="42350-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартлеженд](../resources/chartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42350-145">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42350-146">Пример</span><span class="sxs-lookup"><span data-stu-id="42350-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42350-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="42350-147">Request</span></span>
<span data-ttu-id="42350-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42350-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42350-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="42350-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="42350-150">C#</span><span class="sxs-lookup"><span data-stu-id="42350-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42350-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42350-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42350-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42350-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42350-153">Java</span><span class="sxs-lookup"><span data-stu-id="42350-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42350-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="42350-154">Response</span></span>
<span data-ttu-id="42350-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42350-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
