---
title: 'Воркбукворкшитпротектион: защита'
description: Защита листа. Выдает исключение, если лист защищен.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 36cf3c9ac26331953464062b59e21c3b31a102e6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269687"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="ff32d-104">Воркбукворкшитпротектион: защита</span><span class="sxs-lookup"><span data-stu-id="ff32d-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff32d-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="ff32d-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff32d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff32d-107">Permissions</span></span>
<span data-ttu-id="ff32d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff32d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff32d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff32d-110">Permission type</span></span>      | <span data-ttu-id="ff32d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff32d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff32d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff32d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff32d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff32d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff32d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff32d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff32d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff32d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff32d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff32d-116">Application</span></span> | <span data-ttu-id="ff32d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff32d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff32d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff32d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="ff32d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff32d-119">Request headers</span></span>
| <span data-ttu-id="ff32d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ff32d-120">Name</span></span>       | <span data-ttu-id="ff32d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ff32d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ff32d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff32d-122">Authorization</span></span>  | <span data-ttu-id="ff32d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff32d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff32d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ff32d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ff32d-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ff32d-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff32d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff32d-128">Request body</span></span>
<span data-ttu-id="ff32d-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ff32d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ff32d-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ff32d-130">Parameter</span></span>    | <span data-ttu-id="ff32d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff32d-131">Type</span></span>   |<span data-ttu-id="ff32d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff32d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff32d-133">options</span><span class="sxs-lookup"><span data-stu-id="ff32d-133">options</span></span>|[<span data-ttu-id="ff32d-134">Воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="ff32d-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="ff32d-p106">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="ff32d-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="ff32d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff32d-137">Response</span></span>

<span data-ttu-id="ff32d-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ff32d-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff32d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ff32d-140">Example</span></span>
<span data-ttu-id="ff32d-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ff32d-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff32d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff32d-142">Request</span></span>
<span data-ttu-id="ff32d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff32d-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ff32d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff32d-144">Response</span></span>
<span data-ttu-id="ff32d-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ff32d-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ff32d-146">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ff32d-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ff32d-147">C#</span><span class="sxs-lookup"><span data-stu-id="ff32d-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookworksheetprotection_protect-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff32d-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff32d-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookworksheetprotection_protect-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ff32d-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ff32d-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookworksheetprotection_protect-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/worksheetprotection-protect.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/worksheetprotection-protect.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/worksheetprotection-protect.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
