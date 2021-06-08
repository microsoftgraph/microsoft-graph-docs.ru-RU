---
title: 'Table: delete'
description: Удаляет таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3a8f6b637d46a7cc10d026da942c33444b643845
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786715"
---
# <a name="table-delete"></a><span data-ttu-id="2ba31-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="2ba31-103">Table: delete</span></span>

<span data-ttu-id="2ba31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba31-105">Удаляет таблицу.</span><span class="sxs-lookup"><span data-stu-id="2ba31-105">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ba31-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ba31-106">Permissions</span></span>
<span data-ttu-id="2ba31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ba31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ba31-109">Permission type</span></span>      | <span data-ttu-id="2ba31-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ba31-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ba31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ba31-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ba31-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ba31-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ba31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ba31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ba31-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ba31-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ba31-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ba31-115">Application</span></span> | <span data-ttu-id="2ba31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ba31-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ba31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ba31-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/tables/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/tables/{id|name}
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="2ba31-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ba31-118">Request headers</span></span>
| <span data-ttu-id="2ba31-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ba31-119">Name</span></span>       | <span data-ttu-id="2ba31-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba31-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ba31-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ba31-121">Authorization</span></span>  | <span data-ttu-id="2ba31-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ba31-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ba31-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2ba31-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ba31-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2ba31-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ba31-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ba31-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2ba31-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba31-128">Response</span></span>

<span data-ttu-id="2ba31-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2ba31-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ba31-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2ba31-131">Example</span></span>
<span data-ttu-id="2ba31-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2ba31-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ba31-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ba31-133">Request</span></span>
<span data-ttu-id="2ba31-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ba31-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ba31-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba31-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="2ba31-136">C#</span><span class="sxs-lookup"><span data-stu-id="2ba31-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ba31-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ba31-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ba31-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ba31-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ba31-139">Java</span><span class="sxs-lookup"><span data-stu-id="2ba31-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2ba31-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba31-140">Response</span></span>
<span data-ttu-id="2ba31-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ba31-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


