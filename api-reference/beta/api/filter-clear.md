---
title: 'Filter: clear'
description: Сброс фильтра для определенного столбца.
localization_priority: Normal
ms.openlocfilehash: 2bc1d1f607f062ca7566189d184f37bc74ab09df
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440864"
---
# <a name="filter-clear"></a><span data-ttu-id="42bbf-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="42bbf-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42bbf-104">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="42bbf-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="42bbf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42bbf-105">Permissions</span></span>
<span data-ttu-id="42bbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42bbf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42bbf-108">Permission type</span></span>      | <span data-ttu-id="42bbf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42bbf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42bbf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42bbf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42bbf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42bbf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42bbf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42bbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42bbf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42bbf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42bbf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42bbf-114">Application</span></span> | <span data-ttu-id="42bbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42bbf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42bbf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42bbf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="42bbf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42bbf-117">Request headers</span></span>
| <span data-ttu-id="42bbf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="42bbf-118">Name</span></span>       | <span data-ttu-id="42bbf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="42bbf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42bbf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42bbf-120">Authorization</span></span>  | <span data-ttu-id="42bbf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42bbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42bbf-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42bbf-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="42bbf-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="42bbf-124">Response</span></span>

<span data-ttu-id="42bbf-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="42bbf-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42bbf-127">Пример</span><span class="sxs-lookup"><span data-stu-id="42bbf-127">Example</span></span>
<span data-ttu-id="42bbf-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="42bbf-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="42bbf-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="42bbf-129">Request</span></span>
<span data-ttu-id="42bbf-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42bbf-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="42bbf-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="42bbf-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42bbf-132">C#</span><span class="sxs-lookup"><span data-stu-id="42bbf-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42bbf-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="42bbf-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42bbf-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="42bbf-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="42bbf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="42bbf-135">Response</span></span>
<span data-ttu-id="42bbf-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="42bbf-136">Here is an example of the response.</span></span> 
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
