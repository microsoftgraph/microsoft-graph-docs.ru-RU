---
title: 'RangeFill: clear'
description: Сбрасывает фон диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d149f550ef3ebb00848b978da2e042ef593e906b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576690"
---
# <a name="rangefill-clear"></a><span data-ttu-id="d1f83-103">RangeFill: clear</span><span class="sxs-lookup"><span data-stu-id="d1f83-103">RangeFill: clear</span></span>

<span data-ttu-id="d1f83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1f83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1f83-105">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="d1f83-105">Resets the range background.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1f83-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1f83-106">Permissions</span></span>
<span data-ttu-id="d1f83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1f83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1f83-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1f83-109">Permission type</span></span>      | <span data-ttu-id="d1f83-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1f83-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1f83-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1f83-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d1f83-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1f83-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1f83-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1f83-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1f83-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1f83-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1f83-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1f83-115">Application</span></span> | <span data-ttu-id="d1f83-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1f83-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1f83-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1f83-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/fill/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/fill/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/fill/clear
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/fill/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="d1f83-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1f83-118">Request headers</span></span>
| <span data-ttu-id="d1f83-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d1f83-119">Name</span></span>       | <span data-ttu-id="d1f83-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f83-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1f83-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1f83-121">Authorization</span></span>  | <span data-ttu-id="d1f83-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1f83-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1f83-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d1f83-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d1f83-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d1f83-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1f83-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1f83-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d1f83-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1f83-128">Response</span></span>

<span data-ttu-id="d1f83-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d1f83-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1f83-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d1f83-131">Example</span></span>
<span data-ttu-id="d1f83-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d1f83-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d1f83-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1f83-133">Request</span></span>
<span data-ttu-id="d1f83-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1f83-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1f83-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1f83-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangefill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear
```
# <a name="c"></a>[<span data-ttu-id="d1f83-136">C#</span><span class="sxs-lookup"><span data-stu-id="d1f83-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangefill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1f83-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1f83-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangefill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1f83-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1f83-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangefill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1f83-139">Java</span><span class="sxs-lookup"><span data-stu-id="d1f83-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangefill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d1f83-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1f83-140">Response</span></span>
<span data-ttu-id="d1f83-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1f83-141">Here is an example of the response.</span></span> 
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
  "description": "RangeFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


