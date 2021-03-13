---
title: 'Table: delete'
description: Удаляет таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9ad6a27bdf7cceedf0f53cb68f253e8292f7dd96
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775404"
---
# <a name="table-delete"></a><span data-ttu-id="0e138-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="0e138-103">Table: delete</span></span>

<span data-ttu-id="0e138-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e138-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e138-105">Удаляет таблицу.</span><span class="sxs-lookup"><span data-stu-id="0e138-105">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e138-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e138-106">Permissions</span></span>
<span data-ttu-id="0e138-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e138-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e138-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e138-109">Permission type</span></span>      | <span data-ttu-id="0e138-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e138-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e138-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e138-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e138-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e138-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e138-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e138-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e138-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e138-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e138-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e138-115">Application</span></span> | <span data-ttu-id="0e138-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e138-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e138-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e138-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/tables/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/tables/{id|name}
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="0e138-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e138-118">Request headers</span></span>
| <span data-ttu-id="0e138-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0e138-119">Name</span></span>       | <span data-ttu-id="0e138-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0e138-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e138-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e138-121">Authorization</span></span>  | <span data-ttu-id="0e138-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e138-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e138-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e138-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e138-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0e138-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e138-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e138-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0e138-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e138-128">Response</span></span>

<span data-ttu-id="0e138-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0e138-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e138-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0e138-131">Example</span></span>
<span data-ttu-id="0e138-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0e138-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e138-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e138-133">Request</span></span>
<span data-ttu-id="0e138-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e138-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e138-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e138-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="0e138-136">C#</span><span class="sxs-lookup"><span data-stu-id="0e138-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e138-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e138-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e138-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e138-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e138-139">Java</span><span class="sxs-lookup"><span data-stu-id="0e138-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e138-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e138-140">Response</span></span>
<span data-ttu-id="0e138-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e138-141">Here is an example of the response.</span></span> 
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
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


