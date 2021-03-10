---
title: 'WorksheetProtection: unprotect'
description: Снятие защиты с листа
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dfaf7209037bdbb61e2e487200be9c96b791fa92
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575856"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="06582-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="06582-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="06582-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06582-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06582-105">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="06582-105">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="06582-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06582-106">Permissions</span></span>
<span data-ttu-id="06582-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06582-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06582-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06582-109">Permission type</span></span>      | <span data-ttu-id="06582-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06582-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06582-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06582-111">Delegated (work or school account)</span></span> | <span data-ttu-id="06582-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06582-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="06582-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06582-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06582-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06582-114">Not supported.</span></span>    |
|<span data-ttu-id="06582-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06582-115">Application</span></span> | <span data-ttu-id="06582-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06582-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06582-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06582-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="06582-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06582-118">Request headers</span></span>
| <span data-ttu-id="06582-119">Имя</span><span class="sxs-lookup"><span data-stu-id="06582-119">Name</span></span>       | <span data-ttu-id="06582-120">Описание</span><span class="sxs-lookup"><span data-stu-id="06582-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06582-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06582-121">Authorization</span></span>  | <span data-ttu-id="06582-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06582-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06582-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="06582-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="06582-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="06582-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06582-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06582-127">Request body</span></span>
<span data-ttu-id="06582-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="06582-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06582-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="06582-129">Parameter</span></span>    | <span data-ttu-id="06582-130">Тип</span><span class="sxs-lookup"><span data-stu-id="06582-130">Type</span></span>   |<span data-ttu-id="06582-131">Описание</span><span class="sxs-lookup"><span data-stu-id="06582-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06582-132">password</span><span class="sxs-lookup"><span data-stu-id="06582-132">password</span></span>|<span data-ttu-id="06582-133">string</span><span class="sxs-lookup"><span data-stu-id="06582-133">string</span></span>|<span data-ttu-id="06582-p104">Необязательный пароль защиты листа.</span><span class="sxs-lookup"><span data-stu-id="06582-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="06582-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="06582-136">Response</span></span>

<span data-ttu-id="06582-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="06582-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06582-139">Пример</span><span class="sxs-lookup"><span data-stu-id="06582-139">Example</span></span>
<span data-ttu-id="06582-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="06582-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="06582-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="06582-141">Request</span></span>
<span data-ttu-id="06582-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06582-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06582-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="06582-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="06582-144">C#</span><span class="sxs-lookup"><span data-stu-id="06582-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06582-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06582-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06582-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06582-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06582-147">Java</span><span class="sxs-lookup"><span data-stu-id="06582-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetprotection-unprotect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="06582-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="06582-148">Response</span></span>
<span data-ttu-id="06582-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06582-149">Here is an example of the response.</span></span> 
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

