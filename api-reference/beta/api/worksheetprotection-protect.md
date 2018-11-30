---
title: 'WorksheetProtection: protect'
description: Защита листа. Выдает исключение, если лист защищен.
ms.openlocfilehash: 885928c592f6aafe320181e62b3993dfbdadf87e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078359"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="56d2b-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="56d2b-104">WorksheetProtection: protect</span></span>

> <span data-ttu-id="56d2b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56d2b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56d2b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56d2b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56d2b-p103">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="56d2b-p103">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="56d2b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56d2b-109">Permissions</span></span>
<span data-ttu-id="56d2b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d2b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d2b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56d2b-112">Permission type</span></span>      | <span data-ttu-id="56d2b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56d2b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56d2b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56d2b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="56d2b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56d2b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56d2b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56d2b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d2b-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56d2b-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56d2b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56d2b-118">Application</span></span> | <span data-ttu-id="56d2b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56d2b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56d2b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56d2b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="56d2b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56d2b-121">Request headers</span></span>
| <span data-ttu-id="56d2b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="56d2b-122">Name</span></span>       | <span data-ttu-id="56d2b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="56d2b-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56d2b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56d2b-124">Authorization</span></span>  | <span data-ttu-id="56d2b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56d2b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56d2b-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="56d2b-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="56d2b-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="56d2b-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56d2b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56d2b-130">Request body</span></span>
<span data-ttu-id="56d2b-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="56d2b-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56d2b-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="56d2b-132">Parameter</span></span>    | <span data-ttu-id="56d2b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="56d2b-133">Type</span></span>   |<span data-ttu-id="56d2b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="56d2b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56d2b-135">options</span><span class="sxs-lookup"><span data-stu-id="56d2b-135">options</span></span>|<span data-ttu-id="56d2b-136">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="56d2b-136">WorksheetProtectionOptions</span></span>|<span data-ttu-id="56d2b-p107">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="56d2b-p107">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="56d2b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="56d2b-139">Response</span></span>

<span data-ttu-id="56d2b-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="56d2b-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56d2b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="56d2b-142">Example</span></span>
<span data-ttu-id="56d2b-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="56d2b-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="56d2b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="56d2b-144">Request</span></span>
<span data-ttu-id="56d2b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56d2b-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="56d2b-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="56d2b-146">Response</span></span>
<span data-ttu-id="56d2b-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56d2b-147">Here is an example of the response.</span></span> 
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
