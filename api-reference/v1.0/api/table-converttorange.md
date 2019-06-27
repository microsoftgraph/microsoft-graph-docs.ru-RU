---
title: 'Table: convertToRange'
description: Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c1b01d165e4ccb78e3a2b2fcd4b75bf16cd7b535
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273124"
---
# <a name="table-converttorange"></a><span data-ttu-id="3e3ad-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="3e3ad-104">Table: convertToRange</span></span>

<span data-ttu-id="3e3ad-p102">Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e3ad-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e3ad-107">Permissions</span></span>
<span data-ttu-id="3e3ad-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e3ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e3ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e3ad-110">Permission type</span></span>      | <span data-ttu-id="3e3ad-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e3ad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e3ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e3ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e3ad-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e3ad-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e3ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e3ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e3ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-115">Not supported.</span></span>    |
|<span data-ttu-id="3e3ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e3ad-116">Application</span></span> | <span data-ttu-id="3e3ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e3ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e3ad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="3e3ad-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e3ad-119">Request headers</span></span>
| <span data-ttu-id="3e3ad-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3e3ad-120">Name</span></span>       | <span data-ttu-id="3e3ad-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3e3ad-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e3ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e3ad-122">Authorization</span></span>  | <span data-ttu-id="3e3ad-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e3ad-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3e3ad-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e3ad-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e3ad-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e3ad-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3e3ad-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e3ad-129">Response</span></span>

<span data-ttu-id="3e3ad-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e3ad-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3e3ad-131">Example</span></span>
<span data-ttu-id="3e3ad-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3e3ad-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e3ad-133">Request</span></span>
<span data-ttu-id="3e3ad-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="3e3ad-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e3ad-135">Response</span></span>
<span data-ttu-id="3e3ad-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e3ad-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3e3ad-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="3e3ad-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3e3ad-140">C#</span><span class="sxs-lookup"><span data-stu-id="3e3ad-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/table_converttorange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e3ad-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e3ad-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/table_converttorange-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3e3ad-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3e3ad-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/table_converttorange-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
