---
title: 'Range: clear'
description: Очищает формат, заливку, границу, значения диапазона и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 43b04b3404cbebdc893919710f0da3b402bfe8ef
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577942"
---
# <a name="range-clear"></a><span data-ttu-id="403c9-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="403c9-103">Range: clear</span></span>

<span data-ttu-id="403c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="403c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="403c9-105">Очищает формат, заливку, границу, значения диапазона и т. д.</span><span class="sxs-lookup"><span data-stu-id="403c9-105">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="403c9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="403c9-106">Permissions</span></span>
<span data-ttu-id="403c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="403c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="403c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="403c9-109">Permission type</span></span>      | <span data-ttu-id="403c9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="403c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="403c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="403c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="403c9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="403c9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="403c9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="403c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="403c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="403c9-114">Not supported.</span></span>    |
|<span data-ttu-id="403c9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="403c9-115">Application</span></span> | <span data-ttu-id="403c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="403c9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="403c9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="403c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/clear
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="403c9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="403c9-118">Request headers</span></span>
| <span data-ttu-id="403c9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="403c9-119">Name</span></span>       | <span data-ttu-id="403c9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="403c9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="403c9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="403c9-121">Authorization</span></span>  | <span data-ttu-id="403c9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="403c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="403c9-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="403c9-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="403c9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="403c9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="403c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="403c9-127">Request body</span></span>
<span data-ttu-id="403c9-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="403c9-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="403c9-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="403c9-129">Parameter</span></span>    | <span data-ttu-id="403c9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="403c9-130">Type</span></span>   |<span data-ttu-id="403c9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="403c9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="403c9-132">applyTo</span><span class="sxs-lookup"><span data-stu-id="403c9-132">applyTo</span></span>|<span data-ttu-id="403c9-133">string</span><span class="sxs-lookup"><span data-stu-id="403c9-133">string</span></span>|<span data-ttu-id="403c9-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="403c9-134">Optional.</span></span> <span data-ttu-id="403c9-135">Определяет тип действия очистки.</span><span class="sxs-lookup"><span data-stu-id="403c9-135">Determines the type of clear action.</span></span>  <span data-ttu-id="403c9-136">Допустимые значения: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="403c9-136">The possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="403c9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="403c9-137">Response</span></span>

<span data-ttu-id="403c9-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="403c9-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="403c9-140">Пример</span><span class="sxs-lookup"><span data-stu-id="403c9-140">Example</span></span>
<span data-ttu-id="403c9-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="403c9-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="403c9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="403c9-142">Request</span></span>
<span data-ttu-id="403c9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="403c9-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="403c9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="403c9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```
# <a name="c"></a>[<span data-ttu-id="403c9-145">C#</span><span class="sxs-lookup"><span data-stu-id="403c9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="403c9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="403c9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="403c9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="403c9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="403c9-148">Java</span><span class="sxs-lookup"><span data-stu-id="403c9-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="403c9-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="403c9-149">Response</span></span>
<span data-ttu-id="403c9-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="403c9-150">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

