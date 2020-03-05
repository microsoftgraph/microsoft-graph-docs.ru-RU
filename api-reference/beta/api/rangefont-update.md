---
title: Обновление объекта rangefont
description: Обновление свойств объекта rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 134768bcb6105c25e1265c5401d26660ae6dd8d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454609"
---
# <a name="update-rangefont"></a><span data-ttu-id="f6ca6-103">Обновление объекта rangefont</span><span class="sxs-lookup"><span data-stu-id="f6ca6-103">Update rangefont</span></span>

<span data-ttu-id="f6ca6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f6ca6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6ca6-105">Обновление свойств объекта rangefont.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-105">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6ca6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ca6-106">Permissions</span></span>
<span data-ttu-id="f6ca6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6ca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6ca6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ca6-109">Permission type</span></span>      | <span data-ttu-id="f6ca6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6ca6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6ca6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6ca6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6ca6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6ca6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f6ca6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6ca6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6ca6-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6ca6-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f6ca6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6ca6-115">Application</span></span> | <span data-ttu-id="f6ca6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6ca6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6ca6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="f6ca6-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6ca6-118">Optional request headers</span></span>
| <span data-ttu-id="f6ca6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f6ca6-119">Name</span></span>       | <span data-ttu-id="f6ca6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ca6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f6ca6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6ca6-121">Authorization</span></span>  | <span data-ttu-id="f6ca6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6ca6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f6ca6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f6ca6-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6ca6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6ca6-127">Request body</span></span>
<span data-ttu-id="f6ca6-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f6ca6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6ca6-131">Property</span></span>     | <span data-ttu-id="f6ca6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f6ca6-132">Type</span></span>   |<span data-ttu-id="f6ca6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ca6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6ca6-134">bold</span><span class="sxs-lookup"><span data-stu-id="f6ca6-134">bold</span></span>|<span data-ttu-id="f6ca6-135">boolean</span><span class="sxs-lookup"><span data-stu-id="f6ca6-135">boolean</span></span>|<span data-ttu-id="f6ca6-136">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="f6ca6-137">color</span><span class="sxs-lookup"><span data-stu-id="f6ca6-137">color</span></span>|<span data-ttu-id="f6ca6-138">строка</span><span class="sxs-lookup"><span data-stu-id="f6ca6-138">string</span></span>|<span data-ttu-id="f6ca6-p105">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="f6ca6-142">italic</span><span class="sxs-lookup"><span data-stu-id="f6ca6-142">italic</span></span>|<span data-ttu-id="f6ca6-143">boolean</span><span class="sxs-lookup"><span data-stu-id="f6ca6-143">boolean</span></span>|<span data-ttu-id="f6ca6-144">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="f6ca6-145">name</span><span class="sxs-lookup"><span data-stu-id="f6ca6-145">name</span></span>|<span data-ttu-id="f6ca6-146">string</span><span class="sxs-lookup"><span data-stu-id="f6ca6-146">string</span></span>|<span data-ttu-id="f6ca6-147">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="f6ca6-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="f6ca6-148">size</span><span class="sxs-lookup"><span data-stu-id="f6ca6-148">size</span></span>|<span data-ttu-id="f6ca6-149">double</span><span class="sxs-lookup"><span data-stu-id="f6ca6-149">double</span></span>|<span data-ttu-id="f6ca6-150">размер шрифта</span><span class="sxs-lookup"><span data-stu-id="f6ca6-150">Font size.</span></span>|
|<span data-ttu-id="f6ca6-151">underline</span><span class="sxs-lookup"><span data-stu-id="f6ca6-151">underline</span></span>|<span data-ttu-id="f6ca6-152">string</span><span class="sxs-lookup"><span data-stu-id="f6ca6-152">string</span></span>|<span data-ttu-id="f6ca6-p106">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="f6ca6-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6ca6-155">Response</span></span>

<span data-ttu-id="f6ca6-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжефонт](../resources/workbookrangefont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-156">If successful, this method returns a `200 OK` response code and updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6ca6-157">Пример</span><span class="sxs-lookup"><span data-stu-id="f6ca6-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6ca6-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6ca6-158">Request</span></span>
<span data-ttu-id="f6ca6-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6ca6-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6ca6-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/font
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
# <a name="c"></a>[<span data-ttu-id="f6ca6-161">C#</span><span class="sxs-lookup"><span data-stu-id="f6ca6-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6ca6-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6ca6-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6ca6-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6ca6-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f6ca6-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6ca6-164">Response</span></span>
<span data-ttu-id="f6ca6-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6ca6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
