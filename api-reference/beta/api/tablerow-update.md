---
title: Обновление объекта tableRow
description: Обновление свойств объекта tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cf03055177048b2389ee82ccc2c3dc7ac79045bc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270835"
---
# <a name="update-tablerow"></a><span data-ttu-id="fbc73-103">Обновление объекта tableRow</span><span class="sxs-lookup"><span data-stu-id="fbc73-103">Update tablerow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbc73-104">Обновление свойств объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="fbc73-104">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fbc73-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbc73-105">Permissions</span></span>
<span data-ttu-id="fbc73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbc73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbc73-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbc73-108">Permission type</span></span>      | <span data-ttu-id="fbc73-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbc73-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbc73-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbc73-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fbc73-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbc73-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fbc73-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbc73-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbc73-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbc73-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fbc73-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbc73-114">Application</span></span> | <span data-ttu-id="fbc73-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbc73-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbc73-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbc73-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows/{index}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-request-headers"></a><span data-ttu-id="fbc73-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbc73-117">Optional request headers</span></span>
| <span data-ttu-id="fbc73-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fbc73-118">Name</span></span>       | <span data-ttu-id="fbc73-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fbc73-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fbc73-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbc73-120">Authorization</span></span>  | <span data-ttu-id="fbc73-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbc73-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fbc73-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fbc73-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fbc73-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fbc73-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbc73-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fbc73-126">Request body</span></span>
<span data-ttu-id="fbc73-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fbc73-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fbc73-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbc73-130">Property</span></span>     | <span data-ttu-id="fbc73-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fbc73-131">Type</span></span>   |<span data-ttu-id="fbc73-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fbc73-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbc73-133">values</span><span class="sxs-lookup"><span data-stu-id="fbc73-133">values</span></span>|<span data-ttu-id="fbc73-134">Json</span><span class="sxs-lookup"><span data-stu-id="fbc73-134">Json</span></span>|<span data-ttu-id="fbc73-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="fbc73-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="fbc73-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbc73-138">Response</span></span>

<span data-ttu-id="fbc73-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбуктаблеров](../resources/workbooktablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fbc73-139">If successful, this method returns a `200 OK` response code and updated [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fbc73-140">Пример</span><span class="sxs-lookup"><span data-stu-id="fbc73-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbc73-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbc73-141">Request</span></span>
<span data-ttu-id="fbc73-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbc73-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="fbc73-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbc73-143">Response</span></span>
<span data-ttu-id="fbc73-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbc73-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fbc73-147">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fbc73-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fbc73-148">C#</span><span class="sxs-lookup"><span data-stu-id="fbc73-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_tablerow-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbc73-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="fbc73-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_tablerow-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fbc73-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fbc73-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_tablerow-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablerow-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tablerow-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablerow-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
