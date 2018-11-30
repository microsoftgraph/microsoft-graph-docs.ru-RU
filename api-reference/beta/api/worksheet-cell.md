---
title: 'Worksheet: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.
ms.openlocfilehash: 5c85bf21e88b6b483abe1631c038e9239d3779d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076262"
---
# <a name="worksheet-cell"></a><span data-ttu-id="6c99a-104">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="6c99a-104">Worksheet: Cell</span></span>

> <span data-ttu-id="6c99a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6c99a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c99a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c99a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c99a-p103">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="6c99a-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c99a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c99a-109">Permissions</span></span>
<span data-ttu-id="6c99a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c99a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c99a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c99a-112">Permission type</span></span>      | <span data-ttu-id="6c99a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c99a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c99a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c99a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6c99a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c99a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c99a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c99a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c99a-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c99a-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c99a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c99a-118">Application</span></span> | <span data-ttu-id="6c99a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c99a-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c99a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c99a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="6c99a-121">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="6c99a-121">Function parameters</span></span>
<span data-ttu-id="6c99a-122">В поле путь запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="6c99a-122">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="6c99a-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="6c99a-123">Parameter</span></span>    | <span data-ttu-id="6c99a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="6c99a-124">Type</span></span>   |<span data-ttu-id="6c99a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6c99a-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c99a-126">row</span><span class="sxs-lookup"><span data-stu-id="6c99a-126">row</span></span>|<span data-ttu-id="6c99a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6c99a-127">Int32</span></span>|<span data-ttu-id="6c99a-p105">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="6c99a-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="6c99a-130">column</span><span class="sxs-lookup"><span data-stu-id="6c99a-130">column</span></span>|<span data-ttu-id="6c99a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6c99a-131">Int32</span></span>|<span data-ttu-id="6c99a-p106">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="6c99a-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6c99a-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c99a-134">Request headers</span></span>
| <span data-ttu-id="6c99a-135">Имя</span><span class="sxs-lookup"><span data-stu-id="6c99a-135">Name</span></span>       | <span data-ttu-id="6c99a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6c99a-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6c99a-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c99a-137">Authorization</span></span>  | <span data-ttu-id="6c99a-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c99a-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c99a-140">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6c99a-140">Workbook-Session-Id</span></span>  | <span data-ttu-id="6c99a-p108">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6c99a-p108">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c99a-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c99a-143">Request body</span></span>
<span data-ttu-id="6c99a-144">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c99a-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c99a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c99a-145">Response</span></span>

<span data-ttu-id="6c99a-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6c99a-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c99a-147">Пример</span><span class="sxs-lookup"><span data-stu-id="6c99a-147">Example</span></span>
<span data-ttu-id="6c99a-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6c99a-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6c99a-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c99a-149">Request</span></span>
<span data-ttu-id="6c99a-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c99a-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="6c99a-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c99a-151">Response</span></span>
<span data-ttu-id="6c99a-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6c99a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
