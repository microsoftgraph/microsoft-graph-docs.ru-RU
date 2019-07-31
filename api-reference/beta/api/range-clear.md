---
title: 'Range: clear'
description: Очищает формат, заливку, границу, значения диапазона и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ca611a395858ff5b59dda502d550eef23a0d5d07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978527"
---
# <a name="range-clear"></a><span data-ttu-id="0c4e8-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="0c4e8-103">Range: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c4e8-104">Очищает формат, заливку, границу, значения диапазона и т. д.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c4e8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4e8-105">Permissions</span></span>
<span data-ttu-id="0c4e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c4e8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4e8-108">Permission type</span></span>      | <span data-ttu-id="0c4e8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c4e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c4e8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c4e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c4e8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c4e8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c4e8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c4e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4e8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c4e8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c4e8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c4e8-114">Application</span></span> | <span data-ttu-id="0c4e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c4e8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c4e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="0c4e8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c4e8-117">Request headers</span></span>
| <span data-ttu-id="0c4e8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0c4e8-118">Name</span></span>       | <span data-ttu-id="0c4e8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4e8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c4e8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c4e8-120">Authorization</span></span>  | <span data-ttu-id="0c4e8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c4e8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0c4e8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0c4e8-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c4e8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c4e8-126">Request body</span></span>
<span data-ttu-id="0c4e8-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c4e8-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="0c4e8-128">Parameter</span></span>    | <span data-ttu-id="0c4e8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0c4e8-129">Type</span></span>   |<span data-ttu-id="0c4e8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4e8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c4e8-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="0c4e8-131">applyTo</span></span>|<span data-ttu-id="0c4e8-132">string</span><span class="sxs-lookup"><span data-stu-id="0c4e8-132">string</span></span>|<span data-ttu-id="0c4e8-p104">Необязательный параметр. Определяет тип действия очистки.  Возможные значения: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-p104">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="0c4e8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c4e8-136">Response</span></span>

<span data-ttu-id="0c4e8-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c4e8-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0c4e8-139">Example</span></span>
<span data-ttu-id="0c4e8-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c4e8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c4e8-141">Request</span></span>
<span data-ttu-id="0c4e8-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c4e8-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c4e8-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c4e8-144">C#</span><span class="sxs-lookup"><span data-stu-id="0c4e8-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c4e8-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c4e8-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c4e8-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0c4e8-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c4e8-147">Java</span><span class="sxs-lookup"><span data-stu-id="0c4e8-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c4e8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c4e8-148">Response</span></span>
<span data-ttu-id="0c4e8-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c4e8-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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
