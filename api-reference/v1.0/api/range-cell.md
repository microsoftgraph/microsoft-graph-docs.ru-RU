---
title: 'Range: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.
localization_priority: Normal
ms.openlocfilehash: 3d72f78b6767dffe52e42ae210c24b9d96cc87d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862981"
---
# <a name="range-cell"></a><span data-ttu-id="87e2f-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="87e2f-105">Range: Cell</span></span>

<span data-ttu-id="87e2f-p102">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="87e2f-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="87e2f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87e2f-109">Permissions</span></span>
<span data-ttu-id="87e2f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87e2f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87e2f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87e2f-112">Permission type</span></span>      | <span data-ttu-id="87e2f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87e2f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87e2f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87e2f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="87e2f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87e2f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87e2f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87e2f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87e2f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87e2f-117">Not supported.</span></span>    |
|<span data-ttu-id="87e2f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87e2f-118">Application</span></span> | <span data-ttu-id="87e2f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87e2f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87e2f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87e2f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="87e2f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87e2f-121">Request headers</span></span>
| <span data-ttu-id="87e2f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="87e2f-122">Name</span></span>       | <span data-ttu-id="87e2f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="87e2f-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87e2f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87e2f-124">Authorization</span></span>  | <span data-ttu-id="87e2f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87e2f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87e2f-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="87e2f-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="87e2f-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="87e2f-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="87e2f-130">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="87e2f-130">Path parameters</span></span>
<span data-ttu-id="87e2f-131">В поле путь укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="87e2f-131">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="87e2f-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="87e2f-132">Parameter</span></span>    | <span data-ttu-id="87e2f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="87e2f-133">Type</span></span>   |<span data-ttu-id="87e2f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="87e2f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87e2f-135">row</span><span class="sxs-lookup"><span data-stu-id="87e2f-135">row</span></span>|<span data-ttu-id="87e2f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="87e2f-136">Int32</span></span>|<span data-ttu-id="87e2f-p106">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="87e2f-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="87e2f-139">column</span><span class="sxs-lookup"><span data-stu-id="87e2f-139">column</span></span>|<span data-ttu-id="87e2f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="87e2f-140">Int32</span></span>|<span data-ttu-id="87e2f-p107">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="87e2f-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="87e2f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="87e2f-143">Response</span></span>

<span data-ttu-id="87e2f-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="87e2f-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87e2f-145">Пример</span><span class="sxs-lookup"><span data-stu-id="87e2f-145">Example</span></span>
<span data-ttu-id="87e2f-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="87e2f-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87e2f-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="87e2f-147">Request</span></span>
<span data-ttu-id="87e2f-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87e2f-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```

##### <a name="response"></a><span data-ttu-id="87e2f-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="87e2f-149">Response</span></span>
<span data-ttu-id="87e2f-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87e2f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
