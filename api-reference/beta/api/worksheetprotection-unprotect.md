---
title: 'workbookWorksheetProtection: unprotect'
description: Снятие защиты с листа
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7e827b1610525d096af149648cd5fecde2996389
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869711"
---
# <a name="workbookworksheetprotection-unprotect"></a><span data-ttu-id="9dc25-103">workbookWorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="9dc25-103">workbookWorksheetProtection: unprotect</span></span>

<span data-ttu-id="9dc25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dc25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dc25-105">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="9dc25-105">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="9dc25-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9dc25-106">Permissions</span></span>
<span data-ttu-id="9dc25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dc25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dc25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dc25-109">Permission type</span></span>      | <span data-ttu-id="9dc25-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dc25-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dc25-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dc25-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9dc25-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dc25-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9dc25-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dc25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dc25-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dc25-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9dc25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dc25-115">Application</span></span> | <span data-ttu-id="9dc25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dc25-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dc25-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dc25-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="9dc25-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dc25-118">Request headers</span></span>
| <span data-ttu-id="9dc25-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9dc25-119">Name</span></span>       | <span data-ttu-id="9dc25-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc25-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9dc25-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dc25-121">Authorization</span></span>  | <span data-ttu-id="9dc25-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dc25-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9dc25-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9dc25-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9dc25-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9dc25-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dc25-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9dc25-127">Request body</span></span>
<span data-ttu-id="9dc25-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9dc25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dc25-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dc25-129">Response</span></span>

<span data-ttu-id="9dc25-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9dc25-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dc25-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9dc25-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dc25-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dc25-133">Request</span></span>
<span data-ttu-id="9dc25-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dc25-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9dc25-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dc25-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
```
# <a name="c"></a>[<span data-ttu-id="9dc25-136">C#</span><span class="sxs-lookup"><span data-stu-id="9dc25-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dc25-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dc25-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dc25-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dc25-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dc25-139">Java</span><span class="sxs-lookup"><span data-stu-id="9dc25-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookworksheetprotection-unprotect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9dc25-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dc25-140">Response</span></span>
<span data-ttu-id="9dc25-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9dc25-141">The following is an example of the response.</span></span> 
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
  "description": "workbookWorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


