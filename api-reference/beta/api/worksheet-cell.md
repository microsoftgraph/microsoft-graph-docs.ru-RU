---
title: 'Worksheet: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: be5b461af5a5c8d3586f6af2819d5497a0d0b473
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576836"
---
# <a name="worksheet-cell"></a><span data-ttu-id="516fe-104">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="516fe-104">Worksheet: Cell</span></span>

<span data-ttu-id="516fe-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="516fe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="516fe-p102">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="516fe-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="516fe-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="516fe-108">Permissions</span></span>
<span data-ttu-id="516fe-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="516fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="516fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="516fe-111">Permission type</span></span>      | <span data-ttu-id="516fe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="516fe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="516fe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="516fe-113">Delegated (work or school account)</span></span> | <span data-ttu-id="516fe-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="516fe-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="516fe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="516fe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="516fe-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="516fe-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="516fe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="516fe-117">Application</span></span> | <span data-ttu-id="516fe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="516fe-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="516fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="516fe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row={row},column={column})
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="516fe-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="516fe-120">Function parameters</span></span>
<span data-ttu-id="516fe-121">В пути запроса укай следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="516fe-121">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="516fe-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="516fe-122">Parameter</span></span>    | <span data-ttu-id="516fe-123">Тип</span><span class="sxs-lookup"><span data-stu-id="516fe-123">Type</span></span>   |<span data-ttu-id="516fe-124">Описание</span><span class="sxs-lookup"><span data-stu-id="516fe-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="516fe-125">row</span><span class="sxs-lookup"><span data-stu-id="516fe-125">row</span></span>|<span data-ttu-id="516fe-126">Int32</span><span class="sxs-lookup"><span data-stu-id="516fe-126">Int32</span></span>|<span data-ttu-id="516fe-p104">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="516fe-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="516fe-129">column</span><span class="sxs-lookup"><span data-stu-id="516fe-129">column</span></span>|<span data-ttu-id="516fe-130">Int32</span><span class="sxs-lookup"><span data-stu-id="516fe-130">Int32</span></span>|<span data-ttu-id="516fe-131">Номер столбца ячейки, которую требуется извлечь.</span><span class="sxs-lookup"><span data-stu-id="516fe-131">Column number of the cell to be retrieved.</span></span> <span data-ttu-id="516fe-132">Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="516fe-132">Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="516fe-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="516fe-133">Request headers</span></span>
| <span data-ttu-id="516fe-134">Имя</span><span class="sxs-lookup"><span data-stu-id="516fe-134">Name</span></span>       | <span data-ttu-id="516fe-135">Описание</span><span class="sxs-lookup"><span data-stu-id="516fe-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="516fe-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="516fe-136">Authorization</span></span>  | <span data-ttu-id="516fe-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="516fe-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="516fe-139">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="516fe-139">Workbook-Session-Id</span></span>  | <span data-ttu-id="516fe-p107">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="516fe-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="516fe-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="516fe-142">Request body</span></span>
<span data-ttu-id="516fe-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="516fe-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="516fe-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="516fe-144">Response</span></span>

<span data-ttu-id="516fe-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="516fe-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="516fe-146">Пример</span><span class="sxs-lookup"><span data-stu-id="516fe-146">Example</span></span>
<span data-ttu-id="516fe-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="516fe-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="516fe-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="516fe-148">Request</span></span>
<span data-ttu-id="516fe-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="516fe-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="516fe-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="516fe-150">Response</span></span>
<span data-ttu-id="516fe-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="516fe-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


