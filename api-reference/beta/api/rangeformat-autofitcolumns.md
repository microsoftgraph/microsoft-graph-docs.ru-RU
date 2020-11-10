---
title: 'RangeFormat: autofitColumns'
description: Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9137e971aeb1cfcce454af61bba20c54c1537354
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973726"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="fb558-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="fb558-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="fb558-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb558-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb558-105">Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="fb558-105">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb558-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb558-106">Permissions</span></span>
<span data-ttu-id="fb558-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb558-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb558-109">Permission type</span></span>      | <span data-ttu-id="fb558-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb558-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb558-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb558-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fb558-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb558-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb558-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb558-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb558-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb558-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb558-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb558-115">Application</span></span> | <span data-ttu-id="fb558-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb558-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb558-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb558-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="fb558-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb558-118">Request headers</span></span>
| <span data-ttu-id="fb558-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fb558-119">Name</span></span>       | <span data-ttu-id="fb558-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fb558-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fb558-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb558-121">Authorization</span></span>  | <span data-ttu-id="fb558-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb558-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fb558-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fb558-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="fb558-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fb558-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb558-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb558-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fb558-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb558-128">Response</span></span>

<span data-ttu-id="fb558-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fb558-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb558-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fb558-131">Example</span></span>
<span data-ttu-id="fb558-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fb558-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fb558-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb558-133">Request</span></span>
<span data-ttu-id="fb558-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb558-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fb558-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb558-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="c"></a>[<span data-ttu-id="fb558-136">C#</span><span class="sxs-lookup"><span data-stu-id="fb558-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb558-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb558-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb558-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb558-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb558-139">Java</span><span class="sxs-lookup"><span data-stu-id="fb558-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangeformat-autofitcolumns-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fb558-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb558-140">Response</span></span>
<span data-ttu-id="fb558-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fb558-141">Here is an example of the response.</span></span> 
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


