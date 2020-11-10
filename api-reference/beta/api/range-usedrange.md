---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1af9f26d34ae2aefeda102d00967433f3b74626d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981938"
---
# <a name="range-usedrange"></a><span data-ttu-id="38515-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="38515-103">Range: UsedRange</span></span>

<span data-ttu-id="38515-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38515-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38515-105">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="38515-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="38515-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38515-106">Permissions</span></span>
<span data-ttu-id="38515-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38515-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38515-109">Permission type</span></span>      | <span data-ttu-id="38515-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38515-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38515-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38515-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38515-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38515-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="38515-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38515-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38515-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38515-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="38515-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38515-115">Application</span></span> | <span data-ttu-id="38515-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38515-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38515-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38515-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="38515-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38515-118">Request headers</span></span>
| <span data-ttu-id="38515-119">Имя</span><span class="sxs-lookup"><span data-stu-id="38515-119">Name</span></span>       | <span data-ttu-id="38515-120">Описание</span><span class="sxs-lookup"><span data-stu-id="38515-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="38515-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38515-121">Authorization</span></span>  | <span data-ttu-id="38515-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38515-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38515-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="38515-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="38515-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="38515-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38515-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38515-127">Request body</span></span>
<span data-ttu-id="38515-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="38515-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="38515-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="38515-129">Parameter</span></span>    | <span data-ttu-id="38515-130">Тип</span><span class="sxs-lookup"><span data-stu-id="38515-130">Type</span></span>   |<span data-ttu-id="38515-131">Описание</span><span class="sxs-lookup"><span data-stu-id="38515-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38515-132">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="38515-132">valuesOnly</span></span>|<span data-ttu-id="38515-133">boolean</span><span class="sxs-lookup"><span data-stu-id="38515-133">boolean</span></span>|<span data-ttu-id="38515-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="38515-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="38515-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="38515-136">Response</span></span>

<span data-ttu-id="38515-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="38515-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38515-138">Пример</span><span class="sxs-lookup"><span data-stu-id="38515-138">Example</span></span>
<span data-ttu-id="38515-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="38515-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38515-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="38515-140">Request</span></span>
<span data-ttu-id="38515-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38515-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38515-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="38515-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="38515-143">C#</span><span class="sxs-lookup"><span data-stu-id="38515-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38515-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38515-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38515-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38515-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38515-146">Java</span><span class="sxs-lookup"><span data-stu-id="38515-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="38515-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="38515-147">Response</span></span>
<span data-ttu-id="38515-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38515-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


