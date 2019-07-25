---
title: 'Filter: apply'
description: Применяет заданные условия фильтра для определенного столбца.
localization_priority: Normal
ms.openlocfilehash: b06418a0254c241ab8424aa04a81101f329ef22d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859262"
---
# <a name="filter-apply"></a><span data-ttu-id="9b1e4-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="9b1e4-103">Filter: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b1e4-104">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="9b1e4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b1e4-105">Permissions</span></span>
<span data-ttu-id="9b1e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b1e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b1e4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b1e4-108">Permission type</span></span>      | <span data-ttu-id="9b1e4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b1e4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b1e4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b1e4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b1e4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b1e4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b1e4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b1e4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b1e4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b1e4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b1e4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b1e4-114">Application</span></span> | <span data-ttu-id="9b1e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b1e4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b1e4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="9b1e4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b1e4-117">Request headers</span></span>
| <span data-ttu-id="9b1e4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9b1e4-118">Name</span></span>       | <span data-ttu-id="9b1e4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9b1e4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b1e4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b1e4-120">Authorization</span></span>  | <span data-ttu-id="9b1e4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b1e4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b1e4-123">Request body</span></span>
<span data-ttu-id="9b1e4-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b1e4-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="9b1e4-125">Parameter</span></span>    | <span data-ttu-id="9b1e4-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9b1e4-126">Type</span></span>   |<span data-ttu-id="9b1e4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9b1e4-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b1e4-128">criteria</span><span class="sxs-lookup"><span data-stu-id="9b1e4-128">criteria</span></span>|<span data-ttu-id="9b1e4-129">Воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="9b1e4-129">workbookFilterCriteria</span></span>|<span data-ttu-id="9b1e4-130">Применяемые условия.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="9b1e4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b1e4-131">Response</span></span>

<span data-ttu-id="9b1e4-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b1e4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="9b1e4-134">Example</span></span>
<span data-ttu-id="9b1e4-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b1e4-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b1e4-136">Request</span></span>
<span data-ttu-id="9b1e4-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9b1e4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b1e4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b1e4-139">C#</span><span class="sxs-lookup"><span data-stu-id="9b1e4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b1e4-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="9b1e4-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b1e4-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9b1e4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9b1e4-142">Java</span><span class="sxs-lookup"><span data-stu-id="9b1e4-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9b1e4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b1e4-143">Response</span></span>
<span data-ttu-id="9b1e4-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b1e4-144">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
