---
title: 'Table: convertToRange'
description: Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 00fd43ca5dc3f2647f438d4ee7caa9fc1fcb215a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409630"
---
# <a name="table-converttorange"></a><span data-ttu-id="dc516-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="dc516-104">Table: convertToRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc516-p102">Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.</span><span class="sxs-lookup"><span data-stu-id="dc516-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc516-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc516-107">Permissions</span></span>
<span data-ttu-id="dc516-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc516-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc516-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc516-110">Permission type</span></span>      | <span data-ttu-id="dc516-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc516-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc516-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc516-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dc516-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc516-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc516-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc516-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc516-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc516-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc516-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc516-116">Application</span></span> | <span data-ttu-id="dc516-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc516-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc516-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc516-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="dc516-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc516-119">Request headers</span></span>
| <span data-ttu-id="dc516-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dc516-120">Name</span></span>       | <span data-ttu-id="dc516-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dc516-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc516-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc516-122">Authorization</span></span>  | <span data-ttu-id="dc516-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc516-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc516-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc516-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc516-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc516-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc516-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc516-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dc516-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc516-129">Response</span></span>

<span data-ttu-id="dc516-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dc516-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc516-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dc516-131">Example</span></span>
<span data-ttu-id="dc516-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dc516-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc516-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc516-133">Request</span></span>
<span data-ttu-id="dc516-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc516-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc516-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc516-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc516-136">C#</span><span class="sxs-lookup"><span data-stu-id="dc516-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-converttorange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc516-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc516-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-converttorange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc516-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dc516-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-converttorange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc516-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc516-139">Response</span></span>
<span data-ttu-id="dc516-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc516-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
