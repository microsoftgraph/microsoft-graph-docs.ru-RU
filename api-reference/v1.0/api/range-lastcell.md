---
title: 'Range: LastCell'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8924739bf59468581dbcbd3f4380d5f583277b76
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459092"
---
# <a name="range-lastcell"></a><span data-ttu-id="0a1f6-103">Range: LastCell</span><span class="sxs-lookup"><span data-stu-id="0a1f6-103">Range: LastCell</span></span>

<span data-ttu-id="0a1f6-p101">Возвращает последнюю ячейку в диапазоне. Например, последняя ячейка диапазона B2:D5 — D5.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-p101">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="0a1f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a1f6-106">Permissions</span></span>
<span data-ttu-id="0a1f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a1f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a1f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a1f6-109">Permission type</span></span>      | <span data-ttu-id="0a1f6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a1f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a1f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a1f6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a1f6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a1f6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a1f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a1f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a1f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-114">Not supported.</span></span>    |
|<span data-ttu-id="0a1f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a1f6-115">Application</span></span> | <span data-ttu-id="0a1f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a1f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a1f6-117">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a1f6-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a1f6-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastCell
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastCell
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastCell

```
## <a name="request-headers"></a><span data-ttu-id="0a1f6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a1f6-119">Request headers</span></span>
| <span data-ttu-id="0a1f6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0a1f6-120">Name</span></span>       | <span data-ttu-id="0a1f6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0a1f6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0a1f6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a1f6-122">Authorization</span></span>  | <span data-ttu-id="0a1f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a1f6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0a1f6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0a1f6-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a1f6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a1f6-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0a1f6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a1f6-129">Response</span></span>

<span data-ttu-id="0a1f6-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1f6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0a1f6-131">Example</span></span>
<span data-ttu-id="0a1f6-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0a1f6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a1f6-133">Request</span></span>
<span data-ttu-id="0a1f6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-134">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastCell
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a1f6-135">C#</span><span class="sxs-lookup"><span data-stu-id="0a1f6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a1f6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a1f6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a1f6-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0a1f6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0a1f6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a1f6-138">Response</span></span>
<span data-ttu-id="0a1f6-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastCell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
