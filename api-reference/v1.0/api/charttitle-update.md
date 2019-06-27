---
title: Обновление объекта ChartTitle
description: Обновление свойств объекта charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9480e46672d6ecd021429a4b4187d0e204e62006
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277534"
---
# <a name="update-charttitle"></a><span data-ttu-id="72834-103">Обновление объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="72834-103">Update charttitle</span></span>

<span data-ttu-id="72834-104">Обновление свойств объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="72834-104">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="72834-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72834-105">Permissions</span></span>
<span data-ttu-id="72834-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72834-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72834-108">Permission type</span></span>      | <span data-ttu-id="72834-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72834-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72834-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72834-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72834-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72834-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="72834-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72834-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72834-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72834-113">Not supported.</span></span>    |
|<span data-ttu-id="72834-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72834-114">Application</span></span> | <span data-ttu-id="72834-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72834-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72834-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72834-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="72834-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72834-117">Optional request headers</span></span>
| <span data-ttu-id="72834-118">Имя</span><span class="sxs-lookup"><span data-stu-id="72834-118">Name</span></span>       | <span data-ttu-id="72834-119">Описание</span><span class="sxs-lookup"><span data-stu-id="72834-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="72834-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72834-120">Authorization</span></span>  | <span data-ttu-id="72834-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72834-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72834-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="72834-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="72834-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="72834-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72834-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72834-126">Request body</span></span>
<span data-ttu-id="72834-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="72834-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="72834-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72834-130">Property</span></span>     | <span data-ttu-id="72834-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72834-131">Type</span></span>   |<span data-ttu-id="72834-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72834-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72834-133">overlay</span><span class="sxs-lookup"><span data-stu-id="72834-133">overlay</span></span>|<span data-ttu-id="72834-134">boolean</span><span class="sxs-lookup"><span data-stu-id="72834-134">boolean</span></span>|<span data-ttu-id="72834-135">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="72834-135">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="72834-136">text</span><span class="sxs-lookup"><span data-stu-id="72834-136">text</span></span>|<span data-ttu-id="72834-137">string</span><span class="sxs-lookup"><span data-stu-id="72834-137">string</span></span>|<span data-ttu-id="72834-138">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="72834-138">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="72834-139">visible</span><span class="sxs-lookup"><span data-stu-id="72834-139">visible</span></span>|<span data-ttu-id="72834-140">boolean</span><span class="sxs-lookup"><span data-stu-id="72834-140">boolean</span></span>|<span data-ttu-id="72834-141">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="72834-141">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="72834-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="72834-142">Response</span></span>

<span data-ttu-id="72834-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчарттитле](../resources/charttitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72834-143">If successful, this method returns a `200 OK` response code and updated [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="72834-144">Пример</span><span class="sxs-lookup"><span data-stu-id="72834-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72834-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="72834-145">Request</span></span>
<span data-ttu-id="72834-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72834-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="72834-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="72834-147">Response</span></span>
<span data-ttu-id="72834-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72834-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="72834-151">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="72834-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="72834-152">C#</span><span class="sxs-lookup"><span data-stu-id="72834-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_charttitle-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72834-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="72834-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_charttitle-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="72834-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="72834-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_charttitle-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/charttitle-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/charttitle-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/charttitle-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
