---
title: Обновление объекта rangefont
description: Обновление свойств объекта rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 637a7df54190884f7ccd400dc9be0c3b3f4ea0a6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051055"
---
# <a name="update-rangefont"></a><span data-ttu-id="8edd8-103">Обновление объекта rangefont</span><span class="sxs-lookup"><span data-stu-id="8edd8-103">Update rangefont</span></span>

<span data-ttu-id="8edd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8edd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8edd8-105">Обновление свойств объекта rangefont.</span><span class="sxs-lookup"><span data-stu-id="8edd8-105">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8edd8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8edd8-106">Permissions</span></span>
<span data-ttu-id="8edd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8edd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8edd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8edd8-109">Permission type</span></span>      | <span data-ttu-id="8edd8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8edd8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8edd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8edd8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8edd8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8edd8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8edd8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8edd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8edd8-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8edd8-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8edd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8edd8-115">Application</span></span> | <span data-ttu-id="8edd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8edd8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8edd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8edd8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/font
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/font
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="8edd8-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8edd8-118">Optional request headers</span></span>
| <span data-ttu-id="8edd8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8edd8-119">Name</span></span>       | <span data-ttu-id="8edd8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8edd8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8edd8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8edd8-121">Authorization</span></span>  | <span data-ttu-id="8edd8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8edd8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8edd8-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8edd8-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8edd8-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8edd8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8edd8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8edd8-127">Request body</span></span>
<span data-ttu-id="8edd8-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8edd8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8edd8-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8edd8-131">Property</span></span>     | <span data-ttu-id="8edd8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8edd8-132">Type</span></span>   |<span data-ttu-id="8edd8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8edd8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8edd8-134">bold</span><span class="sxs-lookup"><span data-stu-id="8edd8-134">bold</span></span>|<span data-ttu-id="8edd8-135">boolean</span><span class="sxs-lookup"><span data-stu-id="8edd8-135">boolean</span></span>|<span data-ttu-id="8edd8-136">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="8edd8-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="8edd8-137">color</span><span class="sxs-lookup"><span data-stu-id="8edd8-137">color</span></span>|<span data-ttu-id="8edd8-138">string</span><span class="sxs-lookup"><span data-stu-id="8edd8-138">string</span></span>|<span data-ttu-id="8edd8-p105">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="8edd8-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="8edd8-142">italic</span><span class="sxs-lookup"><span data-stu-id="8edd8-142">italic</span></span>|<span data-ttu-id="8edd8-143">boolean</span><span class="sxs-lookup"><span data-stu-id="8edd8-143">boolean</span></span>|<span data-ttu-id="8edd8-144">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="8edd8-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="8edd8-145">name</span><span class="sxs-lookup"><span data-stu-id="8edd8-145">name</span></span>|<span data-ttu-id="8edd8-146">string</span><span class="sxs-lookup"><span data-stu-id="8edd8-146">string</span></span>|<span data-ttu-id="8edd8-147">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="8edd8-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="8edd8-148">size</span><span class="sxs-lookup"><span data-stu-id="8edd8-148">size</span></span>|<span data-ttu-id="8edd8-149">double</span><span class="sxs-lookup"><span data-stu-id="8edd8-149">double</span></span>|<span data-ttu-id="8edd8-150">размер шрифта</span><span class="sxs-lookup"><span data-stu-id="8edd8-150">Font size.</span></span>|
|<span data-ttu-id="8edd8-151">underline</span><span class="sxs-lookup"><span data-stu-id="8edd8-151">underline</span></span>|<span data-ttu-id="8edd8-152">string</span><span class="sxs-lookup"><span data-stu-id="8edd8-152">string</span></span>|<span data-ttu-id="8edd8-p106">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="8edd8-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="8edd8-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edd8-155">Response</span></span>

<span data-ttu-id="8edd8-156">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [workbookRangeFont](../resources/workbookrangefont.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8edd8-156">If successful, this method returns a `200 OK` response code and updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8edd8-157">Пример</span><span class="sxs-lookup"><span data-stu-id="8edd8-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8edd8-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="8edd8-158">Request</span></span>
<span data-ttu-id="8edd8-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8edd8-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8edd8-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="8edd8-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8edd8-161">C#</span><span class="sxs-lookup"><span data-stu-id="8edd8-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8edd8-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8edd8-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8edd8-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8edd8-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8edd8-164">Java</span><span class="sxs-lookup"><span data-stu-id="8edd8-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8edd8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edd8-165">Response</span></span>
<span data-ttu-id="8edd8-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8edd8-166">Here is an example of the response.</span></span> <span data-ttu-id="8edd8-167">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8edd8-167">Note: The response object shown here might be shortened for readability.</span></span>
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


