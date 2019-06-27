---
title: 'ChartFill: clear'
description: Очищает цвет заливки элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 01fa603e29a4d19e047bb0dd4cec92624255ab0b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272515"
---
# <a name="chartfill-clear"></a><span data-ttu-id="00600-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="00600-103">ChartFill: clear</span></span>

<span data-ttu-id="00600-104">Очищает цвет заливки элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="00600-104">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="00600-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00600-105">Permissions</span></span>
<span data-ttu-id="00600-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00600-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00600-108">Permission type</span></span>      | <span data-ttu-id="00600-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00600-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00600-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00600-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00600-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00600-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00600-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00600-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00600-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00600-113">Not supported.</span></span>    |
|<span data-ttu-id="00600-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00600-114">Application</span></span> | <span data-ttu-id="00600-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00600-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00600-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00600-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="00600-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00600-117">Request headers</span></span>
| <span data-ttu-id="00600-118">Имя</span><span class="sxs-lookup"><span data-stu-id="00600-118">Name</span></span>       | <span data-ttu-id="00600-119">Описание</span><span class="sxs-lookup"><span data-stu-id="00600-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00600-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00600-120">Authorization</span></span>  | <span data-ttu-id="00600-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00600-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00600-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="00600-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="00600-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="00600-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00600-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00600-126">Request body</span></span>
<span data-ttu-id="00600-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00600-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00600-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="00600-128">Response</span></span>

<span data-ttu-id="00600-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="00600-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00600-131">Пример</span><span class="sxs-lookup"><span data-stu-id="00600-131">Example</span></span>
<span data-ttu-id="00600-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="00600-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="00600-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="00600-133">Request</span></span>
<span data-ttu-id="00600-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00600-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="00600-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="00600-135">Response</span></span>
<span data-ttu-id="00600-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00600-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="00600-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="00600-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="00600-138">C#</span><span class="sxs-lookup"><span data-stu-id="00600-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chartfill_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00600-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="00600-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chartfill_clear-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="00600-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="00600-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chartfill_clear-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartfill-clear.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartfill-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartfill-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
