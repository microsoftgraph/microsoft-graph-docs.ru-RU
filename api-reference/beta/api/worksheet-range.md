---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bacde9f1157533fc749fc6031b771f4973a307d0
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578185"
---
# <a name="worksheet-range"></a><span data-ttu-id="781bd-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="781bd-103">Worksheet: Range</span></span>

<span data-ttu-id="781bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="781bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="781bd-105">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="781bd-105">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="781bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="781bd-106">Permissions</span></span>
<span data-ttu-id="781bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="781bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="781bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="781bd-109">Permission type</span></span>      | <span data-ttu-id="781bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="781bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="781bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="781bd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="781bd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="781bd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="781bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="781bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="781bd-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="781bd-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="781bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="781bd-115">Application</span></span> | <span data-ttu-id="781bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="781bd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="781bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="781bd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="781bd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="781bd-118">Request headers</span></span>
| <span data-ttu-id="781bd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="781bd-119">Name</span></span>       | <span data-ttu-id="781bd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="781bd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="781bd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="781bd-121">Authorization</span></span>  | <span data-ttu-id="781bd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="781bd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="781bd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="781bd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="781bd-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="781bd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="781bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="781bd-127">Request body</span></span>
<span data-ttu-id="781bd-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="781bd-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="781bd-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="781bd-129">Parameter</span></span>    | <span data-ttu-id="781bd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="781bd-130">Type</span></span>   |<span data-ttu-id="781bd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="781bd-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="781bd-132">address</span><span class="sxs-lookup"><span data-stu-id="781bd-132">address</span></span>|<span data-ttu-id="781bd-133">string</span><span class="sxs-lookup"><span data-stu-id="781bd-133">string</span></span>|<span data-ttu-id="781bd-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="781bd-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="781bd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="781bd-137">Response</span></span>

<span data-ttu-id="781bd-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="781bd-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="781bd-139">Пример</span><span class="sxs-lookup"><span data-stu-id="781bd-139">Example</span></span>
<span data-ttu-id="781bd-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="781bd-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="781bd-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="781bd-141">Request</span></span>
<span data-ttu-id="781bd-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="781bd-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="781bd-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="781bd-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```
# <a name="c"></a>[<span data-ttu-id="781bd-144">C#</span><span class="sxs-lookup"><span data-stu-id="781bd-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="781bd-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="781bd-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="781bd-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="781bd-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="781bd-147">Java</span><span class="sxs-lookup"><span data-stu-id="781bd-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="781bd-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="781bd-148">Response</span></span>
<span data-ttu-id="781bd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="781bd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


