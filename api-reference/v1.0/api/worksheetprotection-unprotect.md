---
title: 'WorksheetProtection: unprotect'
description: Снятие защиты с листа
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 69c5d8f9d8be793565fe6f93e553e88dc2df5dfa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278241"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="76046-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="76046-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="76046-104">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="76046-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="76046-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76046-105">Permissions</span></span>
<span data-ttu-id="76046-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76046-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76046-108">Permission type</span></span>      | <span data-ttu-id="76046-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76046-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76046-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76046-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76046-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76046-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="76046-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76046-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76046-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76046-113">Not supported.</span></span>    |
|<span data-ttu-id="76046-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76046-114">Application</span></span> | <span data-ttu-id="76046-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76046-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76046-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76046-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="76046-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76046-117">Request headers</span></span>
| <span data-ttu-id="76046-118">Имя</span><span class="sxs-lookup"><span data-stu-id="76046-118">Name</span></span>       | <span data-ttu-id="76046-119">Описание</span><span class="sxs-lookup"><span data-stu-id="76046-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="76046-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76046-120">Authorization</span></span>  | <span data-ttu-id="76046-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76046-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76046-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="76046-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="76046-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="76046-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76046-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76046-126">Request body</span></span>
<span data-ttu-id="76046-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="76046-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76046-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="76046-128">Parameter</span></span>    | <span data-ttu-id="76046-129">Тип</span><span class="sxs-lookup"><span data-stu-id="76046-129">Type</span></span>   |<span data-ttu-id="76046-130">Описание</span><span class="sxs-lookup"><span data-stu-id="76046-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76046-131">password</span><span class="sxs-lookup"><span data-stu-id="76046-131">password</span></span>|<span data-ttu-id="76046-132">string</span><span class="sxs-lookup"><span data-stu-id="76046-132">string</span></span>|<span data-ttu-id="76046-p104">Необязательный пароль защиты листа.</span><span class="sxs-lookup"><span data-stu-id="76046-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="76046-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="76046-135">Response</span></span>

<span data-ttu-id="76046-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="76046-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76046-138">Пример</span><span class="sxs-lookup"><span data-stu-id="76046-138">Example</span></span>
<span data-ttu-id="76046-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="76046-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76046-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="76046-140">Request</span></span>
<span data-ttu-id="76046-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76046-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="76046-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="76046-142">Response</span></span>
<span data-ttu-id="76046-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="76046-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="76046-144">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="76046-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="76046-145">C#</span><span class="sxs-lookup"><span data-stu-id="76046-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheetprotection_unprotect-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76046-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="76046-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheetprotection_unprotect-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="76046-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="76046-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheetprotection_unprotect-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheetprotection-unprotect.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/worksheetprotection-unprotect.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheetprotection-unprotect.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
