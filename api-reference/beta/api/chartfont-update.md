---
title: Обновление объекта ChartFont
description: Обновление свойств объекта chartfont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 729c5e20fef7c4c2c411cfede3a28e512286457c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971496"
---
# <a name="update-chartfont"></a><span data-ttu-id="64f1a-103">Обновление объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="64f1a-103">Update chartfont</span></span>

> <span data-ttu-id="64f1a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64f1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64f1a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64f1a-106">Обновление свойств объекта chartfont.</span><span class="sxs-lookup"><span data-stu-id="64f1a-106">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="64f1a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64f1a-107">Permissions</span></span>
<span data-ttu-id="64f1a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64f1a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64f1a-110">Permission type</span></span>      | <span data-ttu-id="64f1a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64f1a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64f1a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64f1a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="64f1a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64f1a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64f1a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64f1a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64f1a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64f1a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64f1a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64f1a-116">Application</span></span> | <span data-ttu-id="64f1a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f1a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64f1a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64f1a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="64f1a-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64f1a-119">Optional request headers</span></span>
| <span data-ttu-id="64f1a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="64f1a-120">Name</span></span>       | <span data-ttu-id="64f1a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="64f1a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="64f1a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64f1a-122">Authorization</span></span>  | <span data-ttu-id="64f1a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64f1a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64f1a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="64f1a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="64f1a-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="64f1a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f1a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64f1a-128">Request body</span></span>
<span data-ttu-id="64f1a-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="64f1a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="64f1a-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="64f1a-132">Property</span></span>     | <span data-ttu-id="64f1a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="64f1a-133">Type</span></span>   |<span data-ttu-id="64f1a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="64f1a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64f1a-135">bold</span><span class="sxs-lookup"><span data-stu-id="64f1a-135">bold</span></span>|<span data-ttu-id="64f1a-136">boolean</span><span class="sxs-lookup"><span data-stu-id="64f1a-136">boolean</span></span>|<span data-ttu-id="64f1a-137">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="64f1a-137">Represents the bold status of font.</span></span>|
|<span data-ttu-id="64f1a-138">color</span><span class="sxs-lookup"><span data-stu-id="64f1a-138">color</span></span>|<span data-ttu-id="64f1a-139">строка</span><span class="sxs-lookup"><span data-stu-id="64f1a-139">string</span></span>|<span data-ttu-id="64f1a-p106">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="64f1a-p106">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="64f1a-143">italic</span><span class="sxs-lookup"><span data-stu-id="64f1a-143">italic</span></span>|<span data-ttu-id="64f1a-144">boolean</span><span class="sxs-lookup"><span data-stu-id="64f1a-144">boolean</span></span>|<span data-ttu-id="64f1a-145">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="64f1a-145">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="64f1a-146">name</span><span class="sxs-lookup"><span data-stu-id="64f1a-146">name</span></span>|<span data-ttu-id="64f1a-147">строка</span><span class="sxs-lookup"><span data-stu-id="64f1a-147">string</span></span>|<span data-ttu-id="64f1a-148">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="64f1a-148">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="64f1a-149">size</span><span class="sxs-lookup"><span data-stu-id="64f1a-149">size</span></span>|<span data-ttu-id="64f1a-150">Double</span><span class="sxs-lookup"><span data-stu-id="64f1a-150">double</span></span>|<span data-ttu-id="64f1a-151">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="64f1a-151">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="64f1a-152">underline</span><span class="sxs-lookup"><span data-stu-id="64f1a-152">underline</span></span>|<span data-ttu-id="64f1a-153">строка</span><span class="sxs-lookup"><span data-stu-id="64f1a-153">string</span></span>|<span data-ttu-id="64f1a-p107">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="64f1a-p107">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="64f1a-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f1a-156">Response</span></span>

<span data-ttu-id="64f1a-157">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartFont](../resources/chartfont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64f1a-157">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64f1a-158">Пример</span><span class="sxs-lookup"><span data-stu-id="64f1a-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64f1a-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="64f1a-159">Request</span></span>
<span data-ttu-id="64f1a-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64f1a-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
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
##### <a name="response"></a><span data-ttu-id="64f1a-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="64f1a-161">Response</span></span>
<span data-ttu-id="64f1a-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="64f1a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
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
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
