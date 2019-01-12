---
title: 'WorksheetProtection: protect'
description: Защита листа. Выдает исключение, если лист защищен.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d72d81b181c6e2fb82df991baaca7c12bb72c721
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930574"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="4d6ab-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="4d6ab-104">WorksheetProtection: protect</span></span>

> <span data-ttu-id="4d6ab-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d6ab-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d6ab-p103">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-p103">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d6ab-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d6ab-109">Permissions</span></span>
<span data-ttu-id="4d6ab-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d6ab-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d6ab-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d6ab-112">Permission type</span></span>      | <span data-ttu-id="4d6ab-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d6ab-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d6ab-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d6ab-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4d6ab-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d6ab-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d6ab-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d6ab-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d6ab-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d6ab-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d6ab-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d6ab-118">Application</span></span> | <span data-ttu-id="4d6ab-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d6ab-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d6ab-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="4d6ab-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d6ab-121">Request headers</span></span>
| <span data-ttu-id="4d6ab-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4d6ab-122">Name</span></span>       | <span data-ttu-id="4d6ab-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4d6ab-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4d6ab-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d6ab-124">Authorization</span></span>  | <span data-ttu-id="4d6ab-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d6ab-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4d6ab-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="4d6ab-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d6ab-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d6ab-130">Request body</span></span>
<span data-ttu-id="4d6ab-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d6ab-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="4d6ab-132">Parameter</span></span>    | <span data-ttu-id="4d6ab-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4d6ab-133">Type</span></span>   |<span data-ttu-id="4d6ab-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4d6ab-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d6ab-135">options</span><span class="sxs-lookup"><span data-stu-id="4d6ab-135">options</span></span>|<span data-ttu-id="4d6ab-136">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="4d6ab-136">WorksheetProtectionOptions</span></span>|<span data-ttu-id="4d6ab-p107">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-p107">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="4d6ab-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d6ab-139">Response</span></span>

<span data-ttu-id="4d6ab-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d6ab-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4d6ab-142">Example</span></span>
<span data-ttu-id="4d6ab-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4d6ab-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d6ab-144">Request</span></span>
<span data-ttu-id="4d6ab-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4d6ab-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d6ab-146">Response</span></span>
<span data-ttu-id="4d6ab-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d6ab-147">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
