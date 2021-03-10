---
title: 'Filter: apply'
description: Применяет заданные условия фильтра для определенного столбца.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 396a02af0741be59aa054336c67c57f46c945f10
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578782"
---
# <a name="filter-apply"></a><span data-ttu-id="1ed8e-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="1ed8e-103">Filter: apply</span></span>

<span data-ttu-id="1ed8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ed8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1ed8e-105">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-105">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ed8e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ed8e-106">Permissions</span></span>
<span data-ttu-id="1ed8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ed8e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ed8e-109">Permission type</span></span>      | <span data-ttu-id="1ed8e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ed8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ed8e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ed8e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1ed8e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ed8e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1ed8e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ed8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ed8e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-114">Not supported.</span></span>    |
|<span data-ttu-id="1ed8e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ed8e-115">Application</span></span> | <span data-ttu-id="1ed8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ed8e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ed8e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="1ed8e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ed8e-118">Request headers</span></span>
| <span data-ttu-id="1ed8e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1ed8e-119">Name</span></span>       | <span data-ttu-id="1ed8e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1ed8e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ed8e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ed8e-121">Authorization</span></span>  | <span data-ttu-id="1ed8e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ed8e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ed8e-124">Request body</span></span>
<span data-ttu-id="1ed8e-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1ed8e-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="1ed8e-126">Parameter</span></span>    | <span data-ttu-id="1ed8e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1ed8e-127">Type</span></span>   |<span data-ttu-id="1ed8e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1ed8e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ed8e-129">criteria</span><span class="sxs-lookup"><span data-stu-id="1ed8e-129">criteria</span></span>|<span data-ttu-id="1ed8e-130">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="1ed8e-130">WorkbookFilterCriteria</span></span>|<span data-ttu-id="1ed8e-131">Применяемые условия.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-131">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="1ed8e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ed8e-132">Response</span></span>

<span data-ttu-id="1ed8e-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ed8e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="1ed8e-135">Example</span></span>
<span data-ttu-id="1ed8e-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1ed8e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ed8e-137">Request</span></span>
<span data-ttu-id="1ed8e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ed8e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ed8e-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1ed8e-140">C#</span><span class="sxs-lookup"><span data-stu-id="1ed8e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ed8e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ed8e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ed8e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ed8e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ed8e-143">Java</span><span class="sxs-lookup"><span data-stu-id="1ed8e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1ed8e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ed8e-144">Response</span></span>
<span data-ttu-id="1ed8e-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ed8e-145">Here is an example of the response.</span></span>
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

