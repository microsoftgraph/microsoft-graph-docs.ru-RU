---
title: 'WorksheetProtection: protect'
description: Защита листа. Выдает исключение, если лист защищен.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a740d2c82e98d2149cb39b11f8fccbe59b6d5823
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455023"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="8cee7-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="8cee7-104">WorksheetProtection: protect</span></span>

<span data-ttu-id="8cee7-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="8cee7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cee7-107">Permissions</span></span>
<span data-ttu-id="8cee7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cee7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cee7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cee7-110">Permission type</span></span>      | <span data-ttu-id="8cee7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cee7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cee7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cee7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8cee7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cee7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8cee7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cee7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cee7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cee7-115">Not supported.</span></span>    |
|<span data-ttu-id="8cee7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cee7-116">Application</span></span> | <span data-ttu-id="8cee7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cee7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cee7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cee7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="8cee7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cee7-119">Request headers</span></span>
| <span data-ttu-id="8cee7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8cee7-120">Name</span></span>       | <span data-ttu-id="8cee7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8cee7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8cee7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cee7-122">Authorization</span></span>  | <span data-ttu-id="8cee7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8cee7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8cee7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8cee7-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cee7-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8cee7-128">Request body</span></span>
<span data-ttu-id="8cee7-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8cee7-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8cee7-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="8cee7-130">Parameter</span></span>    | <span data-ttu-id="8cee7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8cee7-131">Type</span></span>   |<span data-ttu-id="8cee7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8cee7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cee7-133">options</span><span class="sxs-lookup"><span data-stu-id="8cee7-133">options</span></span>|<span data-ttu-id="8cee7-134">Воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="8cee7-134">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="8cee7-p106">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="8cee7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cee7-137">Response</span></span>

<span data-ttu-id="8cee7-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cee7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8cee7-140">Example</span></span>
<span data-ttu-id="8cee7-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8cee7-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8cee7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cee7-142">Request</span></span>
<span data-ttu-id="8cee7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cee7-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8cee7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cee7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8cee7-145">C#</span><span class="sxs-lookup"><span data-stu-id="8cee7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cee7-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="8cee7-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8cee7-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8cee7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8cee7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cee7-148">Response</span></span>
<span data-ttu-id="8cee7-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8cee7-149">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
