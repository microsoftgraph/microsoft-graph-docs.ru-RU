---
title: 'RangeFormat: autofitColumns'
description: Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1bd7511f2fd27083e561c015b5090d8b11781bf7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454603"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="39002-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="39002-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="39002-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="39002-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39002-105">Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="39002-105">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="39002-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39002-106">Permissions</span></span>
<span data-ttu-id="39002-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39002-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39002-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39002-109">Permission type</span></span>      | <span data-ttu-id="39002-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39002-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39002-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39002-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39002-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39002-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39002-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39002-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39002-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39002-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39002-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39002-115">Application</span></span> | <span data-ttu-id="39002-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39002-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39002-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39002-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="39002-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39002-118">Request headers</span></span>
| <span data-ttu-id="39002-119">Имя</span><span class="sxs-lookup"><span data-stu-id="39002-119">Name</span></span>       | <span data-ttu-id="39002-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39002-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="39002-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39002-121">Authorization</span></span>  | <span data-ttu-id="39002-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39002-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39002-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="39002-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="39002-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="39002-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39002-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39002-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="39002-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="39002-128">Response</span></span>

<span data-ttu-id="39002-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="39002-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39002-131">Пример</span><span class="sxs-lookup"><span data-stu-id="39002-131">Example</span></span>
<span data-ttu-id="39002-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="39002-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="39002-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="39002-133">Request</span></span>
<span data-ttu-id="39002-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39002-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39002-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="39002-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="c"></a>[<span data-ttu-id="39002-136">C#</span><span class="sxs-lookup"><span data-stu-id="39002-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39002-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39002-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39002-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39002-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="39002-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="39002-139">Response</span></span>
<span data-ttu-id="39002-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39002-140">Here is an example of the response.</span></span> 
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
