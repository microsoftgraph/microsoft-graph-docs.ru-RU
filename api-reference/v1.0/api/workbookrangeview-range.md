---
title: 'workbookRangeView: range'
description: Возвращение диапазона, связанного с ресурсом rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 71c2a27326d67adf25268717af5e927ac6f88570
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026314"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="320d3-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="320d3-103">workbookRangeView: range</span></span>
<span data-ttu-id="320d3-104">Возвращение диапазона, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="320d3-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="320d3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="320d3-105">Permissions</span></span>
<span data-ttu-id="320d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="320d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="320d3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="320d3-108">Permission type</span></span>      | <span data-ttu-id="320d3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="320d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="320d3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="320d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="320d3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="320d3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="320d3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="320d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="320d3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="320d3-113">Not supported.</span></span>    |
|<span data-ttu-id="320d3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="320d3-114">Application</span></span> | <span data-ttu-id="320d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="320d3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="320d3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="320d3-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="320d3-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="320d3-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="320d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="320d3-118">Request headers</span></span>
| <span data-ttu-id="320d3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="320d3-119">Name</span></span>       | <span data-ttu-id="320d3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="320d3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="320d3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="320d3-121">Authorization</span></span>  | <span data-ttu-id="320d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="320d3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="320d3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="320d3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="320d3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="320d3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="320d3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="320d3-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="320d3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="320d3-128">Response</span></span>
<span data-ttu-id="320d3-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="320d3-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="320d3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="320d3-130">Example</span></span>
<span data-ttu-id="320d3-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="320d3-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="320d3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="320d3-132">Request</span></span>
<span data-ttu-id="320d3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="320d3-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="320d3-134">C#</span><span class="sxs-lookup"><span data-stu-id="320d3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="320d3-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="320d3-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="320d3-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="320d3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="320d3-137">Java</span><span class="sxs-lookup"><span data-stu-id="320d3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="320d3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="320d3-138">Response</span></span>
<span data-ttu-id="320d3-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="320d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
