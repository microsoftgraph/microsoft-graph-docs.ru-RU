---
title: 'Table: clearFilters'
description: Очищает все фильтры, примененные к таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 948621a81d105181572c2c7372167de90a4051c8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456962"
---
# <a name="table-clearfilters"></a><span data-ttu-id="791df-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="791df-103">Table: clearFilters</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="791df-104">Очищает все фильтры, примененные к таблице.</span><span class="sxs-lookup"><span data-stu-id="791df-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="791df-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="791df-105">Permissions</span></span>
<span data-ttu-id="791df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="791df-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="791df-108">Permission type</span></span>      | <span data-ttu-id="791df-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="791df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="791df-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="791df-110">Delegated (work or school account)</span></span> | <span data-ttu-id="791df-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="791df-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="791df-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="791df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="791df-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="791df-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="791df-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="791df-114">Application</span></span> | <span data-ttu-id="791df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791df-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="791df-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="791df-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="791df-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="791df-117">Request headers</span></span>
| <span data-ttu-id="791df-118">Имя</span><span class="sxs-lookup"><span data-stu-id="791df-118">Name</span></span>       | <span data-ttu-id="791df-119">Описание</span><span class="sxs-lookup"><span data-stu-id="791df-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="791df-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="791df-120">Authorization</span></span>  | <span data-ttu-id="791df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="791df-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="791df-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="791df-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="791df-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="791df-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="791df-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="791df-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="791df-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="791df-127">Response</span></span>

<span data-ttu-id="791df-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="791df-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="791df-130">Пример</span><span class="sxs-lookup"><span data-stu-id="791df-130">Example</span></span>
<span data-ttu-id="791df-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="791df-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="791df-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="791df-132">Request</span></span>
<span data-ttu-id="791df-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="791df-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="791df-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="791df-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="791df-135">C#</span><span class="sxs-lookup"><span data-stu-id="791df-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-clearfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="791df-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="791df-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-clearfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="791df-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="791df-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-clearfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="791df-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="791df-138">Response</span></span>
<span data-ttu-id="791df-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="791df-139">Here is an example of the response.</span></span> 
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
