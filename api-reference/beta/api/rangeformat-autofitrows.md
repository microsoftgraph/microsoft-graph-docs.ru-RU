---
title: 'RangeFormat: autofitRows'
description: Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 7976b3be7f95eccf01db7c82c83820676fe35ac7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265438"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="750ae-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="750ae-103">RangeFormat: autofitRows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="750ae-104">Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="750ae-104">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="750ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="750ae-105">Permissions</span></span>
<span data-ttu-id="750ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="750ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="750ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="750ae-108">Permission type</span></span>      | <span data-ttu-id="750ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="750ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="750ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="750ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="750ae-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="750ae-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="750ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="750ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="750ae-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="750ae-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="750ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="750ae-114">Application</span></span> | <span data-ttu-id="750ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="750ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="750ae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="750ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="750ae-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="750ae-117">Request headers</span></span>
| <span data-ttu-id="750ae-118">Имя</span><span class="sxs-lookup"><span data-stu-id="750ae-118">Name</span></span>       | <span data-ttu-id="750ae-119">Описание</span><span class="sxs-lookup"><span data-stu-id="750ae-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="750ae-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="750ae-120">Authorization</span></span>  | <span data-ttu-id="750ae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="750ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="750ae-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="750ae-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="750ae-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="750ae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="750ae-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="750ae-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="750ae-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="750ae-127">Response</span></span>

<span data-ttu-id="750ae-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="750ae-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="750ae-130">Пример</span><span class="sxs-lookup"><span data-stu-id="750ae-130">Example</span></span>
<span data-ttu-id="750ae-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="750ae-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="750ae-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="750ae-132">Request</span></span>
<span data-ttu-id="750ae-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="750ae-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="750ae-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="750ae-134">Response</span></span>
<span data-ttu-id="750ae-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="750ae-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="750ae-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="750ae-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="750ae-137">C#</span><span class="sxs-lookup"><span data-stu-id="750ae-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/rangeformat_autofitrows-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="750ae-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="750ae-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/rangeformat_autofitrows-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="750ae-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="750ae-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/rangeformat_autofitrows-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangeformat-autofitrows.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-autofitrows.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-autofitrows.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
