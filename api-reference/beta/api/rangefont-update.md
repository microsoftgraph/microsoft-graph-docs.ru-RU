---
title: Обновление объекта rangefont
description: Обновление свойств объекта rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5857941f8c08c9090ba05098ae1d69a34dead791
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546264"
---
# <a name="update-rangefont"></a><span data-ttu-id="16d96-103">Обновление объекта rangefont</span><span class="sxs-lookup"><span data-stu-id="16d96-103">Update rangefont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16d96-104">Обновление свойств объекта rangefont.</span><span class="sxs-lookup"><span data-stu-id="16d96-104">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="16d96-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16d96-105">Permissions</span></span>
<span data-ttu-id="16d96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16d96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16d96-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16d96-108">Permission type</span></span>      | <span data-ttu-id="16d96-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16d96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16d96-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16d96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16d96-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16d96-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16d96-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16d96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16d96-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16d96-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16d96-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16d96-114">Application</span></span> | <span data-ttu-id="16d96-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16d96-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16d96-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16d96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="16d96-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16d96-117">Optional request headers</span></span>
| <span data-ttu-id="16d96-118">Имя</span><span class="sxs-lookup"><span data-stu-id="16d96-118">Name</span></span>       | <span data-ttu-id="16d96-119">Описание</span><span class="sxs-lookup"><span data-stu-id="16d96-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="16d96-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16d96-120">Authorization</span></span>  | <span data-ttu-id="16d96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16d96-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16d96-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="16d96-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="16d96-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="16d96-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16d96-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16d96-126">Request body</span></span>
<span data-ttu-id="16d96-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="16d96-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="16d96-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="16d96-130">Property</span></span>     | <span data-ttu-id="16d96-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16d96-131">Type</span></span>   |<span data-ttu-id="16d96-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16d96-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16d96-133">bold</span><span class="sxs-lookup"><span data-stu-id="16d96-133">bold</span></span>|<span data-ttu-id="16d96-134">логический</span><span class="sxs-lookup"><span data-stu-id="16d96-134">boolean</span></span>|<span data-ttu-id="16d96-135">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="16d96-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="16d96-136">color</span><span class="sxs-lookup"><span data-stu-id="16d96-136">color</span></span>|<span data-ttu-id="16d96-137">строка</span><span class="sxs-lookup"><span data-stu-id="16d96-137">string</span></span>|<span data-ttu-id="16d96-p105">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="16d96-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="16d96-141">italic</span><span class="sxs-lookup"><span data-stu-id="16d96-141">italic</span></span>|<span data-ttu-id="16d96-142">boolean</span><span class="sxs-lookup"><span data-stu-id="16d96-142">boolean</span></span>|<span data-ttu-id="16d96-143">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="16d96-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="16d96-144">name</span><span class="sxs-lookup"><span data-stu-id="16d96-144">name</span></span>|<span data-ttu-id="16d96-145">string</span><span class="sxs-lookup"><span data-stu-id="16d96-145">string</span></span>|<span data-ttu-id="16d96-146">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="16d96-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="16d96-147">size</span><span class="sxs-lookup"><span data-stu-id="16d96-147">size</span></span>|<span data-ttu-id="16d96-148">double</span><span class="sxs-lookup"><span data-stu-id="16d96-148">double</span></span>|<span data-ttu-id="16d96-149">размер шрифта</span><span class="sxs-lookup"><span data-stu-id="16d96-149">Font size.</span></span>|
|<span data-ttu-id="16d96-150">underline</span><span class="sxs-lookup"><span data-stu-id="16d96-150">underline</span></span>|<span data-ttu-id="16d96-151">string</span><span class="sxs-lookup"><span data-stu-id="16d96-151">string</span></span>|<span data-ttu-id="16d96-p106">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="16d96-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="16d96-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d96-154">Response</span></span>

<span data-ttu-id="16d96-155">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [RangeFont](../resources/rangefont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16d96-155">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16d96-156">Пример</span><span class="sxs-lookup"><span data-stu-id="16d96-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16d96-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d96-157">Request</span></span>
<span data-ttu-id="16d96-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16d96-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/font
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
##### <a name="response"></a><span data-ttu-id="16d96-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d96-159">Response</span></span>
<span data-ttu-id="16d96-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d96-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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
    "Error: /api-reference/beta/api/rangefont-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
