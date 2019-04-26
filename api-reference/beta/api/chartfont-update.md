---
title: Обновление Воркбукчартфонт
description: Обновление свойств объекта Воркбукчартфонт.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1228a49815419a077fd6999a400f4d720b6724f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327753"
---
# <a name="update-chartfont"></a><span data-ttu-id="60285-103">Обновление объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="60285-103">Update chartfont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60285-104">Обновление свойств объекта chartfont.</span><span class="sxs-lookup"><span data-stu-id="60285-104">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="60285-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60285-105">Permissions</span></span>
<span data-ttu-id="60285-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60285-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60285-108">Permission type</span></span>      | <span data-ttu-id="60285-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60285-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60285-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60285-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60285-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60285-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60285-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60285-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60285-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60285-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60285-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60285-114">Application</span></span> | <span data-ttu-id="60285-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60285-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60285-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60285-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="60285-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60285-117">Optional request headers</span></span>
| <span data-ttu-id="60285-118">Имя</span><span class="sxs-lookup"><span data-stu-id="60285-118">Name</span></span>       | <span data-ttu-id="60285-119">Описание</span><span class="sxs-lookup"><span data-stu-id="60285-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="60285-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60285-120">Authorization</span></span>  | <span data-ttu-id="60285-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60285-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60285-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="60285-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="60285-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="60285-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60285-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="60285-126">Request body</span></span>
<span data-ttu-id="60285-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="60285-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60285-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="60285-130">Property</span></span>     | <span data-ttu-id="60285-131">Тип</span><span class="sxs-lookup"><span data-stu-id="60285-131">Type</span></span>   |<span data-ttu-id="60285-132">Описание</span><span class="sxs-lookup"><span data-stu-id="60285-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60285-133">bold</span><span class="sxs-lookup"><span data-stu-id="60285-133">bold</span></span>|<span data-ttu-id="60285-134">boolean</span><span class="sxs-lookup"><span data-stu-id="60285-134">boolean</span></span>|<span data-ttu-id="60285-135">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="60285-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="60285-136">color</span><span class="sxs-lookup"><span data-stu-id="60285-136">color</span></span>|<span data-ttu-id="60285-137">строка</span><span class="sxs-lookup"><span data-stu-id="60285-137">string</span></span>|<span data-ttu-id="60285-p105">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="60285-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="60285-141">italic</span><span class="sxs-lookup"><span data-stu-id="60285-141">italic</span></span>|<span data-ttu-id="60285-142">boolean</span><span class="sxs-lookup"><span data-stu-id="60285-142">boolean</span></span>|<span data-ttu-id="60285-143">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="60285-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="60285-144">name</span><span class="sxs-lookup"><span data-stu-id="60285-144">name</span></span>|<span data-ttu-id="60285-145">string</span><span class="sxs-lookup"><span data-stu-id="60285-145">string</span></span>|<span data-ttu-id="60285-146">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="60285-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="60285-147">size</span><span class="sxs-lookup"><span data-stu-id="60285-147">size</span></span>|<span data-ttu-id="60285-148">Double</span><span class="sxs-lookup"><span data-stu-id="60285-148">double</span></span>|<span data-ttu-id="60285-149">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="60285-149">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="60285-150">underline</span><span class="sxs-lookup"><span data-stu-id="60285-150">underline</span></span>|<span data-ttu-id="60285-151">string</span><span class="sxs-lookup"><span data-stu-id="60285-151">string</span></span>|<span data-ttu-id="60285-p106">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="60285-p106">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="60285-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="60285-154">Response</span></span>

<span data-ttu-id="60285-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартфонт](../resources/workbookchartfont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60285-155">If successful, this method returns a `200 OK` response code and updated [workbookChartFont](../resources/workbookchartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60285-156">Пример</span><span class="sxs-lookup"><span data-stu-id="60285-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60285-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="60285-157">Request</span></span>
<span data-ttu-id="60285-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60285-158">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="60285-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="60285-159">Response</span></span>
<span data-ttu-id="60285-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60285-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
