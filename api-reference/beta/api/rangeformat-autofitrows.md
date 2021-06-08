---
title: 'RangeFormat: autofitRows'
description: Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bf283465170a45f5ca64c1761e7dd673f29f011a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785881"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="a89e2-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="a89e2-103">RangeFormat: autofitRows</span></span>

<span data-ttu-id="a89e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89e2-105">Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="a89e2-105">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="a89e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a89e2-106">Permissions</span></span>
<span data-ttu-id="a89e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a89e2-109">Permission type</span></span>      | <span data-ttu-id="a89e2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a89e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a89e2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a89e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a89e2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a89e2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a89e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a89e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a89e2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a89e2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a89e2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a89e2-115">Application</span></span> | <span data-ttu-id="a89e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89e2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a89e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a89e2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/autofitRows
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="a89e2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a89e2-118">Request headers</span></span>
| <span data-ttu-id="a89e2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a89e2-119">Name</span></span>       | <span data-ttu-id="a89e2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a89e2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a89e2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a89e2-121">Authorization</span></span>  | <span data-ttu-id="a89e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a89e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a89e2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a89e2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a89e2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a89e2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a89e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a89e2-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a89e2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89e2-128">Response</span></span>

<span data-ttu-id="a89e2-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a89e2-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a89e2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a89e2-131">Example</span></span>
<span data-ttu-id="a89e2-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a89e2-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a89e2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a89e2-133">Request</span></span>
<span data-ttu-id="a89e2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a89e2-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a89e2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89e2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows
```
# <a name="c"></a>[<span data-ttu-id="a89e2-136">C#</span><span class="sxs-lookup"><span data-stu-id="a89e2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitrows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a89e2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a89e2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitrows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a89e2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a89e2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitrows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a89e2-139">Java</span><span class="sxs-lookup"><span data-stu-id="a89e2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangeformat-autofitrows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a89e2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89e2-140">Response</span></span>
<span data-ttu-id="a89e2-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a89e2-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

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
  ]
}
-->


