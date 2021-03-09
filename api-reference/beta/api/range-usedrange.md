---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e22ca741dfd74554b4da3810eb41bffc8a487563
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578845"
---
# <a name="range-usedrange"></a><span data-ttu-id="c4ed1-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="c4ed1-103">Range: UsedRange</span></span>

<span data-ttu-id="c4ed1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4ed1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4ed1-105">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4ed1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ed1-106">Permissions</span></span>
<span data-ttu-id="c4ed1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4ed1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ed1-109">Permission type</span></span>      | <span data-ttu-id="c4ed1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4ed1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4ed1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4ed1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4ed1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4ed1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4ed1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4ed1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4ed1-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4ed1-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4ed1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4ed1-115">Application</span></span> | <span data-ttu-id="c4ed1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4ed1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4ed1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/UsedRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/UsedRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/UsedRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="c4ed1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4ed1-118">Request headers</span></span>
| <span data-ttu-id="c4ed1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4ed1-119">Name</span></span>       | <span data-ttu-id="c4ed1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4ed1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4ed1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4ed1-121">Authorization</span></span>  | <span data-ttu-id="c4ed1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4ed1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4ed1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4ed1-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4ed1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4ed1-127">Request body</span></span>
<span data-ttu-id="c4ed1-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4ed1-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4ed1-129">Parameter</span></span>    | <span data-ttu-id="c4ed1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c4ed1-130">Type</span></span>   |<span data-ttu-id="c4ed1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c4ed1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4ed1-132">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="c4ed1-132">valuesOnly</span></span>|<span data-ttu-id="c4ed1-133">boolean</span><span class="sxs-lookup"><span data-stu-id="c4ed1-133">boolean</span></span>|<span data-ttu-id="c4ed1-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="c4ed1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ed1-136">Response</span></span>

<span data-ttu-id="c4ed1-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4ed1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c4ed1-138">Example</span></span>
<span data-ttu-id="c4ed1-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4ed1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4ed1-140">Request</span></span>
<span data-ttu-id="c4ed1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4ed1-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ed1-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c4ed1-143">C#</span><span class="sxs-lookup"><span data-stu-id="c4ed1-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4ed1-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4ed1-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4ed1-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4ed1-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4ed1-146">Java</span><span class="sxs-lookup"><span data-stu-id="c4ed1-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4ed1-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ed1-147">Response</span></span>
<span data-ttu-id="c4ed1-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


