---
title: 'RangeFormat: autofitColumns'
description: Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 57fe37109c1308de3cd716a985da0de7b9691f56
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573931"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="08fc3-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="08fc3-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="08fc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08fc3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08fc3-105">Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="08fc3-105">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="08fc3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08fc3-106">Permissions</span></span>
<span data-ttu-id="08fc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08fc3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08fc3-109">Permission type</span></span>      | <span data-ttu-id="08fc3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08fc3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08fc3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08fc3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="08fc3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08fc3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="08fc3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08fc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08fc3-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08fc3-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="08fc3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08fc3-115">Application</span></span> | <span data-ttu-id="08fc3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08fc3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08fc3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08fc3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/autofitColumns
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="08fc3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08fc3-118">Request headers</span></span>
| <span data-ttu-id="08fc3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="08fc3-119">Name</span></span>       | <span data-ttu-id="08fc3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="08fc3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08fc3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08fc3-121">Authorization</span></span>  | <span data-ttu-id="08fc3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08fc3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08fc3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="08fc3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="08fc3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="08fc3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08fc3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08fc3-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="08fc3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="08fc3-128">Response</span></span>

<span data-ttu-id="08fc3-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="08fc3-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08fc3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="08fc3-131">Example</span></span>
<span data-ttu-id="08fc3-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="08fc3-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08fc3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="08fc3-133">Request</span></span>
<span data-ttu-id="08fc3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08fc3-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08fc3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="08fc3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="c"></a>[<span data-ttu-id="08fc3-136">C#</span><span class="sxs-lookup"><span data-stu-id="08fc3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08fc3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08fc3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08fc3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08fc3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08fc3-139">Java</span><span class="sxs-lookup"><span data-stu-id="08fc3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangeformat-autofitcolumns-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08fc3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="08fc3-140">Response</span></span>
<span data-ttu-id="08fc3-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08fc3-141">Here is an example of the response.</span></span> 
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


