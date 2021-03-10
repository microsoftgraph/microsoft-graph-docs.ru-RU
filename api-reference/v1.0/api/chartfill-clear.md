---
title: 'ChartFill: clear'
description: Очищает цвет заливки элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a499cb3d9290734d28d12324f33bfd312cfbef29
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578467"
---
# <a name="chartfill-clear"></a><span data-ttu-id="c4296-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="c4296-103">ChartFill: clear</span></span>

<span data-ttu-id="c4296-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4296-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4296-105">Очищает цвет заливки элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c4296-105">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4296-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4296-106">Permissions</span></span>
<span data-ttu-id="c4296-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4296-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4296-109">Permission type</span></span>      | <span data-ttu-id="c4296-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4296-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4296-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4296-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4296-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4296-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4296-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4296-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4296-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4296-114">Not supported.</span></span>    |
|<span data-ttu-id="c4296-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4296-115">Application</span></span> | <span data-ttu-id="c4296-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4296-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4296-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4296-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="c4296-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4296-118">Request headers</span></span>
| <span data-ttu-id="c4296-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4296-119">Name</span></span>       | <span data-ttu-id="c4296-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4296-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4296-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4296-121">Authorization</span></span>  | <span data-ttu-id="c4296-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4296-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4296-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4296-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4296-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c4296-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4296-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4296-127">Request body</span></span>
<span data-ttu-id="c4296-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4296-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4296-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4296-129">Response</span></span>

<span data-ttu-id="c4296-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c4296-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4296-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c4296-132">Example</span></span>
<span data-ttu-id="c4296-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c4296-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4296-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4296-134">Request</span></span>
<span data-ttu-id="c4296-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4296-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4296-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4296-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```
# <a name="c"></a>[<span data-ttu-id="c4296-137">C#</span><span class="sxs-lookup"><span data-stu-id="c4296-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4296-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4296-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4296-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4296-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4296-140">Java</span><span class="sxs-lookup"><span data-stu-id="c4296-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4296-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4296-141">Response</span></span>
<span data-ttu-id="c4296-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4296-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

