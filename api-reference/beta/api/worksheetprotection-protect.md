---
title: 'Воркбукворкшитпротектион: защита'
description: Защита листа. Выдает исключение, если лист защищен.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b10fa4454b5937c2548e023adfd34900a16c8c95
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339374"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="d1f11-104">Воркбукворкшитпротектион: защита</span><span class="sxs-lookup"><span data-stu-id="d1f11-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1f11-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="d1f11-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1f11-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1f11-107">Permissions</span></span>
<span data-ttu-id="d1f11-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1f11-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1f11-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1f11-110">Permission type</span></span>      | <span data-ttu-id="d1f11-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1f11-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1f11-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1f11-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d1f11-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1f11-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1f11-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1f11-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1f11-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1f11-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1f11-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1f11-116">Application</span></span> | <span data-ttu-id="d1f11-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1f11-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1f11-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1f11-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="d1f11-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1f11-119">Request headers</span></span>
| <span data-ttu-id="d1f11-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d1f11-120">Name</span></span>       | <span data-ttu-id="d1f11-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f11-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1f11-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1f11-122">Authorization</span></span>  | <span data-ttu-id="d1f11-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1f11-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1f11-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d1f11-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d1f11-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d1f11-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1f11-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1f11-128">Request body</span></span>
<span data-ttu-id="d1f11-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d1f11-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1f11-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="d1f11-130">Parameter</span></span>    | <span data-ttu-id="d1f11-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f11-131">Type</span></span>   |<span data-ttu-id="d1f11-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f11-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1f11-133">options</span><span class="sxs-lookup"><span data-stu-id="d1f11-133">options</span></span>|[<span data-ttu-id="d1f11-134">Воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="d1f11-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="d1f11-p106">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="d1f11-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="d1f11-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1f11-137">Response</span></span>

<span data-ttu-id="d1f11-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d1f11-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1f11-140">Пример</span><span class="sxs-lookup"><span data-stu-id="d1f11-140">Example</span></span>
<span data-ttu-id="d1f11-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d1f11-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d1f11-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1f11-142">Request</span></span>
<span data-ttu-id="d1f11-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1f11-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d1f11-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1f11-144">Response</span></span>
<span data-ttu-id="d1f11-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1f11-145">Here is an example of the response.</span></span> 
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
  "suppressions": []
}
-->
