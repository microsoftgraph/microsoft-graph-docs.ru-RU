---
title: Обновление диапазона
description: Обновление свойств объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5d53da9dc653d303ff126d3c237386f856ad98cb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055059"
---
# <a name="update-range"></a><span data-ttu-id="de5a0-103">Обновление диапазона</span><span class="sxs-lookup"><span data-stu-id="de5a0-103">Update range</span></span>

<span data-ttu-id="de5a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de5a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de5a0-105">Обновление свойств объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="de5a0-105">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de5a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de5a0-106">Permissions</span></span>
<span data-ttu-id="de5a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de5a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de5a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de5a0-109">Permission type</span></span>      | <span data-ttu-id="de5a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de5a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de5a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de5a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="de5a0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de5a0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de5a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de5a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de5a0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de5a0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de5a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de5a0-115">Application</span></span> | <span data-ttu-id="de5a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de5a0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de5a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de5a0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="de5a0-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de5a0-118">Optional request headers</span></span>
| <span data-ttu-id="de5a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="de5a0-119">Name</span></span>       | <span data-ttu-id="de5a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="de5a0-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="de5a0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de5a0-121">Authorization</span></span>  | <span data-ttu-id="de5a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de5a0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de5a0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="de5a0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="de5a0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="de5a0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de5a0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de5a0-127">Request body</span></span>
<span data-ttu-id="de5a0-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="de5a0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de5a0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="de5a0-131">Property</span></span>     | <span data-ttu-id="de5a0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="de5a0-132">Type</span></span>   |<span data-ttu-id="de5a0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="de5a0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de5a0-134">columnHidden</span><span class="sxs-lookup"><span data-stu-id="de5a0-134">columnHidden</span></span>|<span data-ttu-id="de5a0-135">boolean</span><span class="sxs-lookup"><span data-stu-id="de5a0-135">boolean</span></span>|<span data-ttu-id="de5a0-136">Указывает, скрыты ли все столбцы текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="de5a0-136">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="de5a0-137">formulas</span><span class="sxs-lookup"><span data-stu-id="de5a0-137">formulas</span></span>|<span data-ttu-id="de5a0-138">Json</span><span class="sxs-lookup"><span data-stu-id="de5a0-138">Json</span></span>|<span data-ttu-id="de5a0-139">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="de5a0-139">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="de5a0-140">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="de5a0-140">formulasLocal</span></span>|<span data-ttu-id="de5a0-141">Json</span><span class="sxs-lookup"><span data-stu-id="de5a0-141">Json</span></span>|<span data-ttu-id="de5a0-p105">Представляет формулу в нотации стиля A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула =SUM(A1, 1.5) превратится в "=СУММ(A1; 1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="de5a0-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="de5a0-144">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="de5a0-144">formulasR1C1</span></span>|<span data-ttu-id="de5a0-145">Json</span><span class="sxs-lookup"><span data-stu-id="de5a0-145">Json</span></span>|<span data-ttu-id="de5a0-146">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="de5a0-146">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="de5a0-147">numberFormat</span><span class="sxs-lookup"><span data-stu-id="de5a0-147">numberFormat</span></span>|<span data-ttu-id="de5a0-148">Json</span><span class="sxs-lookup"><span data-stu-id="de5a0-148">Json</span></span>|<span data-ttu-id="de5a0-149">Представляет код в числовом формате Excel для данной ячейки.</span><span class="sxs-lookup"><span data-stu-id="de5a0-149">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="de5a0-150">rowHidden</span><span class="sxs-lookup"><span data-stu-id="de5a0-150">rowHidden</span></span>|<span data-ttu-id="de5a0-151">boolean</span><span class="sxs-lookup"><span data-stu-id="de5a0-151">boolean</span></span>|<span data-ttu-id="de5a0-152">Указывает, скрыты ли все строки текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="de5a0-152">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="de5a0-153">values</span><span class="sxs-lookup"><span data-stu-id="de5a0-153">values</span></span>|<span data-ttu-id="de5a0-154">Json</span><span class="sxs-lookup"><span data-stu-id="de5a0-154">Json</span></span>|<span data-ttu-id="de5a0-p106">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="de5a0-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="de5a0-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="de5a0-158">Response</span></span>

<span data-ttu-id="de5a0-159">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [workbookRange](../resources/workbookrange.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de5a0-159">If successful, this method returns a `200 OK` response code and updated [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de5a0-160">Пример</span><span class="sxs-lookup"><span data-stu-id="de5a0-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de5a0-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="de5a0-161">Request</span></span>
<span data-ttu-id="de5a0-p107">Ниже приведен пример запроса. Он обновляет диапазон — значения числовой формат и формулу. Значение `null` сообщает API, что в данном случае нужно пропустить ячейку. Значения, числовые форматы и формулы можно обновлять по отдельности или в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="de5a0-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 


# <a name="http"></a>[<span data-ttu-id="de5a0-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="de5a0-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/sheet1/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formulas" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
# <a name="javascript"></a>[<span data-ttu-id="de5a0-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de5a0-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de5a0-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="de5a0-168">Response</span></span>
<span data-ttu-id="de5a0-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de5a0-169">Here is an example of the response.</span></span> <span data-ttu-id="de5a0-170">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de5a0-170">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


