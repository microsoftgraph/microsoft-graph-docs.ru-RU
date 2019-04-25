---
title: 'Range: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 59e25d3155caf13cac5441e6553116c9a54ceac6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546367"
---
# <a name="range-cell"></a><span data-ttu-id="a32eb-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="a32eb-105">Range: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a32eb-p102">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="a32eb-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="a32eb-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a32eb-109">Permissions</span></span>
<span data-ttu-id="a32eb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a32eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a32eb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a32eb-112">Permission type</span></span>      | <span data-ttu-id="a32eb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a32eb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a32eb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a32eb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a32eb-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a32eb-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a32eb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a32eb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a32eb-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a32eb-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a32eb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a32eb-118">Application</span></span> | <span data-ttu-id="a32eb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a32eb-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a32eb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a32eb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="a32eb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a32eb-121">Request headers</span></span>
| <span data-ttu-id="a32eb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a32eb-122">Name</span></span>       | <span data-ttu-id="a32eb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a32eb-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a32eb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a32eb-124">Authorization</span></span>  | <span data-ttu-id="a32eb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a32eb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a32eb-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a32eb-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="a32eb-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a32eb-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a32eb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a32eb-130">Request body</span></span>
<span data-ttu-id="a32eb-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a32eb-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a32eb-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="a32eb-132">Parameter</span></span>    | <span data-ttu-id="a32eb-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a32eb-133">Type</span></span>   |<span data-ttu-id="a32eb-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a32eb-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a32eb-135">row</span><span class="sxs-lookup"><span data-stu-id="a32eb-135">row</span></span>|<span data-ttu-id="a32eb-136">число</span><span class="sxs-lookup"><span data-stu-id="a32eb-136">number</span></span>|<span data-ttu-id="a32eb-p106">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="a32eb-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="a32eb-139">column</span><span class="sxs-lookup"><span data-stu-id="a32eb-139">column</span></span>|<span data-ttu-id="a32eb-140">number</span><span class="sxs-lookup"><span data-stu-id="a32eb-140">number</span></span>|<span data-ttu-id="a32eb-p107">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="a32eb-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="a32eb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a32eb-143">Response</span></span>

<span data-ttu-id="a32eb-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a32eb-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a32eb-145">Пример</span><span class="sxs-lookup"><span data-stu-id="a32eb-145">Example</span></span>
<span data-ttu-id="a32eb-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a32eb-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a32eb-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="a32eb-147">Request</span></span>
<span data-ttu-id="a32eb-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a32eb-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a32eb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="a32eb-149">Response</span></span>
<span data-ttu-id="a32eb-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a32eb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-cell.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
