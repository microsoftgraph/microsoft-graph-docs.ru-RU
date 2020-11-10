---
title: 'RangeFormat: autofitRows'
description: Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9ec2fba555be3354b7e22db6d55efd294bb6bf17
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973685"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="57171-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="57171-103">RangeFormat: autofitRows</span></span>

<span data-ttu-id="57171-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57171-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57171-105">Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="57171-105">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="57171-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57171-106">Permissions</span></span>
<span data-ttu-id="57171-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57171-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57171-109">Permission type</span></span>      | <span data-ttu-id="57171-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57171-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57171-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57171-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57171-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57171-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57171-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57171-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57171-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57171-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57171-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57171-115">Application</span></span> | <span data-ttu-id="57171-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57171-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57171-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57171-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="57171-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57171-118">Request headers</span></span>
| <span data-ttu-id="57171-119">Имя</span><span class="sxs-lookup"><span data-stu-id="57171-119">Name</span></span>       | <span data-ttu-id="57171-120">Описание</span><span class="sxs-lookup"><span data-stu-id="57171-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57171-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57171-121">Authorization</span></span>  | <span data-ttu-id="57171-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57171-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57171-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="57171-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="57171-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="57171-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57171-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57171-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="57171-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="57171-128">Response</span></span>

<span data-ttu-id="57171-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="57171-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57171-131">Пример</span><span class="sxs-lookup"><span data-stu-id="57171-131">Example</span></span>
<span data-ttu-id="57171-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="57171-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57171-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="57171-133">Request</span></span>
<span data-ttu-id="57171-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57171-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57171-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="57171-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows
```
# <a name="c"></a>[<span data-ttu-id="57171-136">C#</span><span class="sxs-lookup"><span data-stu-id="57171-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitrows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57171-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57171-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitrows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57171-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57171-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitrows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57171-139">Java</span><span class="sxs-lookup"><span data-stu-id="57171-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangeformat-autofitrows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="57171-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="57171-140">Response</span></span>
<span data-ttu-id="57171-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57171-141">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


