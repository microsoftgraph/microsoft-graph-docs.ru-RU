---
title: Обновление книгиChartFont
description: Обновление свойств объекта книгиChartFont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b17313a909eddf7660bba1cca214fca54a9113a9
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574554"
---
# <a name="update-chartfont"></a><span data-ttu-id="a7d12-103">Обновление объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="a7d12-103">Update chartfont</span></span>

<span data-ttu-id="a7d12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7d12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7d12-105">Обновление свойств объекта chartfont.</span><span class="sxs-lookup"><span data-stu-id="a7d12-105">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7d12-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7d12-106">Permissions</span></span>
<span data-ttu-id="a7d12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7d12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7d12-109">Permission type</span></span>      | <span data-ttu-id="a7d12-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7d12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7d12-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7d12-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7d12-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7d12-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7d12-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7d12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7d12-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7d12-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7d12-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7d12-115">Application</span></span> | <span data-ttu-id="a7d12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7d12-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7d12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7d12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="a7d12-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7d12-118">Optional request headers</span></span>
| <span data-ttu-id="a7d12-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a7d12-119">Name</span></span>       | <span data-ttu-id="a7d12-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d12-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a7d12-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7d12-121">Authorization</span></span>  | <span data-ttu-id="a7d12-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7d12-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7d12-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a7d12-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a7d12-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a7d12-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7d12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7d12-127">Request body</span></span>
<span data-ttu-id="a7d12-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a7d12-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a7d12-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7d12-131">Property</span></span>     | <span data-ttu-id="a7d12-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a7d12-132">Type</span></span>   |<span data-ttu-id="a7d12-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d12-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7d12-134">bold</span><span class="sxs-lookup"><span data-stu-id="a7d12-134">bold</span></span>|<span data-ttu-id="a7d12-135">boolean</span><span class="sxs-lookup"><span data-stu-id="a7d12-135">boolean</span></span>|<span data-ttu-id="a7d12-136">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="a7d12-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="a7d12-137">color</span><span class="sxs-lookup"><span data-stu-id="a7d12-137">color</span></span>|<span data-ttu-id="a7d12-138">string</span><span class="sxs-lookup"><span data-stu-id="a7d12-138">string</span></span>|<span data-ttu-id="a7d12-p105">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="a7d12-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="a7d12-142">italic</span><span class="sxs-lookup"><span data-stu-id="a7d12-142">italic</span></span>|<span data-ttu-id="a7d12-143">boolean</span><span class="sxs-lookup"><span data-stu-id="a7d12-143">boolean</span></span>|<span data-ttu-id="a7d12-144">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="a7d12-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="a7d12-145">name</span><span class="sxs-lookup"><span data-stu-id="a7d12-145">name</span></span>|<span data-ttu-id="a7d12-146">string</span><span class="sxs-lookup"><span data-stu-id="a7d12-146">string</span></span>|<span data-ttu-id="a7d12-147">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="a7d12-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="a7d12-148">size</span><span class="sxs-lookup"><span data-stu-id="a7d12-148">size</span></span>|<span data-ttu-id="a7d12-149">Double</span><span class="sxs-lookup"><span data-stu-id="a7d12-149">double</span></span>|<span data-ttu-id="a7d12-150">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="a7d12-150">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="a7d12-151">underline</span><span class="sxs-lookup"><span data-stu-id="a7d12-151">underline</span></span>|<span data-ttu-id="a7d12-152">string</span><span class="sxs-lookup"><span data-stu-id="a7d12-152">string</span></span>|<span data-ttu-id="a7d12-p106">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="a7d12-p106">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="a7d12-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7d12-155">Response</span></span>

<span data-ttu-id="a7d12-156">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [книгиChartFont](../resources/workbookchartfont.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7d12-156">If successful, this method returns a `200 OK` response code and updated [workbookChartFont](../resources/workbookchartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7d12-157">Пример</span><span class="sxs-lookup"><span data-stu-id="a7d12-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7d12-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7d12-158">Request</span></span>
<span data-ttu-id="a7d12-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7d12-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7d12-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7d12-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
# <a name="c"></a>[<span data-ttu-id="a7d12-161">C#</span><span class="sxs-lookup"><span data-stu-id="a7d12-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7d12-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7d12-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7d12-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7d12-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7d12-164">Java</span><span class="sxs-lookup"><span data-stu-id="a7d12-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartfont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7d12-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7d12-165">Response</span></span>
<span data-ttu-id="a7d12-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7d12-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


