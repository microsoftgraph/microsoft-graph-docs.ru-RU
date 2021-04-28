---
title: 'workbookRangeView: range'
description: Возвращение диапазона, связанного с ресурсом rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 225d57611fc95abf7fc305294f41e36dbb58f251
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049361"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="ebbeb-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="ebbeb-103">workbookRangeView: range</span></span>

<span data-ttu-id="ebbeb-104">Пространство имен: microsoft.graph Возвращает диапазон, связанный с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-104">Namespace: microsoft.graph Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebbeb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebbeb-105">Permissions</span></span>
<span data-ttu-id="ebbeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebbeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ebbeb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebbeb-108">Permission type</span></span>      | <span data-ttu-id="ebbeb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebbeb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebbeb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebbeb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ebbeb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebbeb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebbeb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebbeb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebbeb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-113">Not supported.</span></span>    |
|<span data-ttu-id="ebbeb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebbeb-114">Application</span></span> | <span data-ttu-id="ebbeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebbeb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebbeb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="ebbeb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebbeb-117">Request headers</span></span>
| <span data-ttu-id="ebbeb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ebbeb-118">Name</span></span>       | <span data-ttu-id="ebbeb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ebbeb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ebbeb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebbeb-120">Authorization</span></span>  | <span data-ttu-id="ebbeb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebbeb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ebbeb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebbeb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebbeb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebbeb-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="ebbeb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebbeb-127">Response</span></span>
<span data-ttu-id="ebbeb-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebbeb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ebbeb-129">Example</span></span>
<span data-ttu-id="ebbeb-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ebbeb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebbeb-131">Request</span></span>
<span data-ttu-id="ebbeb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebbeb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebbeb-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="c"></a>[<span data-ttu-id="ebbeb-134">C#</span><span class="sxs-lookup"><span data-stu-id="ebbeb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebbeb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebbeb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebbeb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebbeb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebbeb-137">Java</span><span class="sxs-lookup"><span data-stu-id="ebbeb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ebbeb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebbeb-138">Response</span></span>
<span data-ttu-id="ebbeb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-139">Here is an example of the response.</span></span> <span data-ttu-id="ebbeb-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ebbeb-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

