---
title: 'WorksheetProtection: unprotect'
description: Снятие защиты с листа
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5061f31674099b9d07a38e02d88fe1f920cc6c18
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026035"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="e01f3-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="e01f3-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="e01f3-104">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="e01f3-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="e01f3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e01f3-105">Permissions</span></span>
<span data-ttu-id="e01f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e01f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e01f3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e01f3-108">Permission type</span></span>      | <span data-ttu-id="e01f3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e01f3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e01f3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e01f3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e01f3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e01f3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e01f3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e01f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e01f3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e01f3-113">Not supported.</span></span>    |
|<span data-ttu-id="e01f3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e01f3-114">Application</span></span> | <span data-ttu-id="e01f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e01f3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e01f3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e01f3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="e01f3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e01f3-117">Request headers</span></span>
| <span data-ttu-id="e01f3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e01f3-118">Name</span></span>       | <span data-ttu-id="e01f3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e01f3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e01f3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e01f3-120">Authorization</span></span>  | <span data-ttu-id="e01f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e01f3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e01f3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e01f3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e01f3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e01f3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e01f3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e01f3-126">Request body</span></span>
<span data-ttu-id="e01f3-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e01f3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e01f3-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="e01f3-128">Parameter</span></span>    | <span data-ttu-id="e01f3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e01f3-129">Type</span></span>   |<span data-ttu-id="e01f3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e01f3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e01f3-131">password</span><span class="sxs-lookup"><span data-stu-id="e01f3-131">password</span></span>|<span data-ttu-id="e01f3-132">string</span><span class="sxs-lookup"><span data-stu-id="e01f3-132">string</span></span>|<span data-ttu-id="e01f3-p104">Необязательный пароль защиты листа.</span><span class="sxs-lookup"><span data-stu-id="e01f3-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="e01f3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e01f3-135">Response</span></span>

<span data-ttu-id="e01f3-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e01f3-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e01f3-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e01f3-138">Example</span></span>
<span data-ttu-id="e01f3-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e01f3-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e01f3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e01f3-140">Request</span></span>
<span data-ttu-id="e01f3-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e01f3-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e01f3-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e01f3-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e01f3-143">C#</span><span class="sxs-lookup"><span data-stu-id="e01f3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e01f3-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="e01f3-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e01f3-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e01f3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e01f3-146">Java</span><span class="sxs-lookup"><span data-stu-id="e01f3-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetprotection-unprotect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e01f3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e01f3-147">Response</span></span>
<span data-ttu-id="e01f3-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e01f3-148">Here is an example of the response.</span></span> 
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
