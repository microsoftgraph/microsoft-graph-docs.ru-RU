---
title: Обновление объекта tableRow
description: Обновление свойств объекта tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d7a982aa54ffb26888f827317aaadaa6a4be6e5f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409459"
---
# <a name="update-tablerow"></a><span data-ttu-id="85868-103">Обновление объекта tableRow</span><span class="sxs-lookup"><span data-stu-id="85868-103">Update tablerow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85868-104">Обновление свойств объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="85868-104">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="85868-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85868-105">Permissions</span></span>
<span data-ttu-id="85868-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85868-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85868-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85868-108">Permission type</span></span>      | <span data-ttu-id="85868-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85868-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85868-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85868-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85868-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85868-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85868-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85868-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85868-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85868-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85868-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85868-114">Application</span></span> | <span data-ttu-id="85868-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85868-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85868-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85868-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows/{index}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-request-headers"></a><span data-ttu-id="85868-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85868-117">Optional request headers</span></span>
| <span data-ttu-id="85868-118">Имя</span><span class="sxs-lookup"><span data-stu-id="85868-118">Name</span></span>       | <span data-ttu-id="85868-119">Описание</span><span class="sxs-lookup"><span data-stu-id="85868-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="85868-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85868-120">Authorization</span></span>  | <span data-ttu-id="85868-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85868-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85868-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="85868-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="85868-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="85868-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85868-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85868-126">Request body</span></span>
<span data-ttu-id="85868-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="85868-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="85868-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85868-130">Property</span></span>     | <span data-ttu-id="85868-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85868-131">Type</span></span>   |<span data-ttu-id="85868-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85868-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85868-133">values</span><span class="sxs-lookup"><span data-stu-id="85868-133">values</span></span>|<span data-ttu-id="85868-134">Json</span><span class="sxs-lookup"><span data-stu-id="85868-134">Json</span></span>|<span data-ttu-id="85868-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="85868-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="85868-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="85868-138">Response</span></span>

<span data-ttu-id="85868-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбуктаблеров](../resources/workbooktablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85868-139">If successful, this method returns a `200 OK` response code and updated [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85868-140">Пример</span><span class="sxs-lookup"><span data-stu-id="85868-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85868-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="85868-141">Request</span></span>
<span data-ttu-id="85868-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85868-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="85868-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="85868-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="85868-144">C#</span><span class="sxs-lookup"><span data-stu-id="85868-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85868-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85868-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="85868-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="85868-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85868-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="85868-147">Response</span></span>
<span data-ttu-id="85868-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85868-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
