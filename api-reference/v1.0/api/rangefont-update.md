---
title: Обновление объекта rangefont
description: Обновление свойств объекта rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 660e7853a13464a902aee944a61f0134ac0263a3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510510"
---
# <a name="update-rangefont"></a><span data-ttu-id="0deaa-103">Обновление объекта rangefont</span><span class="sxs-lookup"><span data-stu-id="0deaa-103">Update rangefont</span></span>

<span data-ttu-id="0deaa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0deaa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0deaa-105">Обновление свойств объекта rangefont.</span><span class="sxs-lookup"><span data-stu-id="0deaa-105">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0deaa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0deaa-106">Permissions</span></span>
<span data-ttu-id="0deaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0deaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0deaa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0deaa-109">Permission type</span></span>      | <span data-ttu-id="0deaa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0deaa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0deaa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0deaa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0deaa-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0deaa-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0deaa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0deaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0deaa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0deaa-114">Not supported.</span></span>    |
|<span data-ttu-id="0deaa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0deaa-115">Application</span></span> | <span data-ttu-id="0deaa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0deaa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0deaa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0deaa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="request-headers"></a><span data-ttu-id="0deaa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0deaa-118">Request headers</span></span>
| <span data-ttu-id="0deaa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0deaa-119">Name</span></span>       | <span data-ttu-id="0deaa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0deaa-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0deaa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0deaa-121">Authorization</span></span>  | <span data-ttu-id="0deaa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0deaa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0deaa-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0deaa-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0deaa-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0deaa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0deaa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0deaa-127">Request body</span></span>
<span data-ttu-id="0deaa-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0deaa-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0deaa-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0deaa-131">Property</span></span>     | <span data-ttu-id="0deaa-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0deaa-132">Type</span></span>   |<span data-ttu-id="0deaa-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0deaa-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0deaa-134">bold</span><span class="sxs-lookup"><span data-stu-id="0deaa-134">bold</span></span>|<span data-ttu-id="0deaa-135">boolean</span><span class="sxs-lookup"><span data-stu-id="0deaa-135">boolean</span></span>|<span data-ttu-id="0deaa-136">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="0deaa-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="0deaa-137">color</span><span class="sxs-lookup"><span data-stu-id="0deaa-137">color</span></span>|<span data-ttu-id="0deaa-138">строка</span><span class="sxs-lookup"><span data-stu-id="0deaa-138">string</span></span>|<span data-ttu-id="0deaa-p105">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="0deaa-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="0deaa-142">italic</span><span class="sxs-lookup"><span data-stu-id="0deaa-142">italic</span></span>|<span data-ttu-id="0deaa-143">boolean</span><span class="sxs-lookup"><span data-stu-id="0deaa-143">boolean</span></span>|<span data-ttu-id="0deaa-144">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="0deaa-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="0deaa-145">name</span><span class="sxs-lookup"><span data-stu-id="0deaa-145">name</span></span>|<span data-ttu-id="0deaa-146">string</span><span class="sxs-lookup"><span data-stu-id="0deaa-146">string</span></span>|<span data-ttu-id="0deaa-147">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="0deaa-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="0deaa-148">size</span><span class="sxs-lookup"><span data-stu-id="0deaa-148">size</span></span>|<span data-ttu-id="0deaa-149">double</span><span class="sxs-lookup"><span data-stu-id="0deaa-149">double</span></span>|<span data-ttu-id="0deaa-150">размер шрифта</span><span class="sxs-lookup"><span data-stu-id="0deaa-150">Font size.</span></span>|
|<span data-ttu-id="0deaa-151">underline</span><span class="sxs-lookup"><span data-stu-id="0deaa-151">underline</span></span>|<span data-ttu-id="0deaa-152">string</span><span class="sxs-lookup"><span data-stu-id="0deaa-152">string</span></span>|<span data-ttu-id="0deaa-153">Тип подчеркивания, применяемый для шрифта.</span><span class="sxs-lookup"><span data-stu-id="0deaa-153">Type of underline applied to the font.</span></span> <span data-ttu-id="0deaa-154">Допустимые значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="0deaa-154">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="0deaa-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0deaa-155">Response</span></span>

<span data-ttu-id="0deaa-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжефонт](../resources/rangefont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0deaa-156">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0deaa-157">Пример</span><span class="sxs-lookup"><span data-stu-id="0deaa-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0deaa-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0deaa-158">Request</span></span>
<span data-ttu-id="0deaa-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0deaa-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0deaa-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="0deaa-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/font
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
# <a name="c"></a>[<span data-ttu-id="0deaa-161">C#</span><span class="sxs-lookup"><span data-stu-id="0deaa-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0deaa-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0deaa-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0deaa-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0deaa-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0deaa-164">Java</span><span class="sxs-lookup"><span data-stu-id="0deaa-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0deaa-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="0deaa-165">Response</span></span>
<span data-ttu-id="0deaa-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0deaa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
