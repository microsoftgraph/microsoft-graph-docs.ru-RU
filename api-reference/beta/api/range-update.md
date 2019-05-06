---
title: Обновление диапазона
description: Обновление свойств объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 49587a52de74503f7bac974a5bc52c7cabea7716
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610519"
---
# <a name="update-range"></a><span data-ttu-id="710a8-103">Обновление диапазона</span><span class="sxs-lookup"><span data-stu-id="710a8-103">Update range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="710a8-104">Обновление свойств объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="710a8-104">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="710a8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="710a8-105">Permissions</span></span>
<span data-ttu-id="710a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="710a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="710a8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="710a8-108">Permission type</span></span>      | <span data-ttu-id="710a8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="710a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="710a8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="710a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="710a8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="710a8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="710a8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="710a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="710a8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="710a8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="710a8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="710a8-114">Application</span></span> | <span data-ttu-id="710a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="710a8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="710a8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="710a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="710a8-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="710a8-117">Optional request headers</span></span>
| <span data-ttu-id="710a8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="710a8-118">Name</span></span>       | <span data-ttu-id="710a8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="710a8-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="710a8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="710a8-120">Authorization</span></span>  | <span data-ttu-id="710a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="710a8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="710a8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="710a8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="710a8-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="710a8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="710a8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="710a8-126">Request body</span></span>
<span data-ttu-id="710a8-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="710a8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="710a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="710a8-130">Property</span></span>     | <span data-ttu-id="710a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="710a8-131">Type</span></span>   |<span data-ttu-id="710a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="710a8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="710a8-133">columnHidden</span><span class="sxs-lookup"><span data-stu-id="710a8-133">columnHidden</span></span>|<span data-ttu-id="710a8-134">boolean</span><span class="sxs-lookup"><span data-stu-id="710a8-134">boolean</span></span>|<span data-ttu-id="710a8-135">Указывает, скрыты ли все столбцы текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="710a8-135">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="710a8-136">formulas</span><span class="sxs-lookup"><span data-stu-id="710a8-136">formulas</span></span>|<span data-ttu-id="710a8-137">Json</span><span class="sxs-lookup"><span data-stu-id="710a8-137">Json</span></span>|<span data-ttu-id="710a8-138">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="710a8-138">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="710a8-139">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="710a8-139">formulasLocal</span></span>|<span data-ttu-id="710a8-140">Json</span><span class="sxs-lookup"><span data-stu-id="710a8-140">Json</span></span>|<span data-ttu-id="710a8-p105">Представляет формулу в нотации стиля A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула =SUM(A1, 1.5) превратится в "=СУММ(A1; 1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="710a8-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="710a8-143">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="710a8-143">formulasR1C1</span></span>|<span data-ttu-id="710a8-144">Json</span><span class="sxs-lookup"><span data-stu-id="710a8-144">Json</span></span>|<span data-ttu-id="710a8-145">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="710a8-145">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="710a8-146">numberFormat</span><span class="sxs-lookup"><span data-stu-id="710a8-146">numberFormat</span></span>|<span data-ttu-id="710a8-147">Json</span><span class="sxs-lookup"><span data-stu-id="710a8-147">Json</span></span>|<span data-ttu-id="710a8-148">Представляет код в числовом формате Excel для данной ячейки.</span><span class="sxs-lookup"><span data-stu-id="710a8-148">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="710a8-149">rowHidden</span><span class="sxs-lookup"><span data-stu-id="710a8-149">rowHidden</span></span>|<span data-ttu-id="710a8-150">boolean</span><span class="sxs-lookup"><span data-stu-id="710a8-150">boolean</span></span>|<span data-ttu-id="710a8-151">Указывает, скрыты ли все строки текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="710a8-151">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="710a8-152">values</span><span class="sxs-lookup"><span data-stu-id="710a8-152">values</span></span>|<span data-ttu-id="710a8-153">Json</span><span class="sxs-lookup"><span data-stu-id="710a8-153">Json</span></span>|<span data-ttu-id="710a8-p106">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="710a8-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="710a8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="710a8-157">Response</span></span>

<span data-ttu-id="710a8-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [workbookRange](../resources/workbookrange.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="710a8-158">If successful, this method returns a `200 OK` response code and updated [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="710a8-159">Пример</span><span class="sxs-lookup"><span data-stu-id="710a8-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="710a8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="710a8-160">Request</span></span>
<span data-ttu-id="710a8-p107">Ниже приведен пример запроса. Он обновляет диапазон — значения числовой формат и формулу. Значение `null` сообщает API, что в данном случае нужно пропустить ячейку. Значения, числовые форматы и формулы можно обновлять по отдельности или в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="710a8-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/sheet1/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formulas" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="710a8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="710a8-165">Response</span></span>
<span data-ttu-id="710a8-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="710a8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="710a8-169">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="710a8-169">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="710a8-170">Язык</span><span class="sxs-lookup"><span data-stu-id="710a8-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_range-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
