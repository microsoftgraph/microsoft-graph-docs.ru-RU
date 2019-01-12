---
title: 'Worksheet: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 96069c11d8e520b64854eb7a2a72dc9d5f6de25b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967303"
---
# <a name="worksheet-cell"></a><span data-ttu-id="0e7a1-104">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="0e7a1-104">Worksheet: Cell</span></span>

<span data-ttu-id="0e7a1-p102">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e7a1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e7a1-107">Permissions</span></span>
<span data-ttu-id="0e7a1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e7a1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e7a1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e7a1-110">Permission type</span></span>      | <span data-ttu-id="0e7a1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e7a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e7a1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e7a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e7a1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e7a1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e7a1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e7a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e7a1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-115">Not supported.</span></span>    |
|<span data-ttu-id="0e7a1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e7a1-116">Application</span></span> | <span data-ttu-id="0e7a1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e7a1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e7a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="0e7a1-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="0e7a1-119">Function parameters</span></span>
<span data-ttu-id="0e7a1-120">В поле путь запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-120">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="0e7a1-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="0e7a1-121">Parameter</span></span>    | <span data-ttu-id="0e7a1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0e7a1-122">Type</span></span>   |<span data-ttu-id="0e7a1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0e7a1-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e7a1-124">row</span><span class="sxs-lookup"><span data-stu-id="0e7a1-124">row</span></span>|<span data-ttu-id="0e7a1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0e7a1-125">Int32</span></span>|<span data-ttu-id="0e7a1-p104">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="0e7a1-128">column</span><span class="sxs-lookup"><span data-stu-id="0e7a1-128">column</span></span>|<span data-ttu-id="0e7a1-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0e7a1-129">Int32</span></span>|<span data-ttu-id="0e7a1-p105">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0e7a1-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e7a1-132">Request headers</span></span>
| <span data-ttu-id="0e7a1-133">Имя</span><span class="sxs-lookup"><span data-stu-id="0e7a1-133">Name</span></span>       | <span data-ttu-id="0e7a1-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0e7a1-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e7a1-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e7a1-135">Authorization</span></span>  | <span data-ttu-id="0e7a1-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e7a1-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e7a1-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e7a1-p107">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e7a1-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e7a1-141">Request body</span></span>
<span data-ttu-id="0e7a1-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e7a1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e7a1-143">Response</span></span>

<span data-ttu-id="0e7a1-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e7a1-145">Пример</span><span class="sxs-lookup"><span data-stu-id="0e7a1-145">Example</span></span>
<span data-ttu-id="0e7a1-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e7a1-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e7a1-147">Request</span></span>
<span data-ttu-id="0e7a1-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="0e7a1-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e7a1-149">Response</span></span>
<span data-ttu-id="0e7a1-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e7a1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
