---
title: 'Range: merge'
description: Объединяет ячейки диапазона в одну область на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b955125367d11848a1d06860812906072abe0925
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454726"
---
# <a name="range-merge"></a><span data-ttu-id="ae14c-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="ae14c-103">Range: merge</span></span>

<span data-ttu-id="ae14c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae14c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae14c-105">Объединяет ячейки диапазона в одну область на листе.</span><span class="sxs-lookup"><span data-stu-id="ae14c-105">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae14c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae14c-106">Permissions</span></span>
<span data-ttu-id="ae14c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae14c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae14c-109">Permission type</span></span>      | <span data-ttu-id="ae14c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae14c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae14c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae14c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae14c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae14c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae14c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae14c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae14c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae14c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae14c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae14c-115">Application</span></span> | <span data-ttu-id="ae14c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae14c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae14c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae14c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="ae14c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae14c-118">Request headers</span></span>
| <span data-ttu-id="ae14c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ae14c-119">Name</span></span>       | <span data-ttu-id="ae14c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae14c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae14c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae14c-121">Authorization</span></span>  | <span data-ttu-id="ae14c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae14c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae14c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ae14c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ae14c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ae14c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae14c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae14c-127">Request body</span></span>
<span data-ttu-id="ae14c-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ae14c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae14c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="ae14c-129">Parameter</span></span>    | <span data-ttu-id="ae14c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ae14c-130">Type</span></span>   |<span data-ttu-id="ae14c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ae14c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae14c-132">across</span><span class="sxs-lookup"><span data-stu-id="ae14c-132">across</span></span>|<span data-ttu-id="ae14c-133">boolean</span><span class="sxs-lookup"><span data-stu-id="ae14c-133">boolean</span></span>|<span data-ttu-id="ae14c-p104">Необязательный параметр. Установите значение true, чтобы объединить ячейки в каждой строке заданного диапазона как отдельные объединенные ячейки. Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="ae14c-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="ae14c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae14c-137">Response</span></span>

<span data-ttu-id="ae14c-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ae14c-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae14c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ae14c-140">Example</span></span>
<span data-ttu-id="ae14c-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ae14c-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae14c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae14c-142">Request</span></span>
<span data-ttu-id="ae14c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae14c-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae14c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae14c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```
# <a name="c"></a>[<span data-ttu-id="ae14c-145">C#</span><span class="sxs-lookup"><span data-stu-id="ae14c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-merge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae14c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae14c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-merge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae14c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae14c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-merge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ae14c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae14c-148">Response</span></span>
<span data-ttu-id="ae14c-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae14c-149">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
