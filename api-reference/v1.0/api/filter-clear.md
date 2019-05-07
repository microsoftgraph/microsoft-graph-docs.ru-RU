---
title: 'Filter: clear'
description: Сброс фильтра для определенного столбца.
localization_priority: Normal
ms.openlocfilehash: 9b796965c14a096a91e4c7dd416a0830bce8ba26
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614623"
---
# <a name="filter-clear"></a><span data-ttu-id="18be9-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="18be9-103">Filter: clear</span></span>

<span data-ttu-id="18be9-104">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="18be9-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="18be9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18be9-105">Permissions</span></span>
<span data-ttu-id="18be9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18be9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18be9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18be9-108">Permission type</span></span>      | <span data-ttu-id="18be9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18be9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18be9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18be9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18be9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="18be9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18be9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18be9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18be9-113">Not supported.</span></span>    |
|<span data-ttu-id="18be9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18be9-114">Application</span></span> | <span data-ttu-id="18be9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18be9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18be9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18be9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="18be9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18be9-117">Request headers</span></span>
| <span data-ttu-id="18be9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="18be9-118">Name</span></span>       | <span data-ttu-id="18be9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="18be9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="18be9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18be9-120">Authorization</span></span>  | <span data-ttu-id="18be9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18be9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18be9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18be9-123">Request body</span></span>
<span data-ttu-id="18be9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18be9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18be9-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="18be9-125">Response</span></span>

<span data-ttu-id="18be9-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="18be9-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18be9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="18be9-128">Example</span></span>
<span data-ttu-id="18be9-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="18be9-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18be9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="18be9-130">Request</span></span>
<span data-ttu-id="18be9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18be9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="18be9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="18be9-132">Response</span></span>
<span data-ttu-id="18be9-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18be9-133">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="18be9-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="18be9-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18be9-135">Языках</span><span class="sxs-lookup"><span data-stu-id="18be9-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/filter_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18be9-136">Язык</span><span class="sxs-lookup"><span data-stu-id="18be9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/filter_clear-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/filter-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/filter-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
