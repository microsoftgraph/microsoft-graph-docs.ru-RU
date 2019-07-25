---
title: 'Table: clearFilters'
description: Очищает все фильтры, примененные к таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5efbb8338d0fac08a7e91c8bb0dcc4242bc29749
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894293"
---
# <a name="table-clearfilters"></a><span data-ttu-id="ad08d-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="ad08d-103">Table: clearFilters</span></span>

<span data-ttu-id="ad08d-104">Очищает все фильтры, примененные к таблице.</span><span class="sxs-lookup"><span data-stu-id="ad08d-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad08d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad08d-105">Permissions</span></span>
<span data-ttu-id="ad08d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad08d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad08d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad08d-108">Permission type</span></span>      | <span data-ttu-id="ad08d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad08d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad08d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad08d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad08d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad08d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ad08d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad08d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad08d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad08d-113">Not supported.</span></span>    |
|<span data-ttu-id="ad08d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad08d-114">Application</span></span> | <span data-ttu-id="ad08d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad08d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad08d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad08d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="ad08d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad08d-117">Request headers</span></span>
| <span data-ttu-id="ad08d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ad08d-118">Name</span></span>       | <span data-ttu-id="ad08d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ad08d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad08d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad08d-120">Authorization</span></span>  | <span data-ttu-id="ad08d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad08d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad08d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ad08d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ad08d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ad08d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad08d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad08d-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ad08d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad08d-127">Response</span></span>

<span data-ttu-id="ad08d-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ad08d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad08d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ad08d-130">Example</span></span>
<span data-ttu-id="ad08d-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ad08d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ad08d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad08d-132">Request</span></span>
<span data-ttu-id="ad08d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad08d-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad08d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad08d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad08d-135">C#</span><span class="sxs-lookup"><span data-stu-id="ad08d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-clearfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad08d-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad08d-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-clearfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad08d-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ad08d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-clearfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ad08d-138">Java</span><span class="sxs-lookup"><span data-stu-id="ad08d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-clearfilters-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ad08d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad08d-139">Response</span></span>
<span data-ttu-id="ad08d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad08d-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
