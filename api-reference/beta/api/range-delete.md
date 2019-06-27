---
title: 'Range: delete'
description: Удаляет ячейки, связанные с диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc9404bd6560973dc3fb256d40320a1df77e801b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267643"
---
# <a name="range-delete"></a><span data-ttu-id="dc787-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="dc787-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc787-104">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="dc787-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc787-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc787-105">Permissions</span></span>
<span data-ttu-id="dc787-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc787-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc787-108">Permission type</span></span>      | <span data-ttu-id="dc787-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc787-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc787-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc787-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc787-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc787-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc787-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc787-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc787-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc787-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc787-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc787-114">Application</span></span> | <span data-ttu-id="dc787-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc787-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc787-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc787-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="dc787-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc787-117">Request headers</span></span>
| <span data-ttu-id="dc787-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dc787-118">Name</span></span>       | <span data-ttu-id="dc787-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dc787-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc787-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc787-120">Authorization</span></span>  | <span data-ttu-id="dc787-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc787-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc787-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc787-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc787-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc787-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc787-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc787-126">Request body</span></span>
<span data-ttu-id="dc787-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dc787-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc787-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="dc787-128">Parameter</span></span>    | <span data-ttu-id="dc787-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dc787-129">Type</span></span>   |<span data-ttu-id="dc787-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dc787-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc787-131">shift</span><span class="sxs-lookup"><span data-stu-id="dc787-131">shift</span></span>|<span data-ttu-id="dc787-132">string</span><span class="sxs-lookup"><span data-stu-id="dc787-132">string</span></span>|<span data-ttu-id="dc787-p104">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="dc787-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="dc787-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc787-135">Response</span></span>

<span data-ttu-id="dc787-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dc787-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc787-138">Пример</span><span class="sxs-lookup"><span data-stu-id="dc787-138">Example</span></span>
<span data-ttu-id="dc787-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dc787-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc787-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc787-140">Request</span></span>
<span data-ttu-id="dc787-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc787-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="dc787-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc787-142">Response</span></span>
<span data-ttu-id="dc787-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc787-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dc787-144">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="dc787-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dc787-145">C#</span><span class="sxs-lookup"><span data-stu-id="dc787-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc787-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc787-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dc787-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dc787-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_delete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
