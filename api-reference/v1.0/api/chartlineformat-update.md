---
title: Обновление объекта ChartLineFormat
description: Обновление свойств объекта chartlineformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e3da69e44fb8736543e46696099928cbe71cb62c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264710"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="a9b8a-103">Обновление объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a9b8a-103">Update chartlineformat</span></span>

<span data-ttu-id="a9b8a-104">Обновление свойств объекта chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-104">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9b8a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9b8a-105">Permissions</span></span>
<span data-ttu-id="a9b8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9b8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b8a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9b8a-108">Permission type</span></span>      | <span data-ttu-id="a9b8a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9b8a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9b8a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9b8a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9b8a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9b8a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a9b8a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9b8a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9b8a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-113">Not supported.</span></span>    |
|<span data-ttu-id="a9b8a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9b8a-114">Application</span></span> | <span data-ttu-id="a9b8a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9b8a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9b8a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="a9b8a-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9b8a-117">Optional request headers</span></span>
| <span data-ttu-id="a9b8a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a9b8a-118">Name</span></span>       | <span data-ttu-id="a9b8a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a9b8a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a9b8a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9b8a-120">Authorization</span></span>  | <span data-ttu-id="a9b8a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9b8a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a9b8a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a9b8a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9b8a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9b8a-126">Request body</span></span>
<span data-ttu-id="a9b8a-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a9b8a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9b8a-130">Property</span></span>     | <span data-ttu-id="a9b8a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9b8a-131">Type</span></span>   |<span data-ttu-id="a9b8a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9b8a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9b8a-133">color</span><span class="sxs-lookup"><span data-stu-id="a9b8a-133">color</span></span>|<span data-ttu-id="a9b8a-134">string</span><span class="sxs-lookup"><span data-stu-id="a9b8a-134">string</span></span>|<span data-ttu-id="a9b8a-135">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-135">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="a9b8a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9b8a-136">Response</span></span>

<span data-ttu-id="a9b8a-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартлинеформат](../resources/chartlineformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9b8a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a9b8a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9b8a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9b8a-139">Request</span></span>
<span data-ttu-id="a9b8a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="a9b8a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9b8a-141">Response</span></span>
<span data-ttu-id="a9b8a-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9b8a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a9b8a-145">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a9b8a-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a9b8a-146">C#</span><span class="sxs-lookup"><span data-stu-id="a9b8a-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartlineformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9b8a-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9b8a-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartlineformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a9b8a-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a9b8a-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_chartlineformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartlineformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartlineformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartlineformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
