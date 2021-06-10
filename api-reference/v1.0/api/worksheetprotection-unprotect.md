---
title: 'WorksheetProtection: unprotect'
description: Снятие защиты с листа
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2839649ba773c9e56a0274183ee716c4f2d16d50
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870355"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="d29dd-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="d29dd-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="d29dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d29dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d29dd-105">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="d29dd-105">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="d29dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d29dd-106">Permissions</span></span>
<span data-ttu-id="d29dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d29dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d29dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d29dd-109">Permission type</span></span>      | <span data-ttu-id="d29dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d29dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d29dd-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d29dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d29dd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d29dd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d29dd-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d29dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d29dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d29dd-114">Not supported.</span></span>    |
|<span data-ttu-id="d29dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d29dd-115">Application</span></span> | <span data-ttu-id="d29dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d29dd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d29dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d29dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="d29dd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d29dd-118">Request headers</span></span>
| <span data-ttu-id="d29dd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d29dd-119">Name</span></span>       | <span data-ttu-id="d29dd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d29dd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d29dd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d29dd-121">Authorization</span></span>  | <span data-ttu-id="d29dd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d29dd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d29dd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d29dd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d29dd-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d29dd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d29dd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d29dd-127">Request body</span></span>
<span data-ttu-id="d29dd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d29dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d29dd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d29dd-129">Response</span></span>

<span data-ttu-id="d29dd-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d29dd-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d29dd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d29dd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d29dd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d29dd-133">Request</span></span>
<span data-ttu-id="d29dd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d29dd-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d29dd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d29dd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
```
# <a name="c"></a>[<span data-ttu-id="d29dd-136">C#</span><span class="sxs-lookup"><span data-stu-id="d29dd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d29dd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d29dd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d29dd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d29dd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d29dd-139">Java</span><span class="sxs-lookup"><span data-stu-id="d29dd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetprotection-unprotect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d29dd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d29dd-140">Response</span></span>
<span data-ttu-id="d29dd-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d29dd-141">The following is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

