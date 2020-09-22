---
title: 'Range: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 27dfc289bc6272af36a92da3901208f0d3e6fcfa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004512"
---
# <a name="range-cell"></a><span data-ttu-id="4f8ef-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="4f8ef-105">Range: Cell</span></span>

<span data-ttu-id="4f8ef-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f8ef-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f8ef-p102">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f8ef-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f8ef-110">Permissions</span></span>
<span data-ttu-id="4f8ef-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f8ef-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f8ef-113">Permission type</span></span>      | <span data-ttu-id="4f8ef-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f8ef-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f8ef-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f8ef-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4f8ef-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f8ef-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f8ef-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f8ef-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f8ef-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f8ef-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f8ef-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f8ef-119">Application</span></span> | <span data-ttu-id="4f8ef-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f8ef-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f8ef-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="4f8ef-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f8ef-122">Request headers</span></span>
| <span data-ttu-id="4f8ef-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4f8ef-123">Name</span></span>       | <span data-ttu-id="4f8ef-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4f8ef-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f8ef-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f8ef-125">Authorization</span></span>  | <span data-ttu-id="4f8ef-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f8ef-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4f8ef-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f8ef-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f8ef-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f8ef-131">Request body</span></span>
<span data-ttu-id="4f8ef-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f8ef-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="4f8ef-133">Parameter</span></span>    | <span data-ttu-id="4f8ef-134">Тип</span><span class="sxs-lookup"><span data-stu-id="4f8ef-134">Type</span></span>   |<span data-ttu-id="4f8ef-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4f8ef-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f8ef-136">row</span><span class="sxs-lookup"><span data-stu-id="4f8ef-136">row</span></span>|<span data-ttu-id="4f8ef-137">number</span><span class="sxs-lookup"><span data-stu-id="4f8ef-137">number</span></span>|<span data-ttu-id="4f8ef-p106">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="4f8ef-140">column</span><span class="sxs-lookup"><span data-stu-id="4f8ef-140">column</span></span>|<span data-ttu-id="4f8ef-141">number</span><span class="sxs-lookup"><span data-stu-id="4f8ef-141">number</span></span>|<span data-ttu-id="4f8ef-p107">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="4f8ef-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f8ef-144">Response</span></span>

<span data-ttu-id="4f8ef-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f8ef-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4f8ef-146">Example</span></span>
<span data-ttu-id="4f8ef-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4f8ef-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f8ef-148">Request</span></span>
<span data-ttu-id="4f8ef-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4f8ef-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f8ef-150">Response</span></span>
<span data-ttu-id="4f8ef-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


