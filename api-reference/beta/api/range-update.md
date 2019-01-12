---
title: Обновление диапазона
description: Обновление свойств объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ca9744fa00fec2928b019dd45c7d503f7f35ee77
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975990"
---
# <a name="update-range"></a><span data-ttu-id="0e154-103">Обновление диапазона</span><span class="sxs-lookup"><span data-stu-id="0e154-103">Update range</span></span>

> <span data-ttu-id="0e154-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e154-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e154-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e154-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e154-106">Обновление свойств объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="0e154-106">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e154-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e154-107">Permissions</span></span>
<span data-ttu-id="0e154-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e154-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e154-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e154-110">Permission type</span></span>      | <span data-ttu-id="0e154-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e154-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e154-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e154-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e154-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e154-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e154-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e154-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e154-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e154-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e154-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e154-116">Application</span></span> | <span data-ttu-id="0e154-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e154-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e154-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e154-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="0e154-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e154-119">Optional request headers</span></span>
| <span data-ttu-id="0e154-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0e154-120">Name</span></span>       | <span data-ttu-id="0e154-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0e154-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0e154-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e154-122">Authorization</span></span>  | <span data-ttu-id="0e154-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e154-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e154-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e154-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e154-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0e154-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e154-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e154-128">Request body</span></span>
<span data-ttu-id="0e154-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0e154-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e154-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e154-132">Property</span></span>     | <span data-ttu-id="0e154-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0e154-133">Type</span></span>   |<span data-ttu-id="0e154-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0e154-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e154-135">columnHidden</span><span class="sxs-lookup"><span data-stu-id="0e154-135">columnHidden</span></span>|<span data-ttu-id="0e154-136">boolean</span><span class="sxs-lookup"><span data-stu-id="0e154-136">boolean</span></span>|<span data-ttu-id="0e154-137">Указывает, скрыты ли все столбцы текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="0e154-137">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="0e154-138">formulas</span><span class="sxs-lookup"><span data-stu-id="0e154-138">formulas</span></span>|<span data-ttu-id="0e154-139">json</span><span class="sxs-lookup"><span data-stu-id="0e154-139">json</span></span>|<span data-ttu-id="0e154-140">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="0e154-140">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="0e154-141">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="0e154-141">formulasLocal</span></span>|<span data-ttu-id="0e154-142">json</span><span class="sxs-lookup"><span data-stu-id="0e154-142">json</span></span>|<span data-ttu-id="0e154-p106">Представляет формулу в нотации стиля A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула =SUM(A1, 1.5) превратится в "=СУММ(A1; 1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="0e154-p106">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="0e154-145">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="0e154-145">formulasR1C1</span></span>|<span data-ttu-id="0e154-146">json</span><span class="sxs-lookup"><span data-stu-id="0e154-146">json</span></span>|<span data-ttu-id="0e154-147">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="0e154-147">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="0e154-148">numberFormat</span><span class="sxs-lookup"><span data-stu-id="0e154-148">numberFormat</span></span>|<span data-ttu-id="0e154-149">json</span><span class="sxs-lookup"><span data-stu-id="0e154-149">json</span></span>|<span data-ttu-id="0e154-150">Представляет код числового формата Excel для данной ячейки.</span><span class="sxs-lookup"><span data-stu-id="0e154-150">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="0e154-151">rowHidden</span><span class="sxs-lookup"><span data-stu-id="0e154-151">rowHidden</span></span>|<span data-ttu-id="0e154-152">boolean</span><span class="sxs-lookup"><span data-stu-id="0e154-152">boolean</span></span>|<span data-ttu-id="0e154-153">Указывает, скрыты ли все строки текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="0e154-153">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="0e154-154">values</span><span class="sxs-lookup"><span data-stu-id="0e154-154">values</span></span>|<span data-ttu-id="0e154-155">json</span><span class="sxs-lookup"><span data-stu-id="0e154-155">json</span></span>|<span data-ttu-id="0e154-p107">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="0e154-p107">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="0e154-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e154-159">Response</span></span>

<span data-ttu-id="0e154-160">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Range](../resources/range.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e154-160">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e154-161">Пример</span><span class="sxs-lookup"><span data-stu-id="0e154-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e154-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e154-162">Request</span></span>
<span data-ttu-id="0e154-p108">Ниже приведен пример запроса. Он обновляет диапазон — значения числовой формат и формулу. Значение `null` сообщает API, что в данном случае нужно пропустить ячейку. Значения, числовые форматы и формулы можно обновлять по отдельности или в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="0e154-p108">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="0e154-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e154-167">Response</span></span>
<span data-ttu-id="0e154-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e154-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
