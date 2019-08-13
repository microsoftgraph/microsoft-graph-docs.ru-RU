---
title: 'Воркбукворкшитпротектион: защита'
description: Защита листа. Выдает исключение, если лист защищен.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 252fc45ec855d40cdd315b092d307675f0c88630
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325717"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="57077-104">Воркбукворкшитпротектион: защита</span><span class="sxs-lookup"><span data-stu-id="57077-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57077-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="57077-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="57077-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57077-107">Permissions</span></span>
<span data-ttu-id="57077-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57077-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57077-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57077-110">Permission type</span></span>      | <span data-ttu-id="57077-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57077-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57077-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57077-112">Delegated (work or school account)</span></span> | <span data-ttu-id="57077-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57077-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57077-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57077-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57077-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57077-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57077-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57077-116">Application</span></span> | <span data-ttu-id="57077-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57077-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57077-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57077-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="57077-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57077-119">Request headers</span></span>
| <span data-ttu-id="57077-120">Имя</span><span class="sxs-lookup"><span data-stu-id="57077-120">Name</span></span>       | <span data-ttu-id="57077-121">Описание</span><span class="sxs-lookup"><span data-stu-id="57077-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57077-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57077-122">Authorization</span></span>  | <span data-ttu-id="57077-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57077-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57077-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="57077-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="57077-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="57077-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57077-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57077-128">Request body</span></span>
<span data-ttu-id="57077-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="57077-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57077-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="57077-130">Parameter</span></span>    | <span data-ttu-id="57077-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57077-131">Type</span></span>   |<span data-ttu-id="57077-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57077-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57077-133">options</span><span class="sxs-lookup"><span data-stu-id="57077-133">options</span></span>|[<span data-ttu-id="57077-134">воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="57077-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="57077-p106">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="57077-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="57077-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="57077-137">Response</span></span>

<span data-ttu-id="57077-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="57077-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57077-140">Пример</span><span class="sxs-lookup"><span data-stu-id="57077-140">Example</span></span>
<span data-ttu-id="57077-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="57077-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57077-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="57077-142">Request</span></span>
<span data-ttu-id="57077-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57077-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="57077-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="57077-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="57077-145">C#</span><span class="sxs-lookup"><span data-stu-id="57077-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57077-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57077-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57077-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="57077-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="57077-148">Java</span><span class="sxs-lookup"><span data-stu-id="57077-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookworksheetprotection-protect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="57077-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="57077-149">Response</span></span>
<span data-ttu-id="57077-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57077-150">Here is an example of the response.</span></span> 
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
