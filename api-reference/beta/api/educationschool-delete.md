---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 38fcebc16d570f5d294e854643b2c5b89ddcb7b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007422"
---
# <a name="delete-educationschool"></a><span data-ttu-id="2e4e9-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="2e4e9-103">Delete educationSchool</span></span>

<span data-ttu-id="2e4e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e4e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e4e9-105">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2e4e9-105">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e4e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e4e9-106">Permissions</span></span>
<span data-ttu-id="2e4e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e4e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e4e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e4e9-109">Permission type</span></span>      | <span data-ttu-id="2e4e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e4e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e4e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e4e9-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2e4e9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e4e9-112">Not supported.</span></span>  |
|<span data-ttu-id="2e4e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e4e9-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2e4e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e4e9-114">Not supported.</span></span>  |
|<span data-ttu-id="2e4e9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e4e9-115">Application</span></span> | <span data-ttu-id="2e4e9-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4e9-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2e4e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e4e9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2e4e9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e4e9-118">Request headers</span></span>
| <span data-ttu-id="2e4e9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e4e9-119">Header</span></span>       | <span data-ttu-id="2e4e9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2e4e9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e4e9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e4e9-121">Authorization</span></span>  | <span data-ttu-id="2e4e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e4e9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e4e9-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e4e9-124">Request body</span></span>
<span data-ttu-id="2e4e9-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e4e9-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2e4e9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e4e9-126">Response</span></span>
<span data-ttu-id="2e4e9-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2e4e9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e4e9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2e4e9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e4e9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e4e9-130">Request</span></span>
<span data-ttu-id="2e4e9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e4e9-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e4e9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4e9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
# <a name="c"></a>[<span data-ttu-id="2e4e9-133">C#</span><span class="sxs-lookup"><span data-stu-id="2e4e9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e4e9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e4e9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e4e9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e4e9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e4e9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e4e9-136">Response</span></span>
<span data-ttu-id="2e4e9-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e4e9-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


