---
title: 'workbookWorksheetProtection: защита'
description: Защита листа. Выдает исключение, если лист защищен.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bfbb6252a13db3afb3cab4f3b21bb947897cd297
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578096"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="0752b-104">workbookWorksheetProtection: защита</span><span class="sxs-lookup"><span data-stu-id="0752b-104">workbookWorksheetProtection: protect</span></span>

<span data-ttu-id="0752b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0752b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0752b-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="0752b-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="0752b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0752b-108">Permissions</span></span>
<span data-ttu-id="0752b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0752b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0752b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0752b-111">Permission type</span></span>      | <span data-ttu-id="0752b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0752b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0752b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0752b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0752b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0752b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0752b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0752b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0752b-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0752b-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0752b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0752b-117">Application</span></span> | <span data-ttu-id="0752b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0752b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0752b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0752b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="0752b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0752b-120">Request headers</span></span>
| <span data-ttu-id="0752b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0752b-121">Name</span></span>       | <span data-ttu-id="0752b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0752b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0752b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0752b-123">Authorization</span></span>  | <span data-ttu-id="0752b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0752b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0752b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0752b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="0752b-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0752b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0752b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0752b-129">Request body</span></span>
<span data-ttu-id="0752b-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0752b-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0752b-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="0752b-131">Parameter</span></span>    | <span data-ttu-id="0752b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0752b-132">Type</span></span>   |<span data-ttu-id="0752b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0752b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0752b-134">options</span><span class="sxs-lookup"><span data-stu-id="0752b-134">options</span></span>|[<span data-ttu-id="0752b-135">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="0752b-135">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="0752b-p106">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="0752b-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="0752b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0752b-138">Response</span></span>

<span data-ttu-id="0752b-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0752b-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0752b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="0752b-141">Example</span></span>
<span data-ttu-id="0752b-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0752b-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0752b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="0752b-143">Request</span></span>
<span data-ttu-id="0752b-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0752b-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0752b-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0752b-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0752b-146">C#</span><span class="sxs-lookup"><span data-stu-id="0752b-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0752b-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0752b-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0752b-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0752b-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0752b-149">Java</span><span class="sxs-lookup"><span data-stu-id="0752b-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookworksheetprotection-protect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0752b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0752b-150">Response</span></span>
<span data-ttu-id="0752b-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0752b-151">Here is an example of the response.</span></span> 
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


