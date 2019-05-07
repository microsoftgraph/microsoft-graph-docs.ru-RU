---
title: Обновление диаграммы
description: Обновление свойств объекта диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d7219f073f02a5e587e1be15cd9d32def6a6eba5
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635619"
---
# <a name="update-chart"></a><span data-ttu-id="e4c17-103">Обновление диаграммы</span><span class="sxs-lookup"><span data-stu-id="e4c17-103">Update chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4c17-104">Обновление свойств объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e4c17-104">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4c17-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4c17-105">Permissions</span></span>
<span data-ttu-id="e4c17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4c17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4c17-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4c17-108">Permission type</span></span>      | <span data-ttu-id="e4c17-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4c17-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4c17-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4c17-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4c17-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4c17-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4c17-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4c17-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4c17-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4c17-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4c17-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4c17-114">Application</span></span> | <span data-ttu-id="e4c17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4c17-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4c17-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4c17-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e4c17-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4c17-117">Optional request headers</span></span>
| <span data-ttu-id="e4c17-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e4c17-118">Name</span></span>       | <span data-ttu-id="e4c17-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e4c17-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e4c17-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4c17-120">Authorization</span></span>  | <span data-ttu-id="e4c17-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4c17-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4c17-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e4c17-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4c17-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e4c17-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4c17-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4c17-126">Request body</span></span>
<span data-ttu-id="e4c17-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e4c17-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e4c17-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4c17-130">Property</span></span>     | <span data-ttu-id="e4c17-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4c17-131">Type</span></span>   |<span data-ttu-id="e4c17-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4c17-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4c17-133">height</span><span class="sxs-lookup"><span data-stu-id="e4c17-133">height</span></span>|<span data-ttu-id="e4c17-134">double</span><span class="sxs-lookup"><span data-stu-id="e4c17-134">double</span></span>|<span data-ttu-id="e4c17-135">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="e4c17-135">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="e4c17-136">left</span><span class="sxs-lookup"><span data-stu-id="e4c17-136">left</span></span>|<span data-ttu-id="e4c17-137">double</span><span class="sxs-lookup"><span data-stu-id="e4c17-137">double</span></span>|<span data-ttu-id="e4c17-138">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="e4c17-138">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="e4c17-139">name</span><span class="sxs-lookup"><span data-stu-id="e4c17-139">name</span></span>|<span data-ttu-id="e4c17-140">string</span><span class="sxs-lookup"><span data-stu-id="e4c17-140">string</span></span>|<span data-ttu-id="e4c17-141">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e4c17-141">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="e4c17-142">top</span><span class="sxs-lookup"><span data-stu-id="e4c17-142">top</span></span>|<span data-ttu-id="e4c17-143">double</span><span class="sxs-lookup"><span data-stu-id="e4c17-143">double</span></span>|<span data-ttu-id="e4c17-144">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="e4c17-144">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="e4c17-145">width</span><span class="sxs-lookup"><span data-stu-id="e4c17-145">width</span></span>|<span data-ttu-id="e4c17-146">double</span><span class="sxs-lookup"><span data-stu-id="e4c17-146">double</span></span>|<span data-ttu-id="e4c17-147">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="e4c17-147">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="e4c17-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4c17-148">Response</span></span>

<span data-ttu-id="e4c17-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчарт](../resources/workbookchart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4c17-149">If successful, this method returns a `200 OK` response code and updated [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4c17-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e4c17-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4c17-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4c17-151">Request</span></span>
<span data-ttu-id="e4c17-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4c17-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="e4c17-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4c17-153">Response</span></span>
<span data-ttu-id="e4c17-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4c17-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e4c17-157">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e4c17-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e4c17-158">Языках</span><span class="sxs-lookup"><span data-stu-id="e4c17-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4c17-159">Язык</span><span class="sxs-lookup"><span data-stu-id="e4c17-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chart-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chart-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
