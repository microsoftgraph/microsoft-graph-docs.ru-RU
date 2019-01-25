---
title: 'WorksheetProtection: unprotect'
description: Снятие защиты с листа
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9fe503034e2d54dd1df7282c2c0e5fa0819bfdfd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515246"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="19b51-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="19b51-103">WorksheetProtection: unprotect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19b51-104">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="19b51-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="19b51-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19b51-105">Permissions</span></span>
<span data-ttu-id="19b51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19b51-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19b51-108">Permission type</span></span>      | <span data-ttu-id="19b51-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19b51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19b51-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19b51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19b51-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19b51-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19b51-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19b51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19b51-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19b51-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19b51-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19b51-114">Application</span></span> | <span data-ttu-id="19b51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b51-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19b51-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19b51-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="19b51-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19b51-117">Request headers</span></span>
| <span data-ttu-id="19b51-118">Имя</span><span class="sxs-lookup"><span data-stu-id="19b51-118">Name</span></span>       | <span data-ttu-id="19b51-119">Описание</span><span class="sxs-lookup"><span data-stu-id="19b51-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19b51-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19b51-120">Authorization</span></span>  | <span data-ttu-id="19b51-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19b51-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19b51-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="19b51-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="19b51-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="19b51-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19b51-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19b51-126">Request body</span></span>
<span data-ttu-id="19b51-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="19b51-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19b51-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="19b51-128">Parameter</span></span>    | <span data-ttu-id="19b51-129">Тип</span><span class="sxs-lookup"><span data-stu-id="19b51-129">Type</span></span>   |<span data-ttu-id="19b51-130">Описание</span><span class="sxs-lookup"><span data-stu-id="19b51-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19b51-131">password</span><span class="sxs-lookup"><span data-stu-id="19b51-131">password</span></span>|<span data-ttu-id="19b51-132">string</span><span class="sxs-lookup"><span data-stu-id="19b51-132">string</span></span>|<span data-ttu-id="19b51-p104">Необязательный пароль защиты листа.</span><span class="sxs-lookup"><span data-stu-id="19b51-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="19b51-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="19b51-135">Response</span></span>

<span data-ttu-id="19b51-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="19b51-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b51-138">Пример</span><span class="sxs-lookup"><span data-stu-id="19b51-138">Example</span></span>
<span data-ttu-id="19b51-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="19b51-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19b51-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="19b51-140">Request</span></span>
<span data-ttu-id="19b51-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19b51-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="19b51-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="19b51-142">Response</span></span>
<span data-ttu-id="19b51-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19b51-143">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetprotection-unprotect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
