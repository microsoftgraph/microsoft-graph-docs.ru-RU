---
title: Получение списка строк rangeView
description: Получение списка, который включает в себя объекты видимых ячеек в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e12a5fc81cb5176acb7141b17a1722ff24d68aae
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278430"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="86439-103">Получение списка строк rangeView</span><span class="sxs-lookup"><span data-stu-id="86439-103">List rangeView rows</span></span>

<span data-ttu-id="86439-104">Получение списка, который включает в себя объекты видимых ячеек в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="86439-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="86439-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86439-105">Permissions</span></span>
<span data-ttu-id="86439-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86439-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86439-108">Permission type</span></span>      | <span data-ttu-id="86439-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86439-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86439-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86439-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86439-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86439-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="86439-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86439-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86439-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86439-113">Not supported.</span></span>    |
|<span data-ttu-id="86439-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86439-114">Application</span></span> | <span data-ttu-id="86439-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86439-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86439-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86439-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="86439-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="86439-117">Optional query parameters</span></span>
<span data-ttu-id="86439-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="86439-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86439-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86439-119">Request headers</span></span>
| <span data-ttu-id="86439-120">Имя</span><span class="sxs-lookup"><span data-stu-id="86439-120">Name</span></span>      |<span data-ttu-id="86439-121">Описание</span><span class="sxs-lookup"><span data-stu-id="86439-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86439-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86439-122">Authorization</span></span>  | <span data-ttu-id="86439-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86439-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86439-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="86439-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="86439-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="86439-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86439-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86439-128">Request body</span></span>
<span data-ttu-id="86439-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86439-129">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="86439-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="86439-130">Response</span></span>
<span data-ttu-id="86439-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="86439-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86439-132">Пример</span><span class="sxs-lookup"><span data-stu-id="86439-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86439-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="86439-133">Request</span></span>
<span data-ttu-id="86439-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86439-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows
```
##### <a name="response"></a><span data-ttu-id="86439-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="86439-135">Response</span></span>
<span data-ttu-id="86439-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86439-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="86439-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="86439-139">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86439-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="86439-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_rows-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="86439-141">C#</span><span class="sxs-lookup"><span data-stu-id="86439-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_rows-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="86439-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="86439-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_rows-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/workbookrangeview-list-rows.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbookrangeview-list-rows.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrangeview-list-rows.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
