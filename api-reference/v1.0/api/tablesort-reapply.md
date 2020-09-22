---
title: 'TableSort: reapply'
description: Повторно применяет текущие параметры сортировки к таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7a279160b966bca86aea70f376cdd50c3b138441
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032861"
---
# <a name="tablesort-reapply"></a><span data-ttu-id="9b787-103">TableSort: reapply</span><span class="sxs-lookup"><span data-stu-id="9b787-103">TableSort: reapply</span></span>

<span data-ttu-id="9b787-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b787-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b787-105">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="9b787-105">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="9b787-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b787-106">Permissions</span></span>
<span data-ttu-id="9b787-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b787-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b787-109">Permission type</span></span>      | <span data-ttu-id="9b787-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b787-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b787-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b787-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b787-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b787-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b787-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b787-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b787-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b787-114">Not supported.</span></span>    |
|<span data-ttu-id="9b787-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b787-115">Application</span></span> | <span data-ttu-id="9b787-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b787-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b787-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b787-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="9b787-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b787-118">Request headers</span></span>
| <span data-ttu-id="9b787-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9b787-119">Name</span></span>       | <span data-ttu-id="9b787-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9b787-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b787-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b787-121">Authorization</span></span>  | <span data-ttu-id="9b787-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b787-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b787-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9b787-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9b787-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9b787-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b787-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b787-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9b787-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b787-128">Response</span></span>

<span data-ttu-id="9b787-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9b787-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b787-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9b787-131">Example</span></span>
<span data-ttu-id="9b787-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9b787-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b787-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b787-133">Request</span></span>
<span data-ttu-id="9b787-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b787-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b787-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b787-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```
# <a name="c"></a>[<span data-ttu-id="9b787-136">C#</span><span class="sxs-lookup"><span data-stu-id="9b787-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-reapply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b787-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b787-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-reapply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b787-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b787-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-reapply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b787-139">Java</span><span class="sxs-lookup"><span data-stu-id="9b787-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-reapply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9b787-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b787-140">Response</span></span>
<span data-ttu-id="9b787-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b787-141">Here is an example of the response.</span></span> 
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
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

