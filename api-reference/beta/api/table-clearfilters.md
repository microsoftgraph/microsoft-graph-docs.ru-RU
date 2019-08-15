---
title: 'Table: clearFilters'
description: Очищает все фильтры, примененные к таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e0cb6d2da50cdf18bda1a3b8f1b762f91de740d1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409636"
---
# <a name="table-clearfilters"></a><span data-ttu-id="2f1cf-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="2f1cf-103">Table: clearFilters</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f1cf-104">Очищает все фильтры, примененные к таблице.</span><span class="sxs-lookup"><span data-stu-id="2f1cf-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f1cf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f1cf-105">Permissions</span></span>
<span data-ttu-id="2f1cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f1cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f1cf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f1cf-108">Permission type</span></span>      | <span data-ttu-id="2f1cf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f1cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f1cf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f1cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f1cf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f1cf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f1cf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f1cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f1cf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f1cf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f1cf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f1cf-114">Application</span></span> | <span data-ttu-id="2f1cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f1cf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f1cf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f1cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="2f1cf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f1cf-117">Request headers</span></span>
| <span data-ttu-id="2f1cf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2f1cf-118">Name</span></span>       | <span data-ttu-id="2f1cf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2f1cf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f1cf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f1cf-120">Authorization</span></span>  | <span data-ttu-id="2f1cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f1cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f1cf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2f1cf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2f1cf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2f1cf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f1cf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f1cf-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2f1cf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f1cf-127">Response</span></span>

<span data-ttu-id="2f1cf-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2f1cf-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f1cf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2f1cf-130">Example</span></span>
<span data-ttu-id="2f1cf-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2f1cf-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f1cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f1cf-132">Request</span></span>
<span data-ttu-id="2f1cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f1cf-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f1cf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f1cf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f1cf-135">C#</span><span class="sxs-lookup"><span data-stu-id="2f1cf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-clearfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f1cf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f1cf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-clearfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f1cf-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2f1cf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-clearfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f1cf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f1cf-138">Response</span></span>
<span data-ttu-id="2f1cf-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f1cf-139">Here is an example of the response.</span></span> 
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
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
