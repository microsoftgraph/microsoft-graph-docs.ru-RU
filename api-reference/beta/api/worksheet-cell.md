---
title: 'Worksheet: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 577b7d4c2d92e8af60bf5ab26476915edc4c3cbc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092904"
---
# <a name="worksheet-cell"></a><span data-ttu-id="214fb-104">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="214fb-104">Worksheet: Cell</span></span>

<span data-ttu-id="214fb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="214fb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="214fb-p102">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="214fb-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="214fb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="214fb-108">Permissions</span></span>
<span data-ttu-id="214fb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="214fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="214fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="214fb-111">Permission type</span></span>      | <span data-ttu-id="214fb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="214fb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="214fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="214fb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="214fb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214fb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="214fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="214fb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="214fb-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214fb-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="214fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="214fb-117">Application</span></span> | <span data-ttu-id="214fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="214fb-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="214fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="214fb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="214fb-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="214fb-120">Function parameters</span></span>
<span data-ttu-id="214fb-121">В пути запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="214fb-121">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="214fb-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="214fb-122">Parameter</span></span>    | <span data-ttu-id="214fb-123">Тип</span><span class="sxs-lookup"><span data-stu-id="214fb-123">Type</span></span>   |<span data-ttu-id="214fb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="214fb-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="214fb-125">row</span><span class="sxs-lookup"><span data-stu-id="214fb-125">row</span></span>|<span data-ttu-id="214fb-126">Int32</span><span class="sxs-lookup"><span data-stu-id="214fb-126">Int32</span></span>|<span data-ttu-id="214fb-p104">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="214fb-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="214fb-129">column</span><span class="sxs-lookup"><span data-stu-id="214fb-129">column</span></span>|<span data-ttu-id="214fb-130">Int32</span><span class="sxs-lookup"><span data-stu-id="214fb-130">Int32</span></span>|<span data-ttu-id="214fb-131">Номер столбца ячейки, которую требуется извлечь.</span><span class="sxs-lookup"><span data-stu-id="214fb-131">Column number of the cell to be retrieved.</span></span> <span data-ttu-id="214fb-132">Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="214fb-132">Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="214fb-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="214fb-133">Request headers</span></span>
| <span data-ttu-id="214fb-134">Имя</span><span class="sxs-lookup"><span data-stu-id="214fb-134">Name</span></span>       | <span data-ttu-id="214fb-135">Описание</span><span class="sxs-lookup"><span data-stu-id="214fb-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="214fb-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="214fb-136">Authorization</span></span>  | <span data-ttu-id="214fb-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="214fb-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="214fb-139">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="214fb-139">Workbook-Session-Id</span></span>  | <span data-ttu-id="214fb-p107">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="214fb-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="214fb-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="214fb-142">Request body</span></span>
<span data-ttu-id="214fb-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="214fb-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="214fb-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="214fb-144">Response</span></span>

<span data-ttu-id="214fb-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="214fb-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="214fb-146">Пример</span><span class="sxs-lookup"><span data-stu-id="214fb-146">Example</span></span>
<span data-ttu-id="214fb-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="214fb-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="214fb-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="214fb-148">Request</span></span>
<span data-ttu-id="214fb-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="214fb-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="214fb-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="214fb-150">Response</span></span>
<span data-ttu-id="214fb-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="214fb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


