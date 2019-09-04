---
title: 'workbookRangeView: range'
description: Возвращение диапазона, связанного с ресурсом rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b01f354cc0ce909108a085a61d200c0517e724c0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727336"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="b1007-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="b1007-103">workbookRangeView: range</span></span>
<span data-ttu-id="b1007-104">Возвращение диапазона, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="b1007-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1007-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1007-105">Permissions</span></span>
<span data-ttu-id="b1007-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b1007-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1007-108">Permission type</span></span>      | <span data-ttu-id="b1007-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1007-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1007-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1007-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1007-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1007-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b1007-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1007-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1007-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1007-113">Not supported.</span></span>    |
|<span data-ttu-id="b1007-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1007-114">Application</span></span> | <span data-ttu-id="b1007-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1007-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1007-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1007-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="b1007-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1007-117">Request headers</span></span>
| <span data-ttu-id="b1007-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b1007-118">Name</span></span>       | <span data-ttu-id="b1007-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b1007-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b1007-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1007-120">Authorization</span></span>  | <span data-ttu-id="b1007-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1007-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1007-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b1007-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b1007-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b1007-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1007-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1007-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="b1007-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1007-127">Response</span></span>
<span data-ttu-id="b1007-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1007-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1007-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b1007-129">Example</span></span>
<span data-ttu-id="b1007-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b1007-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b1007-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1007-131">Request</span></span>
<span data-ttu-id="b1007-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1007-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b1007-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1007-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1007-134">C#</span><span class="sxs-lookup"><span data-stu-id="b1007-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1007-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1007-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1007-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b1007-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1007-137">Java</span><span class="sxs-lookup"><span data-stu-id="b1007-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b1007-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1007-138">Response</span></span>
<span data-ttu-id="b1007-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1007-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
