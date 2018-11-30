---
title: 'Range: Cell'
description: Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.
ms.openlocfilehash: 641de24869d5a57b08f339b7552d67d07be7b75c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082116"
---
# <a name="range-cell"></a><span data-ttu-id="9fde0-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="9fde0-105">Range: Cell</span></span>

> <span data-ttu-id="9fde0-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9fde0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fde0-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fde0-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fde0-p103">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="9fde0-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="9fde0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fde0-111">Permissions</span></span>
<span data-ttu-id="9fde0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fde0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fde0-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fde0-114">Permission type</span></span>      | <span data-ttu-id="9fde0-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fde0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fde0-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fde0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9fde0-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fde0-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9fde0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fde0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fde0-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fde0-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9fde0-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fde0-120">Application</span></span> | <span data-ttu-id="9fde0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fde0-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fde0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fde0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="9fde0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fde0-123">Request headers</span></span>
| <span data-ttu-id="9fde0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9fde0-124">Name</span></span>       | <span data-ttu-id="9fde0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9fde0-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9fde0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fde0-126">Authorization</span></span>  | <span data-ttu-id="9fde0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fde0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9fde0-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9fde0-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="9fde0-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9fde0-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fde0-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fde0-132">Request body</span></span>
<span data-ttu-id="9fde0-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9fde0-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9fde0-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="9fde0-134">Parameter</span></span>    | <span data-ttu-id="9fde0-135">Тип</span><span class="sxs-lookup"><span data-stu-id="9fde0-135">Type</span></span>   |<span data-ttu-id="9fde0-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9fde0-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fde0-137">row</span><span class="sxs-lookup"><span data-stu-id="9fde0-137">row</span></span>|<span data-ttu-id="9fde0-138">number</span><span class="sxs-lookup"><span data-stu-id="9fde0-138">number</span></span>|<span data-ttu-id="9fde0-p107">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="9fde0-p107">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="9fde0-141">column</span><span class="sxs-lookup"><span data-stu-id="9fde0-141">column</span></span>|<span data-ttu-id="9fde0-142">number</span><span class="sxs-lookup"><span data-stu-id="9fde0-142">number</span></span>|<span data-ttu-id="9fde0-p108">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="9fde0-p108">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="9fde0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fde0-145">Response</span></span>

<span data-ttu-id="9fde0-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9fde0-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fde0-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9fde0-147">Example</span></span>
<span data-ttu-id="9fde0-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9fde0-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9fde0-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fde0-149">Request</span></span>
<span data-ttu-id="9fde0-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fde0-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9fde0-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fde0-151">Response</span></span>
<span data-ttu-id="9fde0-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9fde0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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