---
title: 'Table: reapplyFilters'
description: Повторно применяет все текущие фильтры к таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f652b7eda27fca42341414fb1ea3a76a8e3e20f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024492"
---
# <a name="table-reapplyfilters"></a><span data-ttu-id="7f017-103">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="7f017-103">Table: reapplyFilters</span></span>

<span data-ttu-id="7f017-104">Повторно применяет все текущие фильтры к таблице.</span><span class="sxs-lookup"><span data-stu-id="7f017-104">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f017-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f017-105">Permissions</span></span>
<span data-ttu-id="7f017-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f017-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f017-108">Permission type</span></span>      | <span data-ttu-id="7f017-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f017-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f017-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f017-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f017-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f017-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7f017-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f017-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f017-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f017-113">Not supported.</span></span>    |
|<span data-ttu-id="7f017-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f017-114">Application</span></span> | <span data-ttu-id="7f017-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f017-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f017-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f017-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="7f017-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f017-117">Request headers</span></span>
| <span data-ttu-id="7f017-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7f017-118">Name</span></span>       | <span data-ttu-id="7f017-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7f017-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7f017-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f017-120">Authorization</span></span>  | <span data-ttu-id="7f017-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f017-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f017-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7f017-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7f017-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7f017-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f017-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f017-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7f017-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f017-127">Response</span></span>

<span data-ttu-id="7f017-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7f017-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f017-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7f017-130">Example</span></span>
<span data-ttu-id="7f017-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7f017-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7f017-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f017-132">Request</span></span>
<span data-ttu-id="7f017-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f017-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7f017-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f017-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f017-135">C#</span><span class="sxs-lookup"><span data-stu-id="7f017-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-reapplyfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f017-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f017-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-reapplyfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f017-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7f017-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-reapplyfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7f017-138">Java</span><span class="sxs-lookup"><span data-stu-id="7f017-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-reapplyfilters-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f017-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f017-139">Response</span></span>
<span data-ttu-id="7f017-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7f017-140">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
