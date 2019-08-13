---
title: 'workbookRangeView: range'
description: Возвращение диапазона, связанного с ресурсом rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 74a6fd086645831f2181051233b62be3bc87605c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364809"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="fa747-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="fa747-103">workbookRangeView: range</span></span>
<span data-ttu-id="fa747-104">Возвращение диапазона, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="fa747-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa747-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa747-105">Permissions</span></span>
<span data-ttu-id="fa747-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa747-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa747-108">Permission type</span></span>      | <span data-ttu-id="fa747-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa747-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa747-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa747-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa747-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa747-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa747-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa747-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa747-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa747-113">Not supported.</span></span>    |
|<span data-ttu-id="fa747-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa747-114">Application</span></span> | <span data-ttu-id="fa747-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa747-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa747-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa747-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="fa747-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa747-117">Request headers</span></span>
| <span data-ttu-id="fa747-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fa747-118">Name</span></span>       | <span data-ttu-id="fa747-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fa747-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa747-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa747-120">Authorization</span></span>  | <span data-ttu-id="fa747-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa747-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa747-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fa747-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fa747-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fa747-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa747-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa747-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="fa747-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa747-127">Response</span></span>
<span data-ttu-id="fa747-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa747-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa747-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fa747-129">Example</span></span>
<span data-ttu-id="fa747-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fa747-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa747-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa747-131">Request</span></span>
<span data-ttu-id="fa747-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa747-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa747-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa747-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa747-134">C#</span><span class="sxs-lookup"><span data-stu-id="fa747-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa747-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa747-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa747-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fa747-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa747-137">Java</span><span class="sxs-lookup"><span data-stu-id="fa747-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fa747-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa747-138">Response</span></span>
<span data-ttu-id="fa747-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa747-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
