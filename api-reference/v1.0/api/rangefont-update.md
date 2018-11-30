---
title: Обновление объекта rangefont
description: Обновление свойств объекта rangefont.
ms.openlocfilehash: a70efe8c2ff3a6cf3b92061e17a3ec0b1637945d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025444"
---
# <a name="update-rangefont"></a><span data-ttu-id="57561-103">Обновление объекта rangefont</span><span class="sxs-lookup"><span data-stu-id="57561-103">Update rangefont</span></span>

<span data-ttu-id="57561-104">Обновление свойств объекта rangefont.</span><span class="sxs-lookup"><span data-stu-id="57561-104">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="57561-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57561-105">Permissions</span></span>
<span data-ttu-id="57561-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57561-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57561-108">Permission type</span></span>      | <span data-ttu-id="57561-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57561-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57561-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57561-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57561-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57561-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57561-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57561-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57561-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57561-113">Not supported.</span></span>    |
|<span data-ttu-id="57561-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57561-114">Application</span></span> | <span data-ttu-id="57561-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57561-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57561-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57561-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="request-headers"></a><span data-ttu-id="57561-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57561-117">Request headers</span></span>
| <span data-ttu-id="57561-118">Имя</span><span class="sxs-lookup"><span data-stu-id="57561-118">Name</span></span>       | <span data-ttu-id="57561-119">Описание</span><span class="sxs-lookup"><span data-stu-id="57561-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="57561-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57561-120">Authorization</span></span>  | <span data-ttu-id="57561-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57561-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57561-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="57561-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="57561-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="57561-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57561-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57561-126">Request body</span></span>
<span data-ttu-id="57561-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="57561-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="57561-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="57561-130">Property</span></span>     | <span data-ttu-id="57561-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57561-131">Type</span></span>   |<span data-ttu-id="57561-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57561-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57561-133">bold</span><span class="sxs-lookup"><span data-stu-id="57561-133">bold</span></span>|<span data-ttu-id="57561-134">boolean</span><span class="sxs-lookup"><span data-stu-id="57561-134">boolean</span></span>|<span data-ttu-id="57561-135">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="57561-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="57561-136">color</span><span class="sxs-lookup"><span data-stu-id="57561-136">color</span></span>|<span data-ttu-id="57561-137">строка</span><span class="sxs-lookup"><span data-stu-id="57561-137">string</span></span>|<span data-ttu-id="57561-p105">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="57561-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="57561-141">italic</span><span class="sxs-lookup"><span data-stu-id="57561-141">italic</span></span>|<span data-ttu-id="57561-142">boolean</span><span class="sxs-lookup"><span data-stu-id="57561-142">boolean</span></span>|<span data-ttu-id="57561-143">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="57561-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="57561-144">name</span><span class="sxs-lookup"><span data-stu-id="57561-144">name</span></span>|<span data-ttu-id="57561-145">строка</span><span class="sxs-lookup"><span data-stu-id="57561-145">string</span></span>|<span data-ttu-id="57561-146">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="57561-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="57561-147">size</span><span class="sxs-lookup"><span data-stu-id="57561-147">size</span></span>|<span data-ttu-id="57561-148">double</span><span class="sxs-lookup"><span data-stu-id="57561-148">double</span></span>|<span data-ttu-id="57561-149">font-size</span><span class="sxs-lookup"><span data-stu-id="57561-149">Font size.</span></span>|
|<span data-ttu-id="57561-150">underline</span><span class="sxs-lookup"><span data-stu-id="57561-150">underline</span></span>|<span data-ttu-id="57561-151">строка</span><span class="sxs-lookup"><span data-stu-id="57561-151">string</span></span>|<span data-ttu-id="57561-152">Тип подчеркивание шрифта.</span><span class="sxs-lookup"><span data-stu-id="57561-152">Type of underline applied to the font.</span></span> <span data-ttu-id="57561-153">Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="57561-153">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="57561-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="57561-154">Response</span></span>

<span data-ttu-id="57561-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookRangeFont](../resources/rangefont.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="57561-155">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57561-156">Пример</span><span class="sxs-lookup"><span data-stu-id="57561-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57561-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="57561-157">Request</span></span>
<span data-ttu-id="57561-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57561-158">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="57561-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="57561-159">Response</span></span>
<span data-ttu-id="57561-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="57561-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->