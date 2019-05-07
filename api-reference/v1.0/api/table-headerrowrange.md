---
title: 'Table: HeaderRowRange'
description: Получает объект диапазона, связанный со строкой заголовков таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: afb79b0ed44ca84d0a0f58fb4590c16e7148bfb3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602940"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="f3426-103">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="f3426-103">Table: HeaderRowRange</span></span>

<span data-ttu-id="f3426-104">Получает объект диапазона, связанный со строкой заголовков таблицы.</span><span class="sxs-lookup"><span data-stu-id="f3426-104">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3426-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3426-105">Permissions</span></span>
<span data-ttu-id="f3426-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3426-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3426-108">Permission type</span></span>      | <span data-ttu-id="f3426-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3426-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3426-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3426-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3426-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3426-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f3426-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3426-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3426-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3426-113">Not supported.</span></span>    |
|<span data-ttu-id="f3426-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3426-114">Application</span></span> | <span data-ttu-id="f3426-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3426-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3426-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3426-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="f3426-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3426-117">Request headers</span></span>
| <span data-ttu-id="f3426-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f3426-118">Name</span></span>       | <span data-ttu-id="f3426-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f3426-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3426-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3426-120">Authorization</span></span>  | <span data-ttu-id="f3426-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3426-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3426-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f3426-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f3426-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f3426-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3426-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3426-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f3426-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3426-127">Response</span></span>

<span data-ttu-id="f3426-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f3426-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3426-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f3426-129">Example</span></span>
<span data-ttu-id="f3426-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f3426-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f3426-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3426-131">Request</span></span>
<span data-ttu-id="f3426-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3426-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange
```

##### <a name="response"></a><span data-ttu-id="f3426-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3426-133">Response</span></span>
<span data-ttu-id="f3426-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3426-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f3426-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="f3426-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f3426-138">Языках</span><span class="sxs-lookup"><span data-stu-id="f3426-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/table_headerrowrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3426-139">Язык</span><span class="sxs-lookup"><span data-stu-id="f3426-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/table_headerrowrange-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-headerrowrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-headerrowrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
