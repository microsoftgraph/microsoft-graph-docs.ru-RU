---
title: 'Filter: apply'
description: Применяет заданные условия фильтра для определенного столбца.
localization_priority: Normal
ms.openlocfilehash: 1d008b8f9df7c18d1ffc18cf2137e03fe118ef70
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277401"
---
# <a name="filter-apply"></a><span data-ttu-id="9a630-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="9a630-103">Filter: apply</span></span>

<span data-ttu-id="9a630-104">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="9a630-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a630-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a630-105">Permissions</span></span>
<span data-ttu-id="9a630-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a630-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a630-108">Permission type</span></span>      | <span data-ttu-id="9a630-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a630-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a630-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a630-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a630-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a630-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a630-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a630-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a630-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a630-113">Not supported.</span></span>    |
|<span data-ttu-id="9a630-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a630-114">Application</span></span> | <span data-ttu-id="9a630-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a630-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a630-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a630-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="9a630-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a630-117">Request headers</span></span>
| <span data-ttu-id="9a630-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9a630-118">Name</span></span>       | <span data-ttu-id="9a630-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9a630-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a630-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a630-120">Authorization</span></span>  | <span data-ttu-id="9a630-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a630-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a630-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a630-123">Request body</span></span>
<span data-ttu-id="9a630-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9a630-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9a630-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="9a630-125">Parameter</span></span>    | <span data-ttu-id="9a630-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9a630-126">Type</span></span>   |<span data-ttu-id="9a630-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9a630-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a630-128">criteria</span><span class="sxs-lookup"><span data-stu-id="9a630-128">criteria</span></span>|<span data-ttu-id="9a630-129">Воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="9a630-129">WorkbookFilterCriteria</span></span>|<span data-ttu-id="9a630-130">Применяемые условия.</span><span class="sxs-lookup"><span data-stu-id="9a630-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="9a630-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a630-131">Response</span></span>

<span data-ttu-id="9a630-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9a630-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a630-134">Пример</span><span class="sxs-lookup"><span data-stu-id="9a630-134">Example</span></span>
<span data-ttu-id="9a630-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9a630-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a630-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a630-136">Request</span></span>
<span data-ttu-id="9a630-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a630-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="9a630-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a630-138">Response</span></span>
<span data-ttu-id="9a630-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9a630-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9a630-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9a630-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9a630-141">C#</span><span class="sxs-lookup"><span data-stu-id="9a630-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/filter_apply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a630-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a630-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/filter_apply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9a630-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9a630-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/filter_apply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/filter-apply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/filter-apply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/filter-apply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
