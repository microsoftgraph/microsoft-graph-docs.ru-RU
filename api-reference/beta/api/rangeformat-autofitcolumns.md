---
title: 'RangeFormat: autofitColumns'
description: Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: d06b203cf8d3958fb1a159f21ea1420d11f5399f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455765"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="75ac8-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="75ac8-103">RangeFormat: autofitColumns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75ac8-104">Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="75ac8-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="75ac8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75ac8-105">Permissions</span></span>
<span data-ttu-id="75ac8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75ac8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75ac8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75ac8-108">Permission type</span></span>      | <span data-ttu-id="75ac8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75ac8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75ac8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75ac8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75ac8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75ac8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75ac8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75ac8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75ac8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75ac8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75ac8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75ac8-114">Application</span></span> | <span data-ttu-id="75ac8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ac8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75ac8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75ac8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="75ac8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75ac8-117">Request headers</span></span>
| <span data-ttu-id="75ac8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="75ac8-118">Name</span></span>       | <span data-ttu-id="75ac8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="75ac8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75ac8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75ac8-120">Authorization</span></span>  | <span data-ttu-id="75ac8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75ac8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75ac8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75ac8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="75ac8-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="75ac8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75ac8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75ac8-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="75ac8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="75ac8-127">Response</span></span>

<span data-ttu-id="75ac8-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="75ac8-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75ac8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="75ac8-130">Example</span></span>
<span data-ttu-id="75ac8-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="75ac8-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75ac8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="75ac8-132">Request</span></span>
<span data-ttu-id="75ac8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75ac8-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75ac8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="75ac8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75ac8-135">C#</span><span class="sxs-lookup"><span data-stu-id="75ac8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75ac8-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="75ac8-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75ac8-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="75ac8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="75ac8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="75ac8-138">Response</span></span>
<span data-ttu-id="75ac8-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75ac8-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
