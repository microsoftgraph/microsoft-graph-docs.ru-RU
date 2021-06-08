---
title: 'Range: clear'
description: Очищает формат, заливку, границу, значения диапазона и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cc737b9a1f07ce8274fe3ac7ed2ccd105802d24d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786140"
---
# <a name="range-clear"></a><span data-ttu-id="b11d0-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="b11d0-103">Range: clear</span></span>

<span data-ttu-id="b11d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b11d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b11d0-105">Очищает формат, заливку, границу, значения диапазона и т. д.</span><span class="sxs-lookup"><span data-stu-id="b11d0-105">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="b11d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b11d0-106">Permissions</span></span>
<span data-ttu-id="b11d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b11d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b11d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b11d0-109">Permission type</span></span>      | <span data-ttu-id="b11d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b11d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b11d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b11d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b11d0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b11d0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b11d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b11d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b11d0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b11d0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b11d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b11d0-115">Application</span></span> | <span data-ttu-id="b11d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b11d0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b11d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b11d0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/clear
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="b11d0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b11d0-118">Request headers</span></span>
| <span data-ttu-id="b11d0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b11d0-119">Name</span></span>       | <span data-ttu-id="b11d0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b11d0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b11d0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b11d0-121">Authorization</span></span>  | <span data-ttu-id="b11d0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b11d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b11d0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b11d0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b11d0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b11d0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b11d0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b11d0-127">Request body</span></span>
<span data-ttu-id="b11d0-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b11d0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b11d0-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="b11d0-129">Parameter</span></span>    | <span data-ttu-id="b11d0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b11d0-130">Type</span></span>   |<span data-ttu-id="b11d0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b11d0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b11d0-132">applyTo</span><span class="sxs-lookup"><span data-stu-id="b11d0-132">applyTo</span></span>|<span data-ttu-id="b11d0-133">string</span><span class="sxs-lookup"><span data-stu-id="b11d0-133">string</span></span>|<span data-ttu-id="b11d0-p104">Необязательный параметр. Определяет тип действия очистки.  Возможные значения: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="b11d0-p104">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="b11d0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b11d0-137">Response</span></span>

<span data-ttu-id="b11d0-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b11d0-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b11d0-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b11d0-140">Example</span></span>
<span data-ttu-id="b11d0-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b11d0-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b11d0-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b11d0-142">Request</span></span>
<span data-ttu-id="b11d0-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b11d0-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b11d0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b11d0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b11d0-145">C#</span><span class="sxs-lookup"><span data-stu-id="b11d0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b11d0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b11d0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b11d0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b11d0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b11d0-148">Java</span><span class="sxs-lookup"><span data-stu-id="b11d0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b11d0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b11d0-149">Response</span></span>
<span data-ttu-id="b11d0-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b11d0-150">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


