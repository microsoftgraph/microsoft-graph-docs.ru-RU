---
title: 'Range: delete'
description: Удаляет ячейки, связанные с диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a3183e393d66c75afd05ccc2226e5217dd6b4a23
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574001"
---
# <a name="range-delete"></a><span data-ttu-id="bba9d-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="bba9d-103">Range: delete</span></span>

<span data-ttu-id="bba9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bba9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bba9d-105">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="bba9d-105">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="bba9d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bba9d-106">Permissions</span></span>
<span data-ttu-id="bba9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bba9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bba9d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bba9d-109">Permission type</span></span>      | <span data-ttu-id="bba9d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bba9d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bba9d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bba9d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bba9d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bba9d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bba9d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bba9d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bba9d-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bba9d-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bba9d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bba9d-115">Application</span></span> | <span data-ttu-id="bba9d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bba9d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bba9d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bba9d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/delete
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/delete
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/delete
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="bba9d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bba9d-118">Request headers</span></span>
| <span data-ttu-id="bba9d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bba9d-119">Name</span></span>       | <span data-ttu-id="bba9d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bba9d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bba9d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bba9d-121">Authorization</span></span>  | <span data-ttu-id="bba9d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bba9d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bba9d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bba9d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="bba9d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bba9d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bba9d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bba9d-127">Request body</span></span>
<span data-ttu-id="bba9d-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bba9d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bba9d-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="bba9d-129">Parameter</span></span>    | <span data-ttu-id="bba9d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bba9d-130">Type</span></span>   |<span data-ttu-id="bba9d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bba9d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bba9d-132">shift</span><span class="sxs-lookup"><span data-stu-id="bba9d-132">shift</span></span>|<span data-ttu-id="bba9d-133">string</span><span class="sxs-lookup"><span data-stu-id="bba9d-133">string</span></span>|<span data-ttu-id="bba9d-p104">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="bba9d-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="bba9d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bba9d-136">Response</span></span>

<span data-ttu-id="bba9d-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bba9d-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bba9d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="bba9d-139">Example</span></span>
<span data-ttu-id="bba9d-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bba9d-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bba9d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bba9d-141">Request</span></span>
<span data-ttu-id="bba9d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bba9d-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bba9d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="bba9d-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bba9d-144">C#</span><span class="sxs-lookup"><span data-stu-id="bba9d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bba9d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bba9d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bba9d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bba9d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bba9d-147">Java</span><span class="sxs-lookup"><span data-stu-id="bba9d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bba9d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="bba9d-148">Response</span></span>
<span data-ttu-id="bba9d-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bba9d-149">Here is an example of the response.</span></span> 
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


