---
title: Обновление объекта chartlegend
description: Обновление свойств объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6a7fdaca3da7840953aebb908de38f0bcd010675
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317111"
---
# <a name="update-chartlegend"></a><span data-ttu-id="74597-103">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="74597-103">Update chartlegend</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74597-104">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="74597-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="74597-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74597-105">Permissions</span></span>
<span data-ttu-id="74597-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74597-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74597-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74597-108">Permission type</span></span>      | <span data-ttu-id="74597-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74597-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74597-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74597-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74597-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74597-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74597-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74597-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74597-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74597-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74597-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74597-114">Application</span></span> | <span data-ttu-id="74597-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74597-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74597-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74597-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="74597-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74597-117">Optional request headers</span></span>
| <span data-ttu-id="74597-118">Имя</span><span class="sxs-lookup"><span data-stu-id="74597-118">Name</span></span>       | <span data-ttu-id="74597-119">Описание</span><span class="sxs-lookup"><span data-stu-id="74597-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="74597-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74597-120">Authorization</span></span>  | <span data-ttu-id="74597-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74597-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74597-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74597-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="74597-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="74597-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74597-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74597-126">Request body</span></span>
<span data-ttu-id="74597-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="74597-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="74597-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="74597-130">Property</span></span>     | <span data-ttu-id="74597-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74597-131">Type</span></span>   |<span data-ttu-id="74597-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74597-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74597-133">overlay</span><span class="sxs-lookup"><span data-stu-id="74597-133">overlay</span></span>|<span data-ttu-id="74597-134">boolean</span><span class="sxs-lookup"><span data-stu-id="74597-134">boolean</span></span>|<span data-ttu-id="74597-135">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="74597-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="74597-136">position</span><span class="sxs-lookup"><span data-stu-id="74597-136">position</span></span>|<span data-ttu-id="74597-137">string</span><span class="sxs-lookup"><span data-stu-id="74597-137">string</span></span>|<span data-ttu-id="74597-p105">Представляет расположение легенды на диаграмме. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="74597-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="74597-140">visible</span><span class="sxs-lookup"><span data-stu-id="74597-140">visible</span></span>|<span data-ttu-id="74597-141">boolean</span><span class="sxs-lookup"><span data-stu-id="74597-141">boolean</span></span>|<span data-ttu-id="74597-142">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="74597-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="74597-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="74597-143">Response</span></span>

<span data-ttu-id="74597-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартлеженд](../resources/workbookchartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74597-144">If successful, this method returns a `200 OK` response code and updated [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74597-145">Пример</span><span class="sxs-lookup"><span data-stu-id="74597-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74597-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="74597-146">Request</span></span>
<span data-ttu-id="74597-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74597-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74597-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="74597-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74597-149">C#</span><span class="sxs-lookup"><span data-stu-id="74597-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74597-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74597-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74597-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="74597-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="74597-152">Java</span><span class="sxs-lookup"><span data-stu-id="74597-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="74597-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="74597-153">Response</span></span>
<span data-ttu-id="74597-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74597-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
