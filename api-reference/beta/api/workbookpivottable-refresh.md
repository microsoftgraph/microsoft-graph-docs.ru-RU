---
title: 'workbookPivotTable: refresh'
description: Обновляет сводную таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 523aecab7e17330f26142c19bf3df42d4c255c1d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787711"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="b7b89-103">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="b7b89-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="b7b89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7b89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b89-105">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="b7b89-105">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="b7b89-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7b89-106">Permissions</span></span>
<span data-ttu-id="b7b89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7b89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b7b89-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7b89-109">Permission type</span></span>      | <span data-ttu-id="b7b89-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7b89-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7b89-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7b89-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7b89-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7b89-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7b89-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7b89-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7b89-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7b89-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7b89-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7b89-115">Application</span></span> | <span data-ttu-id="b7b89-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7b89-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7b89-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7b89-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id}/pivotTables/{id}/refresh
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="b7b89-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7b89-118">Request headers</span></span>
| <span data-ttu-id="b7b89-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b7b89-119">Name</span></span>       | <span data-ttu-id="b7b89-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b7b89-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7b89-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7b89-121">Authorization</span></span>  | <span data-ttu-id="b7b89-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7b89-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7b89-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b7b89-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b7b89-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b7b89-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7b89-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7b89-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b7b89-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7b89-128">Response</span></span>

<span data-ttu-id="b7b89-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b7b89-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7b89-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b7b89-131">Example</span></span>
<span data-ttu-id="b7b89-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b7b89-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7b89-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7b89-133">Request</span></span>
<span data-ttu-id="b7b89-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7b89-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7b89-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b89-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
# <a name="c"></a>[<span data-ttu-id="b7b89-136">C#</span><span class="sxs-lookup"><span data-stu-id="b7b89-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refresh-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7b89-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7b89-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refresh-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7b89-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7b89-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refresh-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7b89-139">Java</span><span class="sxs-lookup"><span data-stu-id="b7b89-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refresh-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b7b89-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7b89-140">Response</span></span>
<span data-ttu-id="b7b89-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7b89-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


