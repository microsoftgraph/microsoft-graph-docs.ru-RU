---
title: 'Range: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ef9888c934a0d85f66c49e062074c2c328cafa13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915657"
---
# <a name="range-cell"></a><span data-ttu-id="efcef-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="efcef-105">Range: Cell</span></span>

> <span data-ttu-id="efcef-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="efcef-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efcef-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efcef-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="efcef-p103">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="efcef-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="efcef-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efcef-111">Permissions</span></span>
<span data-ttu-id="efcef-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efcef-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efcef-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efcef-114">Permission type</span></span>      | <span data-ttu-id="efcef-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efcef-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efcef-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efcef-116">Delegated (work or school account)</span></span> | <span data-ttu-id="efcef-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efcef-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="efcef-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efcef-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efcef-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efcef-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="efcef-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efcef-120">Application</span></span> | <span data-ttu-id="efcef-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efcef-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="efcef-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efcef-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="efcef-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efcef-123">Request headers</span></span>
| <span data-ttu-id="efcef-124">Имя</span><span class="sxs-lookup"><span data-stu-id="efcef-124">Name</span></span>       | <span data-ttu-id="efcef-125">Описание</span><span class="sxs-lookup"><span data-stu-id="efcef-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="efcef-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efcef-126">Authorization</span></span>  | <span data-ttu-id="efcef-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efcef-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="efcef-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="efcef-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="efcef-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="efcef-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="efcef-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="efcef-132">Request body</span></span>
<span data-ttu-id="efcef-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="efcef-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="efcef-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="efcef-134">Parameter</span></span>    | <span data-ttu-id="efcef-135">Тип</span><span class="sxs-lookup"><span data-stu-id="efcef-135">Type</span></span>   |<span data-ttu-id="efcef-136">Описание</span><span class="sxs-lookup"><span data-stu-id="efcef-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efcef-137">row</span><span class="sxs-lookup"><span data-stu-id="efcef-137">row</span></span>|<span data-ttu-id="efcef-138">number</span><span class="sxs-lookup"><span data-stu-id="efcef-138">number</span></span>|<span data-ttu-id="efcef-p107">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="efcef-p107">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="efcef-141">column</span><span class="sxs-lookup"><span data-stu-id="efcef-141">column</span></span>|<span data-ttu-id="efcef-142">number</span><span class="sxs-lookup"><span data-stu-id="efcef-142">number</span></span>|<span data-ttu-id="efcef-p108">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="efcef-p108">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="efcef-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="efcef-145">Response</span></span>

<span data-ttu-id="efcef-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="efcef-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efcef-147">Пример</span><span class="sxs-lookup"><span data-stu-id="efcef-147">Example</span></span>
<span data-ttu-id="efcef-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="efcef-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="efcef-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="efcef-149">Request</span></span>
<span data-ttu-id="efcef-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efcef-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="efcef-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="efcef-151">Response</span></span>
<span data-ttu-id="efcef-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="efcef-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "tocPath": ""
}-->
