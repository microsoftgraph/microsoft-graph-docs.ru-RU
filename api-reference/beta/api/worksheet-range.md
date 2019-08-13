---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ff7576ecd9d09c3387b9efa1bf9a4cc88e8691f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358122"
---
# <a name="worksheet-range"></a><span data-ttu-id="4cc5d-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="4cc5d-103">Worksheet: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cc5d-104">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cc5d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cc5d-105">Permissions</span></span>
<span data-ttu-id="4cc5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cc5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cc5d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cc5d-108">Permission type</span></span>      | <span data-ttu-id="4cc5d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cc5d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cc5d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cc5d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4cc5d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cc5d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4cc5d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cc5d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cc5d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cc5d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4cc5d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cc5d-114">Application</span></span> | <span data-ttu-id="4cc5d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cc5d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cc5d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="4cc5d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cc5d-117">Request headers</span></span>
| <span data-ttu-id="4cc5d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4cc5d-118">Name</span></span>       | <span data-ttu-id="4cc5d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4cc5d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4cc5d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cc5d-120">Authorization</span></span>  | <span data-ttu-id="4cc5d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cc5d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4cc5d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4cc5d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cc5d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cc5d-126">Request body</span></span>
<span data-ttu-id="4cc5d-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4cc5d-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="4cc5d-128">Parameter</span></span>    | <span data-ttu-id="4cc5d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4cc5d-129">Type</span></span>   |<span data-ttu-id="4cc5d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4cc5d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cc5d-131">address</span><span class="sxs-lookup"><span data-stu-id="4cc5d-131">address</span></span>|<span data-ttu-id="4cc5d-132">string</span><span class="sxs-lookup"><span data-stu-id="4cc5d-132">string</span></span>|<span data-ttu-id="4cc5d-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="4cc5d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cc5d-136">Response</span></span>

<span data-ttu-id="4cc5d-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cc5d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4cc5d-138">Example</span></span>
<span data-ttu-id="4cc5d-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4cc5d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cc5d-140">Request</span></span>
<span data-ttu-id="4cc5d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4cc5d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cc5d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4cc5d-143">C#</span><span class="sxs-lookup"><span data-stu-id="4cc5d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4cc5d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cc5d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4cc5d-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4cc5d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4cc5d-146">Java</span><span class="sxs-lookup"><span data-stu-id="4cc5d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4cc5d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cc5d-147">Response</span></span>
<span data-ttu-id="4cc5d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cc5d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
