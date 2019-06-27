---
title: Обновление объекта chartgridlines
description: Обновление свойств объекта chartgridlines.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cc2d9f7378151e1079584cae2ea8c1a6106e86c6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261721"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="5feba-103">Обновление объекта chartgridlines</span><span class="sxs-lookup"><span data-stu-id="5feba-103">Update chartgridlines</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5feba-104">Обновление свойств объекта chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="5feba-104">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5feba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5feba-105">Permissions</span></span>
<span data-ttu-id="5feba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5feba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5feba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5feba-108">Permission type</span></span>      | <span data-ttu-id="5feba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5feba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5feba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5feba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5feba-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5feba-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5feba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5feba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5feba-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5feba-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5feba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5feba-114">Application</span></span> | <span data-ttu-id="5feba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5feba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5feba-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5feba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/majorgridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines
```
## <a name="optional-request-headers"></a><span data-ttu-id="5feba-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5feba-117">Optional request headers</span></span>
| <span data-ttu-id="5feba-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5feba-118">Name</span></span>       | <span data-ttu-id="5feba-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5feba-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5feba-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5feba-120">Authorization</span></span>  | <span data-ttu-id="5feba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5feba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5feba-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5feba-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5feba-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5feba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5feba-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5feba-126">Request body</span></span>
<span data-ttu-id="5feba-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5feba-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5feba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5feba-130">Property</span></span>     | <span data-ttu-id="5feba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5feba-131">Type</span></span>   |<span data-ttu-id="5feba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5feba-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5feba-133">visible</span><span class="sxs-lookup"><span data-stu-id="5feba-133">visible</span></span>|<span data-ttu-id="5feba-134">boolean</span><span class="sxs-lookup"><span data-stu-id="5feba-134">boolean</span></span>|<span data-ttu-id="5feba-135">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="5feba-135">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="5feba-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5feba-136">Response</span></span>

<span data-ttu-id="5feba-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартгридлинес](../resources/workbookchartgridlines.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5feba-137">If successful, this method returns a `200 OK` response code and updated [workbookChartGridlines](../resources/workbookchartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5feba-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5feba-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5feba-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5feba-139">Request</span></span>
<span data-ttu-id="5feba-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5feba-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="5feba-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5feba-141">Response</span></span>
<span data-ttu-id="5feba-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5feba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5feba-145">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5feba-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5feba-146">C#</span><span class="sxs-lookup"><span data-stu-id="5feba-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartgridlines-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5feba-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="5feba-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartgridlines-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5feba-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5feba-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_chartgridlines-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartgridlines-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chartgridlines-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartgridlines-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
