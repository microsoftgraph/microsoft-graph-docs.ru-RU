---
title: 'WorksheetProtection: protect'
description: Защита листа. Выдает исключение, если лист защищен.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 52c7b9a6d3437417e6b8d527d4625e64a9d91cc8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520132"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="7915f-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="7915f-104">WorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7915f-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="7915f-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="7915f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7915f-107">Permissions</span></span>
<span data-ttu-id="7915f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7915f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7915f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7915f-110">Permission type</span></span>      | <span data-ttu-id="7915f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7915f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7915f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7915f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7915f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7915f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7915f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7915f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7915f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7915f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7915f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7915f-116">Application</span></span> | <span data-ttu-id="7915f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7915f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7915f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7915f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="7915f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7915f-119">Request headers</span></span>
| <span data-ttu-id="7915f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7915f-120">Name</span></span>       | <span data-ttu-id="7915f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7915f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7915f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7915f-122">Authorization</span></span>  | <span data-ttu-id="7915f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7915f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7915f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7915f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7915f-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7915f-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7915f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7915f-128">Request body</span></span>
<span data-ttu-id="7915f-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7915f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7915f-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="7915f-130">Parameter</span></span>    | <span data-ttu-id="7915f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7915f-131">Type</span></span>   |<span data-ttu-id="7915f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7915f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7915f-133">options</span><span class="sxs-lookup"><span data-stu-id="7915f-133">options</span></span>|<span data-ttu-id="7915f-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="7915f-134">WorksheetProtectionOptions</span></span>|<span data-ttu-id="7915f-p106">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="7915f-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="7915f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7915f-137">Response</span></span>

<span data-ttu-id="7915f-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7915f-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7915f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7915f-140">Example</span></span>
<span data-ttu-id="7915f-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7915f-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7915f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7915f-142">Request</span></span>
<span data-ttu-id="7915f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7915f-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
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

##### <a name="response"></a><span data-ttu-id="7915f-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="7915f-144">Response</span></span>
<span data-ttu-id="7915f-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7915f-145">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetprotection-protect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
