---
title: 'Table: convertToRange'
description: Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 19d9f7e84d18886826455ba961e86ab93b4af1dc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603114"
---
# <a name="table-converttorange"></a><span data-ttu-id="b2f60-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="b2f60-104">Table: convertToRange</span></span>

<span data-ttu-id="b2f60-p102">Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.</span><span class="sxs-lookup"><span data-stu-id="b2f60-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="b2f60-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2f60-107">Permissions</span></span>
<span data-ttu-id="b2f60-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2f60-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2f60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2f60-110">Permission type</span></span>      | <span data-ttu-id="b2f60-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2f60-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2f60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2f60-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2f60-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2f60-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2f60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2f60-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2f60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2f60-115">Not supported.</span></span>    |
|<span data-ttu-id="b2f60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2f60-116">Application</span></span> | <span data-ttu-id="b2f60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2f60-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2f60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2f60-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="b2f60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2f60-119">Request headers</span></span>
| <span data-ttu-id="b2f60-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b2f60-120">Name</span></span>       | <span data-ttu-id="b2f60-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b2f60-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2f60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2f60-122">Authorization</span></span>  | <span data-ttu-id="b2f60-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2f60-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2f60-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b2f60-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b2f60-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b2f60-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2f60-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2f60-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b2f60-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2f60-129">Response</span></span>

<span data-ttu-id="b2f60-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b2f60-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2f60-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b2f60-131">Example</span></span>
<span data-ttu-id="b2f60-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b2f60-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b2f60-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2f60-133">Request</span></span>
<span data-ttu-id="b2f60-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2f60-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="b2f60-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2f60-135">Response</span></span>
<span data-ttu-id="b2f60-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2f60-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b2f60-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b2f60-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b2f60-140">Языках</span><span class="sxs-lookup"><span data-stu-id="b2f60-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/table_converttorange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2f60-141">Язык</span><span class="sxs-lookup"><span data-stu-id="b2f60-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/table_converttorange-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
