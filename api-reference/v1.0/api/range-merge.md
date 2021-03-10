---
title: 'Range: merge'
description: Объединяет ячейки диапазона в одну область на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2ac0ea9456175c929fb1194345536180ee12dd07
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573665"
---
# <a name="range-merge"></a><span data-ttu-id="15ce0-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="15ce0-103">Range: merge</span></span>

<span data-ttu-id="15ce0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15ce0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15ce0-105">Объединяет ячейки диапазона в одну область на листе.</span><span class="sxs-lookup"><span data-stu-id="15ce0-105">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="15ce0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15ce0-106">Permissions</span></span>
<span data-ttu-id="15ce0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ce0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15ce0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15ce0-109">Permission type</span></span>      | <span data-ttu-id="15ce0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15ce0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15ce0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15ce0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="15ce0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ce0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="15ce0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15ce0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ce0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15ce0-114">Not supported.</span></span>    |
|<span data-ttu-id="15ce0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15ce0-115">Application</span></span> | <span data-ttu-id="15ce0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15ce0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15ce0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15ce0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/merge
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/merge
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/merge
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="15ce0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15ce0-118">Request headers</span></span>
| <span data-ttu-id="15ce0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="15ce0-119">Name</span></span>       | <span data-ttu-id="15ce0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="15ce0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="15ce0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15ce0-121">Authorization</span></span>  | <span data-ttu-id="15ce0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15ce0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15ce0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="15ce0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="15ce0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="15ce0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15ce0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15ce0-127">Request body</span></span>
<span data-ttu-id="15ce0-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="15ce0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="15ce0-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="15ce0-129">Parameter</span></span>    | <span data-ttu-id="15ce0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="15ce0-130">Type</span></span>   |<span data-ttu-id="15ce0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="15ce0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15ce0-132">across</span><span class="sxs-lookup"><span data-stu-id="15ce0-132">across</span></span>|<span data-ttu-id="15ce0-133">boolean</span><span class="sxs-lookup"><span data-stu-id="15ce0-133">boolean</span></span>|<span data-ttu-id="15ce0-p104">Необязательный параметр. Установите значение true, чтобы объединить ячейки в каждой строке заданного диапазона как отдельные объединенные ячейки. Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="15ce0-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="15ce0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="15ce0-137">Response</span></span>

<span data-ttu-id="15ce0-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="15ce0-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15ce0-140">Пример</span><span class="sxs-lookup"><span data-stu-id="15ce0-140">Example</span></span>
<span data-ttu-id="15ce0-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="15ce0-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="15ce0-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="15ce0-142">Request</span></span>
<span data-ttu-id="15ce0-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15ce0-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15ce0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="15ce0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```
# <a name="c"></a>[<span data-ttu-id="15ce0-145">C#</span><span class="sxs-lookup"><span data-stu-id="15ce0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-merge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15ce0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15ce0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-merge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15ce0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15ce0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-merge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15ce0-148">Java</span><span class="sxs-lookup"><span data-stu-id="15ce0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-merge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="15ce0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="15ce0-149">Response</span></span>
<span data-ttu-id="15ce0-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15ce0-150">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

