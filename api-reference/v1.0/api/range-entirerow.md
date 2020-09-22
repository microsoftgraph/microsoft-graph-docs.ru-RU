---
title: 'Range: EntireRow'
description: Возвращает объект, представляющий всю строку диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cd12a5b650fadcc87db98bf0f860d34ec0fc9ad7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978729"
---
# <a name="range-entirerow"></a><span data-ttu-id="2b098-103">Range: EntireRow</span><span class="sxs-lookup"><span data-stu-id="2b098-103">Range: EntireRow</span></span>

<span data-ttu-id="2b098-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b098-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b098-105">Возвращает объект, представляющий всю строку диапазона.</span><span class="sxs-lookup"><span data-stu-id="2b098-105">Gets an object that represents the entire row of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b098-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b098-106">Permissions</span></span>
<span data-ttu-id="2b098-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b098-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b098-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b098-109">Permission type</span></span>      | <span data-ttu-id="2b098-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b098-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b098-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b098-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b098-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b098-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2b098-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b098-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b098-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b098-114">Not supported.</span></span>    |
|<span data-ttu-id="2b098-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b098-115">Application</span></span> | <span data-ttu-id="2b098-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b098-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b098-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b098-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/entireRow
GET /workbook/worksheets/{id|name}/range(address='<address>'/entireRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/entireRow

```
## <a name="request-headers"></a><span data-ttu-id="2b098-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b098-118">Request headers</span></span>
| <span data-ttu-id="2b098-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2b098-119">Name</span></span>       | <span data-ttu-id="2b098-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2b098-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2b098-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b098-121">Authorization</span></span>  | <span data-ttu-id="2b098-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b098-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b098-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2b098-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="2b098-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2b098-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b098-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b098-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2b098-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b098-128">Response</span></span>

<span data-ttu-id="2b098-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b098-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b098-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2b098-130">Example</span></span>
<span data-ttu-id="2b098-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2b098-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2b098-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b098-132">Request</span></span>
<span data-ttu-id="2b098-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b098-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b098-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b098-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirerow"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireRow
```
# <a name="c"></a>[<span data-ttu-id="2b098-135">C#</span><span class="sxs-lookup"><span data-stu-id="2b098-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-entirerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b098-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b098-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-entirerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b098-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b098-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-entirerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b098-138">Java</span><span class="sxs-lookup"><span data-stu-id="2b098-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-entirerow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2b098-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b098-139">Response</span></span>
<span data-ttu-id="2b098-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b098-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: EntireRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

