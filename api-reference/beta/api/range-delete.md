---
title: 'Range: delete'
description: Удаляет ячейки, связанные с диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1900ae6f02414d177f2aea5a90d9c5d940cc6792
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454784"
---
# <a name="range-delete"></a><span data-ttu-id="98c64-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="98c64-103">Range: delete</span></span>

<span data-ttu-id="98c64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98c64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98c64-105">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="98c64-105">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="98c64-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98c64-106">Permissions</span></span>
<span data-ttu-id="98c64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98c64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98c64-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98c64-109">Permission type</span></span>      | <span data-ttu-id="98c64-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98c64-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98c64-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98c64-111">Delegated (work or school account)</span></span> | <span data-ttu-id="98c64-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98c64-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="98c64-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98c64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98c64-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98c64-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="98c64-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98c64-115">Application</span></span> | <span data-ttu-id="98c64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98c64-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98c64-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98c64-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="98c64-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98c64-118">Request headers</span></span>
| <span data-ttu-id="98c64-119">Имя</span><span class="sxs-lookup"><span data-stu-id="98c64-119">Name</span></span>       | <span data-ttu-id="98c64-120">Описание</span><span class="sxs-lookup"><span data-stu-id="98c64-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98c64-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98c64-121">Authorization</span></span>  | <span data-ttu-id="98c64-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98c64-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98c64-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="98c64-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="98c64-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="98c64-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98c64-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98c64-127">Request body</span></span>
<span data-ttu-id="98c64-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="98c64-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98c64-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="98c64-129">Parameter</span></span>    | <span data-ttu-id="98c64-130">Тип</span><span class="sxs-lookup"><span data-stu-id="98c64-130">Type</span></span>   |<span data-ttu-id="98c64-131">Описание</span><span class="sxs-lookup"><span data-stu-id="98c64-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98c64-132">shift</span><span class="sxs-lookup"><span data-stu-id="98c64-132">shift</span></span>|<span data-ttu-id="98c64-133">string</span><span class="sxs-lookup"><span data-stu-id="98c64-133">string</span></span>|<span data-ttu-id="98c64-p104">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="98c64-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="98c64-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="98c64-136">Response</span></span>

<span data-ttu-id="98c64-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="98c64-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98c64-139">Пример</span><span class="sxs-lookup"><span data-stu-id="98c64-139">Example</span></span>
<span data-ttu-id="98c64-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="98c64-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="98c64-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="98c64-141">Request</span></span>
<span data-ttu-id="98c64-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98c64-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98c64-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="98c64-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="98c64-144">C#</span><span class="sxs-lookup"><span data-stu-id="98c64-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98c64-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98c64-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98c64-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98c64-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98c64-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="98c64-147">Response</span></span>
<span data-ttu-id="98c64-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98c64-148">Here is an example of the response.</span></span> 
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
