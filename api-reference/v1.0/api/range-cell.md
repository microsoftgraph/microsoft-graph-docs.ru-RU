---
title: 'Range: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c326dbbb5885786008d4bac0730a37b4dd92941d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025395"
---
# <a name="range-cell"></a><span data-ttu-id="a22a4-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="a22a4-105">Range: Cell</span></span>

<span data-ttu-id="a22a4-p102">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="a22a4-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="a22a4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a22a4-109">Permissions</span></span>
<span data-ttu-id="a22a4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a22a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a22a4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a22a4-112">Permission type</span></span>      | <span data-ttu-id="a22a4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a22a4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a22a4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a22a4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a22a4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a22a4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a22a4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a22a4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a22a4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a22a4-117">Not supported.</span></span>    |
|<span data-ttu-id="a22a4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a22a4-118">Application</span></span> | <span data-ttu-id="a22a4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a22a4-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a22a4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a22a4-120">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a22a4-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="a22a4-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="a22a4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a22a4-122">Request headers</span></span>
| <span data-ttu-id="a22a4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a22a4-123">Name</span></span>       | <span data-ttu-id="a22a4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a22a4-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a22a4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a22a4-125">Authorization</span></span>  | <span data-ttu-id="a22a4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a22a4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a22a4-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a22a4-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="a22a4-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a22a4-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="a22a4-131">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="a22a4-131">Path parameters</span></span>
<span data-ttu-id="a22a4-132">В поле путь укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="a22a4-132">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="a22a4-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="a22a4-133">Parameter</span></span>    | <span data-ttu-id="a22a4-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a22a4-134">Type</span></span>   |<span data-ttu-id="a22a4-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a22a4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a22a4-136">row</span><span class="sxs-lookup"><span data-stu-id="a22a4-136">row</span></span>|<span data-ttu-id="a22a4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a22a4-137">Int32</span></span>|<span data-ttu-id="a22a4-p106">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="a22a4-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="a22a4-140">column</span><span class="sxs-lookup"><span data-stu-id="a22a4-140">column</span></span>|<span data-ttu-id="a22a4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a22a4-141">Int32</span></span>|<span data-ttu-id="a22a4-p107">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="a22a4-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="a22a4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a22a4-144">Response</span></span>

<span data-ttu-id="a22a4-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a22a4-145">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a22a4-146">Пример</span><span class="sxs-lookup"><span data-stu-id="a22a4-146">Example</span></span>
<span data-ttu-id="a22a4-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a22a4-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a22a4-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a22a4-148">Request</span></span>
<span data-ttu-id="a22a4-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a22a4-149">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a22a4-150">C#</span><span class="sxs-lookup"><span data-stu-id="a22a4-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-cell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a22a4-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="a22a4-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-cell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a22a4-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a22a4-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-cell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a22a4-153">Java</span><span class="sxs-lookup"><span data-stu-id="a22a4-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-cell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a22a4-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="a22a4-154">Response</span></span>
<span data-ttu-id="a22a4-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a22a4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
