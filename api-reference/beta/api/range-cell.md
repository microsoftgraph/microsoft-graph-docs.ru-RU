---
title: 'Range: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9dffd75ed5e70e373f824d11fdcc287ce09f051a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991949"
---
# <a name="range-cell"></a><span data-ttu-id="0151c-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="0151c-105">Range: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0151c-p102">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="0151c-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="0151c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0151c-109">Permissions</span></span>
<span data-ttu-id="0151c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0151c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0151c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0151c-112">Permission type</span></span>      | <span data-ttu-id="0151c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0151c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0151c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0151c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0151c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0151c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0151c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0151c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0151c-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0151c-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0151c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0151c-118">Application</span></span> | <span data-ttu-id="0151c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0151c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0151c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0151c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="0151c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0151c-121">Request headers</span></span>
| <span data-ttu-id="0151c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0151c-122">Name</span></span>       | <span data-ttu-id="0151c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0151c-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0151c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0151c-124">Authorization</span></span>  | <span data-ttu-id="0151c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0151c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0151c-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0151c-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="0151c-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0151c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0151c-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0151c-130">Request body</span></span>
<span data-ttu-id="0151c-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0151c-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0151c-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="0151c-132">Parameter</span></span>    | <span data-ttu-id="0151c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0151c-133">Type</span></span>   |<span data-ttu-id="0151c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0151c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0151c-135">row</span><span class="sxs-lookup"><span data-stu-id="0151c-135">row</span></span>|<span data-ttu-id="0151c-136">число</span><span class="sxs-lookup"><span data-stu-id="0151c-136">number</span></span>|<span data-ttu-id="0151c-p106">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="0151c-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="0151c-139">column</span><span class="sxs-lookup"><span data-stu-id="0151c-139">column</span></span>|<span data-ttu-id="0151c-140">number</span><span class="sxs-lookup"><span data-stu-id="0151c-140">number</span></span>|<span data-ttu-id="0151c-p107">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="0151c-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="0151c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0151c-143">Response</span></span>

<span data-ttu-id="0151c-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0151c-144">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0151c-145">Пример</span><span class="sxs-lookup"><span data-stu-id="0151c-145">Example</span></span>
<span data-ttu-id="0151c-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0151c-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0151c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0151c-147">Request</span></span>
<span data-ttu-id="0151c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0151c-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="0151c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0151c-149">Response</span></span>
<span data-ttu-id="0151c-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0151c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
