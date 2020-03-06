---
title: 'Worksheet: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b447bed5bd6e77faa941a3c228f78b804d0204f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508697"
---
# <a name="worksheet-cell"></a><span data-ttu-id="44c16-104">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="44c16-104">Worksheet: Cell</span></span>

<span data-ttu-id="44c16-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44c16-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44c16-p102">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="44c16-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="44c16-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44c16-108">Permissions</span></span>
<span data-ttu-id="44c16-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44c16-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44c16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44c16-111">Permission type</span></span>      | <span data-ttu-id="44c16-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44c16-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44c16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44c16-113">Delegated (work or school account)</span></span> | <span data-ttu-id="44c16-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44c16-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44c16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44c16-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44c16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44c16-116">Not supported.</span></span>    |
|<span data-ttu-id="44c16-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44c16-117">Application</span></span> | <span data-ttu-id="44c16-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44c16-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44c16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44c16-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="44c16-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="44c16-120">Function parameters</span></span>
<span data-ttu-id="44c16-121">В пути запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="44c16-121">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="44c16-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="44c16-122">Parameter</span></span>    | <span data-ttu-id="44c16-123">Тип</span><span class="sxs-lookup"><span data-stu-id="44c16-123">Type</span></span>   |<span data-ttu-id="44c16-124">Описание</span><span class="sxs-lookup"><span data-stu-id="44c16-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44c16-125">row</span><span class="sxs-lookup"><span data-stu-id="44c16-125">row</span></span>|<span data-ttu-id="44c16-126">Int32</span><span class="sxs-lookup"><span data-stu-id="44c16-126">Int32</span></span>|<span data-ttu-id="44c16-p104">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="44c16-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="44c16-129">column</span><span class="sxs-lookup"><span data-stu-id="44c16-129">column</span></span>|<span data-ttu-id="44c16-130">Int32</span><span class="sxs-lookup"><span data-stu-id="44c16-130">Int32</span></span>|<span data-ttu-id="44c16-131">Номер столбца ячейки, которую требуется извлечь.</span><span class="sxs-lookup"><span data-stu-id="44c16-131">Column number of the cell to be retrieved.</span></span> <span data-ttu-id="44c16-132">Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="44c16-132">Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="44c16-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44c16-133">Request headers</span></span>
| <span data-ttu-id="44c16-134">Имя</span><span class="sxs-lookup"><span data-stu-id="44c16-134">Name</span></span>       | <span data-ttu-id="44c16-135">Описание</span><span class="sxs-lookup"><span data-stu-id="44c16-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44c16-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44c16-136">Authorization</span></span>  | <span data-ttu-id="44c16-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44c16-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44c16-139">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="44c16-139">Workbook-Session-Id</span></span>  | <span data-ttu-id="44c16-p107">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="44c16-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44c16-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44c16-142">Request body</span></span>
<span data-ttu-id="44c16-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44c16-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44c16-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="44c16-144">Response</span></span>

<span data-ttu-id="44c16-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="44c16-145">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44c16-146">Пример</span><span class="sxs-lookup"><span data-stu-id="44c16-146">Example</span></span>
<span data-ttu-id="44c16-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="44c16-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="44c16-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="44c16-148">Request</span></span>
<span data-ttu-id="44c16-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44c16-149">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="44c16-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="44c16-150">Response</span></span>
<span data-ttu-id="44c16-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44c16-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
