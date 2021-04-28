---
title: Обновление объекта chartlegend
description: Обновление свойств объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 86e5bb36845d5309a445e76e9843660f3cd6b8fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035766"
---
# <a name="update-chartlegend"></a><span data-ttu-id="e0b9c-103">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="e0b9c-103">Update chartlegend</span></span>

<span data-ttu-id="e0b9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0b9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0b9c-105">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-105">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0b9c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0b9c-106">Permissions</span></span>
<span data-ttu-id="e0b9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0b9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0b9c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0b9c-109">Permission type</span></span>      | <span data-ttu-id="e0b9c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0b9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0b9c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0b9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0b9c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0b9c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0b9c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0b9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0b9c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-114">Not supported.</span></span>    |
|<span data-ttu-id="e0b9c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0b9c-115">Application</span></span> | <span data-ttu-id="e0b9c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0b9c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0b9c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="e0b9c-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0b9c-118">Optional request headers</span></span>
| <span data-ttu-id="e0b9c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e0b9c-119">Name</span></span>       | <span data-ttu-id="e0b9c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e0b9c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e0b9c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0b9c-121">Authorization</span></span>  | <span data-ttu-id="e0b9c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0b9c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0b9c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0b9c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0b9c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0b9c-127">Request body</span></span>
<span data-ttu-id="e0b9c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e0b9c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0b9c-131">Property</span></span>     | <span data-ttu-id="e0b9c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e0b9c-132">Type</span></span>   |<span data-ttu-id="e0b9c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e0b9c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0b9c-134">overlay</span><span class="sxs-lookup"><span data-stu-id="e0b9c-134">overlay</span></span>|<span data-ttu-id="e0b9c-135">boolean</span><span class="sxs-lookup"><span data-stu-id="e0b9c-135">boolean</span></span>|<span data-ttu-id="e0b9c-136">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-136">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="e0b9c-137">position</span><span class="sxs-lookup"><span data-stu-id="e0b9c-137">position</span></span>|<span data-ttu-id="e0b9c-138">string</span><span class="sxs-lookup"><span data-stu-id="e0b9c-138">string</span></span>|<span data-ttu-id="e0b9c-139">Представляет расположение легенды на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-139">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="e0b9c-140">Допустимые значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-140">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="e0b9c-141">visible</span><span class="sxs-lookup"><span data-stu-id="e0b9c-141">visible</span></span>|<span data-ttu-id="e0b9c-142">boolean</span><span class="sxs-lookup"><span data-stu-id="e0b9c-142">boolean</span></span>|<span data-ttu-id="e0b9c-143">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-143">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="e0b9c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0b9c-144">Response</span></span>

<span data-ttu-id="e0b9c-145">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookChartLegend](../resources/chartlegend.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-145">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0b9c-146">Пример</span><span class="sxs-lookup"><span data-stu-id="e0b9c-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0b9c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0b9c-147">Request</span></span>
<span data-ttu-id="e0b9c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0b9c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0b9c-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e0b9c-150">C#</span><span class="sxs-lookup"><span data-stu-id="e0b9c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0b9c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0b9c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0b9c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0b9c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0b9c-153">Java</span><span class="sxs-lookup"><span data-stu-id="e0b9c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0b9c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0b9c-154">Response</span></span>
<span data-ttu-id="e0b9c-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-155">Here is an example of the response.</span></span> <span data-ttu-id="e0b9c-156">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e0b9c-156">Note: The response object shown here might be shortened for readability.</span></span>
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

