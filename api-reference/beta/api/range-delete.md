---
title: 'Range: delete'
description: Удаляет ячейки, связанные с диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e6c89780f02f521e6bc60427bdffc63d3e30fe6c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785916"
---
# <a name="range-delete"></a><span data-ttu-id="b9cb2-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="b9cb2-103">Range: delete</span></span>

<span data-ttu-id="b9cb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9cb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9cb2-105">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-105">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9cb2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9cb2-106">Permissions</span></span>
<span data-ttu-id="b9cb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9cb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9cb2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9cb2-109">Permission type</span></span>      | <span data-ttu-id="b9cb2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9cb2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9cb2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9cb2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9cb2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9cb2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9cb2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9cb2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9cb2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9cb2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9cb2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9cb2-115">Application</span></span> | <span data-ttu-id="b9cb2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9cb2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9cb2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/delete
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/delete
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/delete
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="b9cb2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9cb2-118">Request headers</span></span>
| <span data-ttu-id="b9cb2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b9cb2-119">Name</span></span>       | <span data-ttu-id="b9cb2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b9cb2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9cb2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9cb2-121">Authorization</span></span>  | <span data-ttu-id="b9cb2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9cb2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b9cb2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9cb2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9cb2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9cb2-127">Request body</span></span>
<span data-ttu-id="b9cb2-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9cb2-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="b9cb2-129">Parameter</span></span>    | <span data-ttu-id="b9cb2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b9cb2-130">Type</span></span>   |<span data-ttu-id="b9cb2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b9cb2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9cb2-132">shift</span><span class="sxs-lookup"><span data-stu-id="b9cb2-132">shift</span></span>|<span data-ttu-id="b9cb2-133">string</span><span class="sxs-lookup"><span data-stu-id="b9cb2-133">string</span></span>|<span data-ttu-id="b9cb2-p104">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="b9cb2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9cb2-136">Response</span></span>

<span data-ttu-id="b9cb2-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9cb2-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b9cb2-139">Example</span></span>
<span data-ttu-id="b9cb2-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9cb2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9cb2-141">Request</span></span>
<span data-ttu-id="b9cb2-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9cb2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9cb2-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9cb2-144">C#</span><span class="sxs-lookup"><span data-stu-id="b9cb2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9cb2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9cb2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9cb2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9cb2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9cb2-147">Java</span><span class="sxs-lookup"><span data-stu-id="b9cb2-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b9cb2-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9cb2-148">Response</span></span>
<span data-ttu-id="b9cb2-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9cb2-149">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


