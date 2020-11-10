---
title: 'Filter: clear'
description: Сброс фильтра для определенного столбца.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 8f94d4807b55ecdd00a5d0596b003e2a44b0da1b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965537"
---
# <a name="filter-clear"></a><span data-ttu-id="1e7dc-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="1e7dc-103">Filter: clear</span></span>

<span data-ttu-id="1e7dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e7dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e7dc-105">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="1e7dc-105">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e7dc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e7dc-106">Permissions</span></span>
<span data-ttu-id="1e7dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e7dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e7dc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e7dc-109">Permission type</span></span>      | <span data-ttu-id="1e7dc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e7dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e7dc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e7dc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1e7dc-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e7dc-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e7dc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e7dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e7dc-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e7dc-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e7dc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e7dc-115">Application</span></span> | <span data-ttu-id="1e7dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e7dc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e7dc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e7dc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="1e7dc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e7dc-118">Request headers</span></span>
| <span data-ttu-id="1e7dc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1e7dc-119">Name</span></span>       | <span data-ttu-id="1e7dc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1e7dc-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e7dc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e7dc-121">Authorization</span></span>  | <span data-ttu-id="1e7dc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e7dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e7dc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e7dc-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1e7dc-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e7dc-125">Response</span></span>

<span data-ttu-id="1e7dc-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1e7dc-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e7dc-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1e7dc-128">Example</span></span>
<span data-ttu-id="1e7dc-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1e7dc-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e7dc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e7dc-130">Request</span></span>
<span data-ttu-id="1e7dc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e7dc-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1e7dc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e7dc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="c"></a>[<span data-ttu-id="1e7dc-133">C#</span><span class="sxs-lookup"><span data-stu-id="1e7dc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e7dc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e7dc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e7dc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e7dc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e7dc-136">Java</span><span class="sxs-lookup"><span data-stu-id="1e7dc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1e7dc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e7dc-137">Response</span></span>
<span data-ttu-id="1e7dc-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1e7dc-138">Here is an example of the response.</span></span>
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


