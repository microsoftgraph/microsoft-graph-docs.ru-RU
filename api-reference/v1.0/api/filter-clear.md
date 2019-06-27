---
title: 'Filter: clear'
description: Сброс фильтра для определенного столбца.
localization_priority: Normal
ms.openlocfilehash: 2d33e4e25fa2593dadd4792e2d6fb9b1d39cffe8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275910"
---
# <a name="filter-clear"></a><span data-ttu-id="54071-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="54071-103">Filter: clear</span></span>

<span data-ttu-id="54071-104">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="54071-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="54071-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54071-105">Permissions</span></span>
<span data-ttu-id="54071-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54071-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54071-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54071-108">Permission type</span></span>      | <span data-ttu-id="54071-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54071-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54071-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54071-110">Delegated (work or school account)</span></span> | <span data-ttu-id="54071-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54071-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="54071-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54071-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54071-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54071-113">Not supported.</span></span>    |
|<span data-ttu-id="54071-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54071-114">Application</span></span> | <span data-ttu-id="54071-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54071-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54071-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54071-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="54071-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54071-117">Request headers</span></span>
| <span data-ttu-id="54071-118">Имя</span><span class="sxs-lookup"><span data-stu-id="54071-118">Name</span></span>       | <span data-ttu-id="54071-119">Описание</span><span class="sxs-lookup"><span data-stu-id="54071-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="54071-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54071-120">Authorization</span></span>  | <span data-ttu-id="54071-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54071-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54071-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54071-123">Request body</span></span>
<span data-ttu-id="54071-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54071-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54071-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="54071-125">Response</span></span>

<span data-ttu-id="54071-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="54071-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54071-128">Пример</span><span class="sxs-lookup"><span data-stu-id="54071-128">Example</span></span>
<span data-ttu-id="54071-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="54071-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="54071-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="54071-130">Request</span></span>
<span data-ttu-id="54071-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54071-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="54071-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="54071-132">Response</span></span>
<span data-ttu-id="54071-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54071-133">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="54071-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="54071-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="54071-135">C#</span><span class="sxs-lookup"><span data-stu-id="54071-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/filter_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54071-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="54071-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/filter_clear-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="54071-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="54071-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/filter_clear-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/filter-clear.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/filter-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/filter-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
