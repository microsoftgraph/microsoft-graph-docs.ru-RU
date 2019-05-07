---
title: 'workbookPivotTable: refreshAll'
description: Обновляет сводную таблицу на заданном листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 28d6fc1922844307b0c2871d699e16f225772a81
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636949"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="bcd91-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="bcd91-103">workbookPivotTable: refreshAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcd91-104">Обновляет сводную таблицу на заданном листе.</span><span class="sxs-lookup"><span data-stu-id="bcd91-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcd91-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcd91-105">Permissions</span></span>
<span data-ttu-id="bcd91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcd91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcd91-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcd91-108">Permission type</span></span>      | <span data-ttu-id="bcd91-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcd91-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcd91-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcd91-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bcd91-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcd91-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bcd91-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcd91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcd91-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcd91-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bcd91-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcd91-114">Application</span></span> | <span data-ttu-id="bcd91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcd91-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcd91-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcd91-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="bcd91-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcd91-117">Request headers</span></span>
| <span data-ttu-id="bcd91-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bcd91-118">Name</span></span>       | <span data-ttu-id="bcd91-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bcd91-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bcd91-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcd91-120">Authorization</span></span>  | <span data-ttu-id="bcd91-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcd91-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bcd91-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bcd91-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bcd91-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bcd91-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcd91-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcd91-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bcd91-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcd91-127">Response</span></span>

<span data-ttu-id="bcd91-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bcd91-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcd91-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bcd91-130">Example</span></span>
<span data-ttu-id="bcd91-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bcd91-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bcd91-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcd91-132">Request</span></span>
<span data-ttu-id="bcd91-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcd91-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="bcd91-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcd91-134">Response</span></span>
<span data-ttu-id="bcd91-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bcd91-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bcd91-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="bcd91-136">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="bcd91-137">Языках</span><span class="sxs-lookup"><span data-stu-id="bcd91-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookpivottable_refreshall-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookpivottable-refreshall.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookpivottable-refreshall.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
