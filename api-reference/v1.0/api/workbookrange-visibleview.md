---
title: 'workbookRange: visibleView'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 284e38d68a48bfaef395335600345cb3134080db
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278444"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="0e78e-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="0e78e-104">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="0e78e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e78e-105">Permissions</span></span>
<span data-ttu-id="0e78e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e78e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e78e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e78e-108">Permission type</span></span>      | <span data-ttu-id="0e78e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e78e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e78e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e78e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e78e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e78e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e78e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e78e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e78e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e78e-113">Not supported.</span></span>    |
|<span data-ttu-id="0e78e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e78e-114">Application</span></span> | <span data-ttu-id="0e78e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e78e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e78e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e78e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="0e78e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e78e-117">Request headers</span></span>
| <span data-ttu-id="0e78e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0e78e-118">Name</span></span>       | <span data-ttu-id="0e78e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0e78e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e78e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e78e-120">Authorization</span></span>  | <span data-ttu-id="0e78e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e78e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e78e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e78e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e78e-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0e78e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e78e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e78e-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="0e78e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e78e-127">Response</span></span>
<span data-ttu-id="0e78e-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0e78e-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e78e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0e78e-129">Example</span></span>
<span data-ttu-id="0e78e-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0e78e-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e78e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e78e-131">Request</span></span>
<span data-ttu-id="0e78e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e78e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="0e78e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e78e-133">Response</span></span>
<span data-ttu-id="0e78e-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e78e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0e78e-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0e78e-137">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e78e-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e78e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_visibleview-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="0e78e-139">C#</span><span class="sxs-lookup"><span data-stu-id="0e78e-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_visibleview-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e78e-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0e78e-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookrange_visibleview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbookrange-visibleview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbookrange-visibleview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrange-visibleview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
