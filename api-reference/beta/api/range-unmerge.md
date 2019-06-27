---
title: 'Range: unmerge'
description: Разъединяет ячейки диапазона на отдельные ячейки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4214d2505e1a223ed479e0ebaa4a6be2a42c0a13
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265522"
---
# <a name="range-unmerge"></a><span data-ttu-id="e67d6-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="e67d6-103">Range: unmerge</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e67d6-104">Разъединяет ячейки диапазона на отдельные ячейки.</span><span class="sxs-lookup"><span data-stu-id="e67d6-104">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="e67d6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e67d6-105">Permissions</span></span>
<span data-ttu-id="e67d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e67d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e67d6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e67d6-108">Permission type</span></span>      | <span data-ttu-id="e67d6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e67d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e67d6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e67d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e67d6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e67d6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e67d6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e67d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e67d6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e67d6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e67d6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e67d6-114">Application</span></span> | <span data-ttu-id="e67d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e67d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e67d6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e67d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="e67d6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e67d6-117">Request headers</span></span>
| <span data-ttu-id="e67d6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e67d6-118">Name</span></span>       | <span data-ttu-id="e67d6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e67d6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e67d6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e67d6-120">Authorization</span></span>  | <span data-ttu-id="e67d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e67d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e67d6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e67d6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e67d6-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e67d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e67d6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e67d6-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e67d6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e67d6-127">Response</span></span>

<span data-ttu-id="e67d6-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e67d6-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e67d6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e67d6-130">Example</span></span>
<span data-ttu-id="e67d6-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e67d6-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e67d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e67d6-132">Request</span></span>
<span data-ttu-id="e67d6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e67d6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```

##### <a name="response"></a><span data-ttu-id="e67d6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e67d6-134">Response</span></span>
<span data-ttu-id="e67d6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e67d6-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e67d6-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e67d6-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e67d6-137">C#</span><span class="sxs-lookup"><span data-stu-id="e67d6-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_unmerge-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e67d6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="e67d6-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_unmerge-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e67d6-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e67d6-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_unmerge-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-unmerge.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-unmerge.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-unmerge.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
