---
title: 'RangeFormat: autofitColumns'
description: Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 03edc3f2b9c35084c0de1c39df5a45bbeaeb3374
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577256"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="ee0b1-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="ee0b1-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="ee0b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee0b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee0b1-105">Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-105">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee0b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee0b1-106">Permissions</span></span>
<span data-ttu-id="ee0b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee0b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee0b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee0b1-109">Permission type</span></span>      | <span data-ttu-id="ee0b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee0b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee0b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee0b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee0b1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee0b1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee0b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee0b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee0b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-114">Not supported.</span></span>    |
|<span data-ttu-id="ee0b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee0b1-115">Application</span></span> | <span data-ttu-id="ee0b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee0b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee0b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/autofitColumns
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="ee0b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee0b1-118">Request headers</span></span>
| <span data-ttu-id="ee0b1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ee0b1-119">Name</span></span>       | <span data-ttu-id="ee0b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ee0b1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee0b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee0b1-121">Authorization</span></span>  | <span data-ttu-id="ee0b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee0b1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ee0b1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ee0b1-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee0b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee0b1-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ee0b1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee0b1-128">Response</span></span>

<span data-ttu-id="ee0b1-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee0b1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ee0b1-131">Example</span></span>
<span data-ttu-id="ee0b1-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee0b1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee0b1-133">Request</span></span>
<span data-ttu-id="ee0b1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee0b1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee0b1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="c"></a>[<span data-ttu-id="ee0b1-136">C#</span><span class="sxs-lookup"><span data-stu-id="ee0b1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee0b1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee0b1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee0b1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee0b1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee0b1-139">Java</span><span class="sxs-lookup"><span data-stu-id="ee0b1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangeformat-autofitcolumns-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee0b1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee0b1-140">Response</span></span>
<span data-ttu-id="ee0b1-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ee0b1-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

