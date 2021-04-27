---
title: 'Range: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 85d66ee7385b178fa23806ce91c45b740ef88faa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055143"
---
# <a name="range-cell"></a><span data-ttu-id="16517-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="16517-105">Range: Cell</span></span>

<span data-ttu-id="16517-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16517-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16517-p102">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="16517-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="16517-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16517-110">Permissions</span></span>
<span data-ttu-id="16517-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16517-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16517-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16517-113">Permission type</span></span>      | <span data-ttu-id="16517-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16517-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16517-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16517-115">Delegated (work or school account)</span></span> | <span data-ttu-id="16517-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16517-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16517-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16517-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16517-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16517-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16517-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16517-119">Application</span></span> | <span data-ttu-id="16517-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16517-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16517-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16517-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/Cell
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/Cell
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/Cell
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="16517-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16517-122">Request headers</span></span>
| <span data-ttu-id="16517-123">Имя</span><span class="sxs-lookup"><span data-stu-id="16517-123">Name</span></span>       | <span data-ttu-id="16517-124">Описание</span><span class="sxs-lookup"><span data-stu-id="16517-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16517-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16517-125">Authorization</span></span>  | <span data-ttu-id="16517-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16517-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16517-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="16517-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="16517-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="16517-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16517-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16517-131">Request body</span></span>
<span data-ttu-id="16517-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="16517-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16517-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="16517-133">Parameter</span></span>    | <span data-ttu-id="16517-134">Тип</span><span class="sxs-lookup"><span data-stu-id="16517-134">Type</span></span>   |<span data-ttu-id="16517-135">Описание</span><span class="sxs-lookup"><span data-stu-id="16517-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16517-136">row</span><span class="sxs-lookup"><span data-stu-id="16517-136">row</span></span>|<span data-ttu-id="16517-137">number</span><span class="sxs-lookup"><span data-stu-id="16517-137">number</span></span>|<span data-ttu-id="16517-p106">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="16517-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="16517-140">column</span><span class="sxs-lookup"><span data-stu-id="16517-140">column</span></span>|<span data-ttu-id="16517-141">number</span><span class="sxs-lookup"><span data-stu-id="16517-141">number</span></span>|<span data-ttu-id="16517-p107">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="16517-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="16517-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="16517-144">Response</span></span>

<span data-ttu-id="16517-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16517-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16517-146">Пример</span><span class="sxs-lookup"><span data-stu-id="16517-146">Example</span></span>
<span data-ttu-id="16517-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="16517-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="16517-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="16517-148">Request</span></span>
<span data-ttu-id="16517-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16517-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="16517-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="16517-150">Response</span></span>
<span data-ttu-id="16517-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16517-151">Here is an example of the response.</span></span> <span data-ttu-id="16517-152">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="16517-152">Note: The response object shown here might be shortened for readability.</span></span>
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


