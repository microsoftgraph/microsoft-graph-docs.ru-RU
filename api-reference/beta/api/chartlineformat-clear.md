---
title: 'ChartLineFormat: clear'
description: Очищает формат линий элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3b9f43d877a008780b8e7ce50b39fea70bd5fa78
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33585242"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="9176e-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="9176e-103">ChartLineFormat: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9176e-104">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9176e-104">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="9176e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9176e-105">Permissions</span></span>
<span data-ttu-id="9176e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9176e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9176e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9176e-108">Permission type</span></span>      | <span data-ttu-id="9176e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9176e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9176e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9176e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9176e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9176e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9176e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9176e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9176e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9176e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9176e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9176e-114">Application</span></span> | <span data-ttu-id="9176e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9176e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9176e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9176e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="9176e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9176e-117">Request headers</span></span>
| <span data-ttu-id="9176e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9176e-118">Name</span></span>       | <span data-ttu-id="9176e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9176e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9176e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9176e-120">Authorization</span></span>  | <span data-ttu-id="9176e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9176e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9176e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9176e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9176e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9176e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9176e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9176e-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9176e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9176e-127">Response</span></span>

<span data-ttu-id="9176e-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9176e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9176e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9176e-130">Example</span></span>
<span data-ttu-id="9176e-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9176e-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9176e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9176e-132">Request</span></span>
<span data-ttu-id="9176e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9176e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
```

##### <a name="response"></a><span data-ttu-id="9176e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9176e-134">Response</span></span>
<span data-ttu-id="9176e-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9176e-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9176e-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9176e-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9176e-137">Языках</span><span class="sxs-lookup"><span data-stu-id="9176e-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chartlineformat_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9176e-138">Язык</span><span class="sxs-lookup"><span data-stu-id="9176e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chartlineformat_clear-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartlineformat-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartlineformat-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
