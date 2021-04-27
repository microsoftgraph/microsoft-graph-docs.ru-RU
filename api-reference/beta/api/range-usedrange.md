---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d705c89ca70616a57209bf788e43c433c6f8ee61
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055052"
---
# <a name="range-usedrange"></a><span data-ttu-id="4194e-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="4194e-103">Range: UsedRange</span></span>

<span data-ttu-id="4194e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4194e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4194e-105">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="4194e-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4194e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4194e-106">Permissions</span></span>
<span data-ttu-id="4194e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4194e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4194e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4194e-109">Permission type</span></span>      | <span data-ttu-id="4194e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4194e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4194e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4194e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4194e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4194e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4194e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4194e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4194e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4194e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4194e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4194e-115">Application</span></span> | <span data-ttu-id="4194e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4194e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4194e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4194e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/UsedRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/UsedRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/UsedRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="4194e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4194e-118">Request headers</span></span>
| <span data-ttu-id="4194e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4194e-119">Name</span></span>       | <span data-ttu-id="4194e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4194e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4194e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4194e-121">Authorization</span></span>  | <span data-ttu-id="4194e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4194e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4194e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4194e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4194e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4194e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4194e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4194e-127">Request body</span></span>
<span data-ttu-id="4194e-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4194e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4194e-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="4194e-129">Parameter</span></span>    | <span data-ttu-id="4194e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4194e-130">Type</span></span>   |<span data-ttu-id="4194e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4194e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4194e-132">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="4194e-132">valuesOnly</span></span>|<span data-ttu-id="4194e-133">boolean</span><span class="sxs-lookup"><span data-stu-id="4194e-133">boolean</span></span>|<span data-ttu-id="4194e-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="4194e-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="4194e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4194e-136">Response</span></span>

<span data-ttu-id="4194e-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4194e-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4194e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4194e-138">Example</span></span>
<span data-ttu-id="4194e-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4194e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4194e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4194e-140">Request</span></span>
<span data-ttu-id="4194e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4194e-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4194e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4194e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="4194e-143">C#</span><span class="sxs-lookup"><span data-stu-id="4194e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4194e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4194e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4194e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4194e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4194e-146">Java</span><span class="sxs-lookup"><span data-stu-id="4194e-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4194e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4194e-147">Response</span></span>
<span data-ttu-id="4194e-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4194e-148">Here is an example of the response.</span></span> <span data-ttu-id="4194e-149">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4194e-149">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


