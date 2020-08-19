---
title: 'Filter: clear'
description: Сброс фильтра для определенного столбца.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 65ce55da63cc0991b2acfec34c5c38aa34f3e910
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809277"
---
# <a name="filter-clear"></a><span data-ttu-id="786ba-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="786ba-103">Filter: clear</span></span>

<span data-ttu-id="786ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="786ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="786ba-105">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="786ba-105">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="786ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="786ba-106">Permissions</span></span>
<span data-ttu-id="786ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="786ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="786ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="786ba-109">Permission type</span></span>      | <span data-ttu-id="786ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="786ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="786ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="786ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="786ba-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="786ba-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="786ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="786ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="786ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="786ba-114">Not supported.</span></span>    |
|<span data-ttu-id="786ba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="786ba-115">Application</span></span> | <span data-ttu-id="786ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="786ba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="786ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="786ba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="786ba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="786ba-118">Request headers</span></span>
| <span data-ttu-id="786ba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="786ba-119">Name</span></span>       | <span data-ttu-id="786ba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="786ba-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="786ba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="786ba-121">Authorization</span></span>  | <span data-ttu-id="786ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="786ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="786ba-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="786ba-124">Request body</span></span>
<span data-ttu-id="786ba-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="786ba-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="786ba-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="786ba-126">Response</span></span>

<span data-ttu-id="786ba-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="786ba-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="786ba-129">Пример</span><span class="sxs-lookup"><span data-stu-id="786ba-129">Example</span></span>
<span data-ttu-id="786ba-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="786ba-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="786ba-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="786ba-131">Request</span></span>
<span data-ttu-id="786ba-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="786ba-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="786ba-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="786ba-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="c"></a>[<span data-ttu-id="786ba-134">C#</span><span class="sxs-lookup"><span data-stu-id="786ba-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="786ba-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="786ba-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="786ba-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="786ba-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="786ba-137">Java</span><span class="sxs-lookup"><span data-stu-id="786ba-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="786ba-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="786ba-138">Response</span></span>
<span data-ttu-id="786ba-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="786ba-139">Here is an example of the response.</span></span>
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
