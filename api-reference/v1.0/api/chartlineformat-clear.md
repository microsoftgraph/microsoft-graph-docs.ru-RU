---
title: 'ChartLineFormat: clear'
description: Очищает формат линий элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3e0a1cdef407f6fe750e0f64a8a7ecc4ea90344c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443282"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="c054f-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="c054f-103">ChartLineFormat: clear</span></span>

<span data-ttu-id="c054f-104">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c054f-104">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="c054f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c054f-105">Permissions</span></span>
<span data-ttu-id="c054f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c054f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c054f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c054f-108">Permission type</span></span>      | <span data-ttu-id="c054f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c054f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c054f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c054f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c054f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c054f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c054f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c054f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c054f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c054f-113">Not supported.</span></span>    |
|<span data-ttu-id="c054f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c054f-114">Application</span></span> | <span data-ttu-id="c054f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c054f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c054f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c054f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="c054f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c054f-117">Request headers</span></span>
| <span data-ttu-id="c054f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c054f-118">Name</span></span>       | <span data-ttu-id="c054f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c054f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c054f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c054f-120">Authorization</span></span>  | <span data-ttu-id="c054f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c054f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c054f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c054f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c054f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c054f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c054f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c054f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c054f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c054f-127">Response</span></span>

<span data-ttu-id="c054f-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c054f-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c054f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c054f-130">Example</span></span>
<span data-ttu-id="c054f-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c054f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c054f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c054f-132">Request</span></span>
<span data-ttu-id="c054f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c054f-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c054f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c054f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c054f-135">C#</span><span class="sxs-lookup"><span data-stu-id="c054f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartlineformat-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c054f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c054f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartlineformat-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c054f-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c054f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartlineformat-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c054f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c054f-138">Response</span></span>
<span data-ttu-id="c054f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c054f-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
