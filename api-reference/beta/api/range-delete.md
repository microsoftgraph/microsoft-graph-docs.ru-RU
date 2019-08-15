---
title: 'Range: delete'
description: Удаляет ячейки, связанные с диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f48e7a51c718782e8c38b96bafe8d4110520baa4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412301"
---
# <a name="range-delete"></a><span data-ttu-id="3aed5-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="3aed5-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aed5-104">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="3aed5-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="3aed5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3aed5-105">Permissions</span></span>
<span data-ttu-id="3aed5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aed5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aed5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3aed5-108">Permission type</span></span>      | <span data-ttu-id="3aed5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3aed5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aed5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3aed5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3aed5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aed5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3aed5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3aed5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aed5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aed5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3aed5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3aed5-114">Application</span></span> | <span data-ttu-id="3aed5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aed5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aed5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3aed5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="3aed5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3aed5-117">Request headers</span></span>
| <span data-ttu-id="3aed5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3aed5-118">Name</span></span>       | <span data-ttu-id="3aed5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3aed5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3aed5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3aed5-120">Authorization</span></span>  | <span data-ttu-id="3aed5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3aed5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3aed5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3aed5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3aed5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3aed5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aed5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3aed5-126">Request body</span></span>
<span data-ttu-id="3aed5-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3aed5-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3aed5-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="3aed5-128">Parameter</span></span>    | <span data-ttu-id="3aed5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3aed5-129">Type</span></span>   |<span data-ttu-id="3aed5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3aed5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3aed5-131">shift</span><span class="sxs-lookup"><span data-stu-id="3aed5-131">shift</span></span>|<span data-ttu-id="3aed5-132">string</span><span class="sxs-lookup"><span data-stu-id="3aed5-132">string</span></span>|<span data-ttu-id="3aed5-p104">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="3aed5-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="3aed5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3aed5-135">Response</span></span>

<span data-ttu-id="3aed5-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3aed5-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aed5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3aed5-138">Example</span></span>
<span data-ttu-id="3aed5-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3aed5-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3aed5-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3aed5-140">Request</span></span>
<span data-ttu-id="3aed5-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3aed5-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3aed5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aed5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3aed5-143">C#</span><span class="sxs-lookup"><span data-stu-id="3aed5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3aed5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aed5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3aed5-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3aed5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3aed5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3aed5-146">Response</span></span>
<span data-ttu-id="3aed5-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3aed5-147">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
