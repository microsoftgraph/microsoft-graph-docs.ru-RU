---
title: 'Воркбукворкшитпротектион: защита'
description: Защита листа. Выдает исключение, если лист защищен.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0d097adb2c00a54c6072d2742b7cdaa012144309
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456024"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="5e662-104">Воркбукворкшитпротектион: защита</span><span class="sxs-lookup"><span data-stu-id="5e662-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e662-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="5e662-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e662-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e662-107">Permissions</span></span>
<span data-ttu-id="5e662-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e662-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e662-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e662-110">Permission type</span></span>      | <span data-ttu-id="5e662-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e662-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e662-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e662-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5e662-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e662-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e662-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e662-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e662-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e662-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e662-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e662-116">Application</span></span> | <span data-ttu-id="5e662-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e662-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e662-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e662-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="5e662-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e662-119">Request headers</span></span>
| <span data-ttu-id="5e662-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5e662-120">Name</span></span>       | <span data-ttu-id="5e662-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5e662-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5e662-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e662-122">Authorization</span></span>  | <span data-ttu-id="5e662-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e662-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e662-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5e662-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5e662-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5e662-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e662-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e662-128">Request body</span></span>
<span data-ttu-id="5e662-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5e662-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e662-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="5e662-130">Parameter</span></span>    | <span data-ttu-id="5e662-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5e662-131">Type</span></span>   |<span data-ttu-id="5e662-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5e662-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e662-133">options</span><span class="sxs-lookup"><span data-stu-id="5e662-133">options</span></span>|[<span data-ttu-id="5e662-134">Воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="5e662-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="5e662-p106">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="5e662-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="5e662-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e662-137">Response</span></span>

<span data-ttu-id="5e662-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5e662-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e662-140">Пример</span><span class="sxs-lookup"><span data-stu-id="5e662-140">Example</span></span>
<span data-ttu-id="5e662-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5e662-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5e662-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e662-142">Request</span></span>
<span data-ttu-id="5e662-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e662-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5e662-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e662-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e662-145">C#</span><span class="sxs-lookup"><span data-stu-id="5e662-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e662-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="5e662-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e662-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5e662-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5e662-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e662-148">Response</span></span>
<span data-ttu-id="5e662-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e662-149">Here is an example of the response.</span></span> 
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
  "description": "workbookWorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
