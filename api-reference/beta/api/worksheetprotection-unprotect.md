---
title: 'Воркбукворкшитпротектион: Unprotect'
description: Снятие защиты с листа
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 89f6017fedb447fb500f51cf07097fc17b27938f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451156"
---
# <a name="workbookworksheetprotection-unprotect"></a><span data-ttu-id="67bd4-103">Воркбукворкшитпротектион: Unprotect</span><span class="sxs-lookup"><span data-stu-id="67bd4-103">workbookWorksheetProtection: unprotect</span></span>

<span data-ttu-id="67bd4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67bd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67bd4-105">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="67bd4-105">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="67bd4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67bd4-106">Permissions</span></span>
<span data-ttu-id="67bd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67bd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67bd4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67bd4-109">Permission type</span></span>      | <span data-ttu-id="67bd4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67bd4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67bd4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67bd4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67bd4-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67bd4-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67bd4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67bd4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67bd4-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67bd4-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67bd4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67bd4-115">Application</span></span> | <span data-ttu-id="67bd4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67bd4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67bd4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67bd4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="67bd4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67bd4-118">Request headers</span></span>
| <span data-ttu-id="67bd4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="67bd4-119">Name</span></span>       | <span data-ttu-id="67bd4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="67bd4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67bd4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67bd4-121">Authorization</span></span>  | <span data-ttu-id="67bd4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67bd4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67bd4-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="67bd4-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="67bd4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="67bd4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67bd4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67bd4-127">Request body</span></span>
<span data-ttu-id="67bd4-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="67bd4-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="67bd4-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="67bd4-129">Parameter</span></span>    | <span data-ttu-id="67bd4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="67bd4-130">Type</span></span>   |<span data-ttu-id="67bd4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="67bd4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67bd4-132">password</span><span class="sxs-lookup"><span data-stu-id="67bd4-132">password</span></span>|<span data-ttu-id="67bd4-133">string</span><span class="sxs-lookup"><span data-stu-id="67bd4-133">string</span></span>|<span data-ttu-id="67bd4-p104">Необязательный пароль защиты листа.</span><span class="sxs-lookup"><span data-stu-id="67bd4-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="67bd4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="67bd4-136">Response</span></span>

<span data-ttu-id="67bd4-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="67bd4-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67bd4-139">Пример</span><span class="sxs-lookup"><span data-stu-id="67bd4-139">Example</span></span>
<span data-ttu-id="67bd4-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="67bd4-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="67bd4-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="67bd4-141">Request</span></span>
<span data-ttu-id="67bd4-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67bd4-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67bd4-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="67bd4-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```
# <a name="c"></a>[<span data-ttu-id="67bd4-144">C#</span><span class="sxs-lookup"><span data-stu-id="67bd4-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67bd4-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67bd4-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67bd4-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67bd4-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="67bd4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="67bd4-147">Response</span></span>
<span data-ttu-id="67bd4-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67bd4-148">Here is an example of the response.</span></span> 
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
  "description": "workbookWorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
