---
title: 'Filter: clear'
description: Сброс фильтра для определенного столбца.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: bd9368e8c3b773e412ce6ebfdb78dce23d06428a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325227"
---
# <a name="filter-clear"></a><span data-ttu-id="8c382-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="8c382-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c382-104">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="8c382-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c382-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c382-105">Permissions</span></span>
<span data-ttu-id="8c382-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c382-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c382-108">Permission type</span></span>      | <span data-ttu-id="8c382-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c382-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c382-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c382-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c382-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c382-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c382-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c382-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c382-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c382-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c382-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c382-114">Application</span></span> | <span data-ttu-id="8c382-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c382-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c382-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c382-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="8c382-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c382-117">Request headers</span></span>
| <span data-ttu-id="8c382-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8c382-118">Name</span></span>       | <span data-ttu-id="8c382-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8c382-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c382-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c382-120">Authorization</span></span>  | <span data-ttu-id="8c382-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c382-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c382-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c382-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8c382-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c382-124">Response</span></span>

<span data-ttu-id="8c382-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8c382-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c382-127">Пример</span><span class="sxs-lookup"><span data-stu-id="8c382-127">Example</span></span>
<span data-ttu-id="8c382-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8c382-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c382-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c382-129">Request</span></span>
<span data-ttu-id="8c382-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c382-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c382-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c382-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c382-132">C#</span><span class="sxs-lookup"><span data-stu-id="8c382-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c382-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c382-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c382-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8c382-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c382-135">Java</span><span class="sxs-lookup"><span data-stu-id="8c382-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8c382-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c382-136">Response</span></span>
<span data-ttu-id="8c382-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c382-137">Here is an example of the response.</span></span> 
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
