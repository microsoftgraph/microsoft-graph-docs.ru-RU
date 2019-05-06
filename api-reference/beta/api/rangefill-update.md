---
title: Обновление объекта rangeFill
description: Обновление свойств объекта rangefill.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 77ab021ee00db067c6c77466abcdc2291a82460f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610925"
---
# <a name="update-rangefill"></a><span data-ttu-id="7227d-103">Обновление объекта rangeFill</span><span class="sxs-lookup"><span data-stu-id="7227d-103">Update rangefill</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7227d-104">Обновление свойств объекта rangefill.</span><span class="sxs-lookup"><span data-stu-id="7227d-104">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7227d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7227d-105">Permissions</span></span>
<span data-ttu-id="7227d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7227d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7227d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7227d-108">Permission type</span></span>      | <span data-ttu-id="7227d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7227d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7227d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7227d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7227d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7227d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7227d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7227d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7227d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7227d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7227d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7227d-114">Application</span></span> | <span data-ttu-id="7227d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7227d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7227d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7227d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="7227d-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7227d-117">Optional request headers</span></span>
| <span data-ttu-id="7227d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7227d-118">Name</span></span>       | <span data-ttu-id="7227d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7227d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7227d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7227d-120">Authorization</span></span>  | <span data-ttu-id="7227d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7227d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7227d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7227d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7227d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7227d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7227d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7227d-126">Request body</span></span>
<span data-ttu-id="7227d-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7227d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7227d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7227d-130">Property</span></span>     | <span data-ttu-id="7227d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7227d-131">Type</span></span>   |<span data-ttu-id="7227d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7227d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7227d-133">color</span><span class="sxs-lookup"><span data-stu-id="7227d-133">color</span></span>|<span data-ttu-id="7227d-134">string</span><span class="sxs-lookup"><span data-stu-id="7227d-134">string</span></span>|<span data-ttu-id="7227d-135">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="7227d-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="7227d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7227d-136">Response</span></span>

<span data-ttu-id="7227d-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжефилл](../resources/workbookrangefill.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7227d-137">If successful, this method returns a `200 OK` response code and updated [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7227d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7227d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7227d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7227d-139">Request</span></span>
<span data-ttu-id="7227d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7227d-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="7227d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7227d-141">Response</span></span>
<span data-ttu-id="7227d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7227d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7227d-145">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7227d-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7227d-146">Языках</span><span class="sxs-lookup"><span data-stu-id="7227d-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangefill-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7227d-147">Язык</span><span class="sxs-lookup"><span data-stu-id="7227d-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangefill-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangefill-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangefill-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
