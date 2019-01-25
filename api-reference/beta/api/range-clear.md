---
title: 'Range: clear'
description: Очищает формат, заливку, границу, значения диапазона и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 63e468b651b84279ede824796a1ff63acd50c2ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524592"
---
# <a name="range-clear"></a><span data-ttu-id="3abb2-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="3abb2-103">Range: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3abb2-104">Очищает формат, заливку, границу, значения диапазона и т. д.</span><span class="sxs-lookup"><span data-stu-id="3abb2-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="3abb2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3abb2-105">Permissions</span></span>
<span data-ttu-id="3abb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3abb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3abb2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3abb2-108">Permission type</span></span>      | <span data-ttu-id="3abb2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3abb2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3abb2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3abb2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3abb2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3abb2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3abb2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3abb2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3abb2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3abb2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3abb2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3abb2-114">Application</span></span> | <span data-ttu-id="3abb2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3abb2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3abb2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3abb2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="3abb2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3abb2-117">Request headers</span></span>
| <span data-ttu-id="3abb2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3abb2-118">Name</span></span>       | <span data-ttu-id="3abb2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3abb2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3abb2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3abb2-120">Authorization</span></span>  | <span data-ttu-id="3abb2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3abb2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3abb2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3abb2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3abb2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3abb2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3abb2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3abb2-126">Request body</span></span>
<span data-ttu-id="3abb2-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3abb2-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3abb2-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="3abb2-128">Parameter</span></span>    | <span data-ttu-id="3abb2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3abb2-129">Type</span></span>   |<span data-ttu-id="3abb2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3abb2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3abb2-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="3abb2-131">applyTo</span></span>|<span data-ttu-id="3abb2-132">string</span><span class="sxs-lookup"><span data-stu-id="3abb2-132">string</span></span>|<span data-ttu-id="3abb2-p104">Необязательный параметр. Определяет тип действия очистки.  Возможные значения: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="3abb2-p104">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="3abb2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3abb2-136">Response</span></span>

<span data-ttu-id="3abb2-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3abb2-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3abb2-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3abb2-139">Example</span></span>
<span data-ttu-id="3abb2-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3abb2-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3abb2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3abb2-141">Request</span></span>
<span data-ttu-id="3abb2-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3abb2-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="3abb2-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="3abb2-143">Response</span></span>
<span data-ttu-id="3abb2-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3abb2-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
